## Minecraft Acorn

This Acorn provides a Minecraft server that can be connected to from the Minecraft Java edition and the Minecraft Bedrock edition.

NOTE: Running this Acorn means you agree to the Minecraft EULA.  

## Tl;dr

Click this button to deploy the Minecraft Acorn to your own Acorn Sandbox:

[![Run in Acorn](https://acorn.io/v1-ui/run/badge?image=ghcr.io+cloudnautique+minecraft-acorn:latest-%23&ref=cloudnautique)](https://acorn.io/run/ghcr.io/cloudnautique/minecraft-acorn:latest-%23?ref=cloudnautique)

## Quick Start

To get up and running quickly from the Acon CLI just run the command below.

```shell
acorn run ghcr.io/cloudnautique/minecraft-acorn:latest-#
```

This will start a Minecraft server that is accessible from Minecraft Java and Bedrock clients. Bedrock is the version of Minecraft that runs on Windows 10, Xbox, Playstation, Nintendo Switch, iOS, and Android. Mac OSX and Linux users can use the Java edition.

## Options

The following options are available for this Acorn.

```shell
--allowFlight         Allow characters to fly
--difficulty string   Difficulty level of the game. Options are "peaceful", "easy", "normal", "hard". Default is "easy"
--eula                This must be TRUE to accept the EULA
--geyser              Enable GeyserMC. Allows Bedrock clients to connect to the server.
--mode string         Mode: "creative or survival". Default is "survival"
--version string      Version of Minecraft paper to download. Current version is 1.20.2
```

If you would like to only allow Java Clients to connect to your server, you can disable GeyserMC by passing the `--geyser=false` option.

If you do not agree to the EULA, the Acorn will not run. You can agree to the EULA by passing the `--eula=true` option, which is the default.

You can change the difficulty of the game by passing the `--difficulty` option. By default it is set to `peaceful`, but can be set to `easy`, `normal`, or `hard` for more of a challenge.

You can also set the mode from `creative` to `survival` by passing the `--mode` option. By default it is set to `creative`. In creative mode, you have unlimited resources, can fly, and can't be hurt by anything. In survival mode, you have to gather resources and can be hurt by mobs.
