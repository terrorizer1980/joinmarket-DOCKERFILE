# [JoinMarket](https://github.com/JoinMarket-Org/joinmarket-clientserver) Docker Images

See [dmp1ce/joinmarket](https://hub.docker.com/r/dmp1ce/joinmarket/tags/) on Docker Hub for available images.

## Tags

- `dev` ([Dockerfile](https://github.com/dmp1ce/joinmarket-DOCKERFILE/blob/master/Dockerfile))
- `latest`, `0.9.1` ([Dockerfile.release](https://github.com/dmp1ce/joinmarket-DOCKERFILE/blob/v0.9.1/Dockerfile.release))

## What is this?

A dockerized version of JoinMarket and a few helper scripts to make it easier to install and run JoinMarket scripts.

## How to use

Create a JoinMarket config file in your home directory:

`./jm wallet-tool.py`

Edit the JoinMarket config so it can connect to your bitcoin node:

`gedit ~/.joinmarket/joinmarket.cfg`

Generate a wallet:

`./jm wallet-tool.py generate`

Display your addresses:

`./jm wallet-tool.py wallet.jmdat display`

All JoinMarket data should be located at `~/.joinmarket`.

## More information

List all scripts available to run:

`docker run --rm -it --entrypoint="" dmp1ce/joinmarket ls /jm/clientserver/scripts`

See [JoinMarket repo](https://github.com/JoinMarket-Org/joinmarket-clientserver) for more information on using JoinMarket.
