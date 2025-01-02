# Level Format

## Byte Order

The level data is stored in **Big Endian** byte order.

## Level Data

| Name | Size (in bytes) | Description |
|------|-----------------|-------------|
| Magic Number | 4 | Identifier of the format. Always `27 1B B7 88`. |
| Version | 1 | Version of the format. Always `02`. |
| Serialized Java `com.mojang.minecraft.level.Level` Class | Variable | Contains all the level information, player data, entities, and more.[\[1\]](#1) |

## Notes
1. <a id="1"></a> Due to a bug in Minecraft Classic the `Height` and `Depth` values are swapped causing Height to be the Depth and Depth to be the Height.