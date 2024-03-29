# hiv-orderly

[![Build status](https://badge.buildkite.com/238568f4671d9f391b7e48e5a225f3e1be32b7b6191caa261f.svg?branch=main)](https://buildkite.com/mrc-ide/hiv-orderly)

This is the docker container for [naomi-orderly](https://github.com/mrc-ide/naomi-orderly).

This repo is a fork of [`montagu-orderly`](https://github.com/vimc/montagu-orderly) with minor modifications

**Interaction with the server**.  These commands interact with the orderly server on the *same host* as you run it.  If you run these on your desktop they will not affect any other machine.

Make sure you have the most recent version of the container with

```
docker pull mrc-ide/hiv-orderly:latest
```

Update the `https://github.com/mrc-ide/naomi-orderly` repo on the orderly volume

```
./pull_sources
```

Run orderly commands with

```
./orderly run <name>
./orderly list names
./orderly --help
```

etc.

Get a shell on the container with

```
./shell
```

## Building the image

The image is built on [Buildkite](https://buildkite.com/mrc-ide/hiv-orderly)
