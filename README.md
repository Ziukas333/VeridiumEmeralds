# Veridium Emeralds

Veridium Emeralds is a small, data-driven mod for Minecraft 1.21.1. It changes what Create's crushing wheels can get from raw Veridium: crushed raw copper, copper nuggets, and a chance of emeralds.

## Features

Crushing one raw `create:veridium` independently rolls for each of these results:

| Result | Chance |
| --- | ---: |
| 1 `create:crushed_raw_copper` | 80% |
| 1 `create:copper_nugget` | 80% |
| 1 `minecraft:emerald` | 10% |

## Supported versions

- Minecraft: **1.21.1**
- NeoForge: **21.1.265 or newer in the 21.1 line**
- Create: **6.0.10 or newer**
- Veridium Emeralds: **1.0.0**

## Requirements

You need:

- A Minecraft 1.21.1 server or game using NeoForge.
- The NeoForge loader.
- Create 6.0.10 or newer.
- **Both** the Veridium Emeralds mod JAR and the external `veridiumemeralds-override.zip` datapack.

The mod JAR and datapack ZIP do different jobs. Installing only one is not enough for the intended recipe override.

## Installation

1. Stop the server, or close the game and world.
2. Put the Veridium Emeralds mod JAR in the instance or server's `mods` folder. Create must also be installed there.
3. Put `veridiumemeralds-override.zip` in the `datapacks` folder of the world you want to use. For a server using the default world folder, this is usually `world/datapacks/` under the server directory. Keep the ZIP compressed; do not extract it.
4. Start the server and load the target world.
5. In that world, enable the datapack at highest priority by running:

   ```text
   /datapack enable "file/veridiumemeralds-override.zip" last
   ```

6. If the server reports a different pack name in `/datapack list available`, use the exact name it reports. If the pack is already enabled, disable it first, then enable it with `last`.
7. Run `/reload`, or restart the server/reopen the world, so the datapack is applied.

For multiplayer, install the mod JAR on the server and ensure Create is present as a required dependency. The recipe data is loaded by the server; clients do not need this recipe-only mod to join.

## Credits

Recipe support depends on [Create](https://github.com/Creators-of-Create/Create). Thanks to the Create developers and contributors for making Create and maintaining its recipes and modding support.

## License

Veridium Emeralds is distributed under the MIT License. See [LICENSE](./LICENSE).
