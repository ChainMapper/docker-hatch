# docker-hatch
Wallet and daemon for Hatch [HATCH] cryptocurrency on docker

# Quickstart
Type `docker run -it -e "USER=someuser" -e "PASSWORD=topsecret" -e "RPCALLOW=127.0.0.1" chainmapper/hatch` and see the wallet starting.

Alternatively type `docker run -it -v "<path_to_config>:/config/hatch.conf" chainmapper/hatch` to use your own config.

```
Docker HATCH wallet

By: ChainMapper
Website: https://chainmapper.com

Starting HATCH daemon...
```

# Proper start
Use a volume to store all data. The image stores it's data in `/data`. So mapping that volume will do the trick.

Additionally you can override the config and wallet file using volumes pointing to `/config/hatch.conf` and `/config/wallet.data`

# License
MIT, see LICENSE file