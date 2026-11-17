
# Veridium Emeralds

A data-driven NeoForge mod for Minecraft 1.21.1 that replaces Create's
`create:crushing/veridium` recipe. Create 6.0.10 or later is required.

Crushing `create:veridium` takes 250 processing ticks and independently rolls
for each result:

| Result | Count | Chance |
|---|---:|---:|
| `create:crushed_raw_copper` | 1 | 80% |
| `create:copper_nugget` | 1 | 80% |
| `minecraft:emerald` | 1 | 25% |

The recipe is supplied at
`src/main/resources/data/create/recipe/crushing/veridium.json` under the
`create` namespace so it overrides Create's existing recipe ID.

## Building

Use Java 21 and run:

```powershell
.\gradlew.bat build
```

The built mod JAR is written to `build/libs/`.
