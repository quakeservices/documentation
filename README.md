# Project Overview

Initial scope for this project is to impliment a master server for Quake 2 dedicated servers; whether they are Vanilla, Q2Pro, or R1Q2.
Additional plans to include QuakeWorld and Quake 3 support in the near future.

## Table of Contents

- [Usage](#usage)
  - [Client Browsers](#client-browsers)
  - [Server Administrators](#server-administrators)
- [Contact](#contact)
- [Deployment](https://github.com/quakeservices/documentation/deployment.md)
  - [infrastructure](https://github.com/quakeservices/infrastructure)
  - [master](https://github.com/quakeservices/master_deploy)
  - [web-frontend](https://github.com/quakeservices/web-frontend_deploy)
  - [web-backend](https://github.com/quakeservices/web-backend_deploy)


## Usage

This section covers usage by end users.

See [Deployment](https://github.com/quakeservices/documentation/deployment.md) for information about deploying this project.

### Client browsers

[qstat](https://github.com/multiplay/qstat) (aka quakestat) is currently the only client server browser this withwhich this application has been tested.
However any other client that allows the user to specify a master server should work.

The following command will request the list of servers:

```
quakestat -q2m master.quake.services
```

Example output:

```
$ quakestat -q2m master.quake.services
ADDRESS           PLAYERS      MAP   RESPONSE TIME    NAME
Q2M master.quake.services 1 servers    395 / 0
Q2S  116.240.207.35:27910   0/8   0/0     q2dm7     14 / 0            quake.services
```

### Server Administrators

Setting the master of a running Quake 2 server:

```
setmaster master.quake.services
```

It's recommended that this be set as part of your server config for simplicity along with any other master servers you're using.

## Contact

Currently handling communication through Discord: https://discord.gg/g5csDkR

Note: My timezone is AEST so communications will likely be asynchronous wherever you are in the world.
