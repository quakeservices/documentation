# Project Overview

Initial scope for this project is to implement a master server for Quake 2 dedicated servers; whether they are Vanilla, Q2Pro, or R1Q2.
Additional plans to include QuakeWorld and Quake 3 support in the near future.

- [Usage](#usage)
  - [Client Browsers](#client-browsers)
  - [Server Administrators](#server-administrators)
- [Contributing](#contributing)
- [Contact](#contact)


## Usage

This section covers usage by end users via client browsers, and server administrators configuring their game servers to point to this master server.

See [Deployment](https://github.com/quakeservices/documentation/blob/master/deployment.md) for information about deploying this project.

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

## Contributing

All contributions welcome; whether they are code changes for new features or to fix bugs, reporting bugs, updating documentation, and any other form of contribution.

### Code

- Spaces, no tabs, tab = 4 spaces
- Pull requests should be related to a singular feature or bug.
- Readability will be favoured over speed
- Sufficiently complex code should be commented

### Feature requests and bug reports

- Raise an issue in the appropriate GitHub repository. 
- Not sure which repository? Use [master](https://github.com/quakeservices/master/) and we can move it from there.

### License

The license for this whole project is GNU General Public License v3.0 unless otherwise stated.

## Contact

Currently handling communication through Discord: https://discord.gg/g5csDkR

Note: My timezone is AEST so communications will likely be asynchronous wherever you are in the world.
