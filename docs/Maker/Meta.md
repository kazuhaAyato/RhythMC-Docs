---
sidebar_position: 1
---

# 谱面META信息

为什么是英文呢？ 因为GPT出来好像只有英文哦。

The `meta` section of a RhythMC beatmap contains essential information about the beatmap. Below is a detailed explanation of each field and how to modify them using the `/editor setmeta` command.

#### Fields

1. **name**
   - **Description**: The name of the beatmap.
   - **Example**: `"name": "Intro"`
   - **Modification Command**: `/editor setmeta name <new_name>`

2. **composer**
   - **Description**: The composer of the music used in the beatmap.
   - **Example**: `"composer": "Frkovo"`
   - **Modification Command**: `/editor setmeta composer <new_composer>`

3. **charter**
   - **Description**: The UUID of the player who created the beatmap.
   - **Example**: `"charter": "a765dbe0-44eb-3cb1-961d-3967c00c6a77"`
   - **Modification Command**: `Do Not Modify This!`

4. **level**
   - **Description**: The difficulty level of the beatmap.
   - **Example**: `"level": 1.0`
   - **Modification Command**: `/editor setmeta level <new_level>`

5. **offset**
   - **Description**: The overall offset of the beatmap, which adjusts the timing of notes.
   - **Example**: `"offset": 3`
   - **Modification Command**: `/editor setmeta offset <new_offset>`

6. **flow-speed**
   - **Description**: The speed at which notes flow in the beatmap.
   - **Example**: `"flow-speed": 1.0`
   - **Modification Command**: `/editor setmeta flow-speed <new_flow_speed>`

7. **uuid**
   - **Description**: The unique UUID of the beatmap.
   - **Example**: `"uuid": "ad3dac5d-7af7-b63e-c57b-abbf4478e1b6"`
   - **Modification Command**: `Do Not Modify This!`

8. **length**
   - **Description**: The length of the song in the beatmap.
   - **Example**: `"length": 3320`
   - **Modification Command**: `/editor setmeta length <new_length>`
