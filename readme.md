# Remote Exchange Subgraph
![TESTS](https://github.com/remote-exchange/remote-exchange-subgraph/actions/workflows/test.yml/badge.svg)


## Install

Install dependencies `yarn`

Generate types `yarn codegen`

Build the project `yarn build`

Very useful deploy subgraph on the local [graph-node](https://github.com/graphprotocol/graph-node).


## Testing

More about tests on [matchstick](https://thegraph.com/docs/en/developer/matchstick/)

On Linux/MacOS run tests should work with `graph test`

On Windows you can run test with following command (make sure you have installed docker)

`docker run -t --rm --mount type=bind,source=<ABSOLUTE_PATH_TO_REPO>,target=/matchstick belbix/subgraph:matchstick`

For run concrete test you can add env variables to the docker run like `-e ARGS="controller"`

Or build your own Docker image from [Dokerfile](./Dockerfile)

## Endpoints

* Goerli https://api.thegraph.com/subgraphs/name/a17/remote-testnet
