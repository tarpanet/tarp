# tarp
_peer-to-peer networking for boring people_

tarp is a peer-to-peer network for people who really don't want to care about the details. It's designed to get data from point A to point B, no matter the weather.

## Technical details

### Identity
Each tarp node generates a public-private key pair. The hash of its public key is its unique identifier across the tarp network: no two tarp nodes can have the same identity unless they both have the same private key.

### Routing
Each tarp node maintains a Kademlia routing table of other nodes and maintains open WebRTC connections to each node.
