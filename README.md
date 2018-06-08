[DEPRECATED] go-libp2p-interface-conn
=====================================

This package has been deprecated and is no loner used by go-libp2p. Libp2p used
to build up connections as follows:

1. go "net" conn
2. multiaddr conn -- net conn with multiaddrs
3. go-libp2p-transport conn -- multiaddr conns with associated transports
4. this package -- secured, multiplexed connections
5. go-libp2p-net conn -- connections associated with a Network (e.g., go-libp2p-swarm).

However, go-libp2p-transport connections are now fully secured and multiplexed
so the interfaces in this package have been subsumed by those in
go-libp2p-transport.


[![](https://img.shields.io/badge/made%20by-Protocol%20Labs-blue.svg?style=flat-square)](http://ipn.io)
[![](https://img.shields.io/badge/project-IPFS-blue.svg?style=flat-square)](http://libp2p.io/)
[![](https://img.shields.io/badge/freenode-%23ipfs-blue.svg?style=flat-square)](http://webchat.freenode.net/?channels=%23ipfs)

> Interfaces to implement to create a connection object for use in libp2p.


## Table of Contents

- [Install](#install)
- [Contribute](#contribute)
- [License](#license)

## Install

```sh
make install
```

## Contribute

PRs are welcome!

Small note: If editing the Readme, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## License

MIT © Jeromy Johnson
