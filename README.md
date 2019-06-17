# Minecraft Forge
Docker image for a self-updating Forge modded Minecraft server.

## Usage
Create your own version of `docker-compose.yml` and use one of the following environment variables:
- `CURSE_MODPACK_ID`: for use with the [Curse modpack repository](https://minecraft.curseforge.com/modpacks).
- `MODPACK_MANIFEST_URL`: for use with a [self-hosted solution](https://hub.docker.com/r/nekroido/forge-modpack-web).

Use volume `/minecraft/merge` if you want to copy your own files into Minecraft server's root folder (e.g. whitelist.json, server-icon.png, server.properties etc).

## Volumes
- /minecraft/config
- /minecraft/logs
- /minecraft/merge
- /minecraft/mods
- /minecraft/world

## Ports
* 25565
* 25575
* 8123
* 8080

## Available environment variables
- CURSE_MODPACK_ID
- MODPACK_MANIFEST_URL
- SERVER_START_MEMORY
- SERVER_MAX_MEMORY
- SERVER_MAX_META
- SERVER_OPTS
- SERVER_LEAK_DETECTION
- JAVA_OPTS

## Contributing
Pull requests and suggestions are welcome!

## Authors
* [Nekroido](https://github.com/nekroido)

## Licence
[MIT](LICENSE)
