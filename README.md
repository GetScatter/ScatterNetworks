# ScatterNetworks
A repository of networks/chains for use within Scatter

**Note: This is not a repository to add your "other" networks for existing chains.** This is a repository for adding **new** chains. If there is already a network with the `chainId` in this repository, another network will not be added as a redundant node. Networks *can be swapped out* if a network is proven to cause instability for users.

**We can not offer support for all networks that are added**. Though we will try to help in most cases, we can't take customer support responsibility for proprietary chains. 

--------------------------------------

## Adding new Networks

- Create a pull request adding your proxy to the correct blockchain in the "proxies.json" file. 
- **Fill out all of the fields, they are all required.**

```
{
  "name":"",        // The name of the Blockchain network
  "host":"",        // The FQDN for the network
  "port":-1,        // The network's port ( should always be SSL )
  "protocol":"",    // The protocol ( should always be https )
  "chainId":""      // The unique chain id for this network.
}
```

## Example Entry

```
{
  "name":"EOS Mainnet",
  "host":"nodes.get-scatter.com",
  "port":443,
  "protocol":"https",
  "chainId":"aca376f206b8fc25a6ed44dbdc66547c36c6c33e3a119ffbeaef943642f0e906"
}
```



