# Trust periods in Phase 1b

## A big part of Game of Zones is learning to use the relayer.

The relayer is pretty complex piece of software and documentation is still emerging. For the purposes of Game of Zones 1b, we want to players to pay close attention to how they initialize the connection on their relayer.

The trust period is a value in the on-chain light client that powers IBC. In a production IBC chain, the trust-period of a the on-chain light client should be slightly shorter the unbonding period of the chains.  This means a period of 21 days for a chain connected to the Cosmos hub. When creating a client for IBC, the creator can choose any trust period they want. 

As part of the Game of Zones, we are encouraging player to create make a choice. A shorter trust period will provide a high score in the phase 1b ranking and a longer trust period will cost less gas and be easier to maintain. 

Trust periods created using the relayer must be defined in the configuration *before* the relayer created a client. 

The trust period the relayer will create is set in the configuration for the chain in `config.yaml`

``` yaml
chains:
- key: testkey
  chain-id: gameofzoneshub-1b
  rpc-addr: http://localhost:26657
  account-prefix: cosmos
  gas: 200000
  gas-prices: 0.0025doubloons
  default-denom: doubloons
  trusting-period: 10m
```

Players can choose any trust period they want. They need to balance a limited about gas to keep updates and risks of network congestion blocking update.

Remember the Game of Zones team will be scoring each teams’s longest lived channel.

Remember to make all these choice before creating your client with `rly transact link` because trust periods are immutable.