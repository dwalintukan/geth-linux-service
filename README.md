# geth-linux-service

These instructions help you setup a `geth` node as a Linux service. It will auto-run on reboots.

## Minimum Requirements

1. Linux-based AMD64 arch type OS
2. Dual-core CPU
3. 2 GB RAM

## Add Geth Binary

Copy the `geth binary` to `/usr/local/bin` so it can be used.

## New Node Setup

1. Clone repo
2. Edit env file
3. Run init script: `./init.sh`. This creates a Linux system service for geth among other necessary setup.
4. Note that the `geth` system service is now setup to auto-run on reboots.

## Start Node

```bash
./start.sh
```

## Stop Node

```bash
./stop.sh
```

## Check Node Status

```bash
systemctl status geth
```

## Logging

Logs are stored and rotated in `/var/log/geth/geth.log`.
