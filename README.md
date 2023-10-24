# README

## Everest Smart Chain

[![Version](https://img.shields.io/github/tag/tharsis/evmos.svg) ](https://github.com/EverestSmartChain/EverestSmartChain/releases)[![License: Apache-2.0](https://img.shields.io/github/license/tharsis/evmos.svg) ](https://github.com/evmos/evmos/blob/main/LICENSE)[![GoDoc](https://godoc.org/github.com/evmos/evmos?status.svg) ](https://pkg.go.dev/github.com/evmos/evmos)[![Go report card](https://goreportcard.com/badge/github.com/evmos/evmos) ](https://goreportcard.com/report/github.com/evmos/evmos)[![Lines of code](https://img.shields.io/tokei/lines/github/tharsis/evmos)](https://bestpractices.coreinfrastructure.org/projects/5018)[![Discord](https://img.shields.io/discord/809048090249134080.svg) ](https://discord.gg/pDv6sERWFF)[![Lint Status](https://github.com/evmos/evmos/actions/workflows/lint.yml/badge.svg?branch=main) ](https://github.com/evmos/evmos/actions?query=branch%3Amain+workflow%3ALint)[![Code Coverage](https://codecov.io/gh/evmos/evmos/branch/main/graph/badge.svg)](https://codecov.io/gh/evmos/evmos)

Everest Smart Chain is a scalable, high-throughput Proof-of-Stake blockchain that is fully compatible and interoperable with Ethereum. It's built using the [Cosmos SDK](https://github.com/cosmos/cosmos-sdk/) which runs on top of the [Tendermint Core](https://github.com/tendermint/tendermint) consensus engine.

### Documentation

Our documentation is hosted in a [separate repository](https://github.com/EverestSmartChain/docs) and can be found at [docs.everestchain.net](https://docs.everestchain.net). Head over there and check it out.

**Note**: Requires [Go 1.20+](https://golang.org/dl/)

### Installation

For prerequisites and detailed build instructions please read the [Installation](https://docs.evmos.org/protocol/evmos-cli) instructions. To Quickly Spin up a validator Node or a Full Node below steps are Enough&#x20;

```bash
#Ubunto 20.04 Prefered 

# Install Dependicies 

apt install jq make bc gcc

# Install golang 

curl -OL https://go.dev/dl/go1.21.3.linux-amd64.tar.gz
tar -C /usr/local -xvf go1.21.3.linux-amd64.tar.gz
nano ~/.profile

#add the below in the last line on /.profile

. . .
export PATH=$PATH:/usr/local/go/bin

source ~/.profile

#clone this repository 

git clone https://github.com/EverestSmartChain/EverestSmartChain
cd EverestSmartChain
make install

# once make finishes your binaries will be avilable in /root/go/bin/

# Create EVT keys prior starting the Chain , Assuming you are inside the Directlry where binary is i.e /root/go/bin/  (replace your-identifier-name with any name you like)

./evtd keys add your-identifier-name  

#initialize the chain 

./evtd init your-identifier-name --chain-id "evt_8848-1"

#Once the Chain is initialized some files will be generated inside /root/.evtd/config/
# We need to Supply the Original genesis.json file prior starting the chain


```

Or check out the latest [release](https://github.com/evmos/evmos/releases).

### Quick Start

To learn how the Everest Smart Chain works from a high-level perspective, go to the [Protocol Overview](https://docs.evmos.org/protocol) section from the documentation. You can also check the instructions to [Run a Node](https://docs.evmos.org/protocol/evmos-cli#run-an-evmos-node).

### Community

The following chat channels and forums are a great spot to ask questions about Evmos:

* [Evmos Twitter](https://twitter.com/EverestC19862)
* [Evmos Discord](https://discord.gg/pDv6sERWFF)

### Contributing

Looking for a good place to start contributing? Check out some [`good first issues`](https://github.com/EverestSmartChain/EverestSmartChain/issues).

For additional instructions, standards and style guides, please refer to the [Contributing](broken-reference) document.
