# Raptor V90

Unofficial Powkiddy V90/MiyooCFW port of **Raptor: Call of the Shadows**.

This port is based on [RetroGamer02/raptor-consoles](https://github.com/RetroGamer02/raptor-consoles), branch `multi-sys`, version 1.0.4. The upstream project is based on reconstructed and reverse-engineered Raptor source code by nukeykt, wel97459, skynettx and other contributors.

## Features

* Powkiddy V90 support
* MiyooCFW 2.0.0-beta-2
* SDL 1.2 controls
* ARM-safe animation and sprite decoding
* Pixel-perfect 320×200 image centered on the 320×240 display
* Music and sound effects
* Pilot save and load
* Automatic `PLAYER / RAPTOR` registration without a keyboard
* Hangar, store and complete campaign support

## Required game data

Commercial Raptor game data is **not included** in this release.

You must provide the data files from a legally owned DOS version 1.2 copy of **Raptor: Call of the Shadows**.

The full version requires these five files:

* `FILE0000.GLB`
* `FILE0001.GLB`
* `FILE0002.GLB`
* `FILE0003.GLB`
* `FILE0004.GLB`

All five files must be placed in the same directory as `raptor.elf` and `Raptor.sh`.

On the Powkiddy V90 SD card, the required directory is:

```text
/mnt/games/Raptor/
```

When the SD card is connected to a Windows computer, open its main partition and navigate to:

```text
games\Raptor\
```

Copy the five `FILE*.GLB` files into that folder.

Do not place them:

* in the root of the SD card;
* inside the `SOURCE` folder;
* inside the `gmenu2x` folder;
* inside an additional nested folder such as `games\Raptor\Raptor\`.

The final `games\Raptor` directory should contain at least:

```text
games\Raptor\raptor.elf
games\Raptor\Raptor.sh
games\Raptor\SETUP.V90.INI
games\Raptor\raptor.png
games\Raptor\FILE0000.GLB
games\Raptor\FILE0001.GLB
games\Raptor\FILE0002.GLB
games\Raptor\FILE0003.GLB
games\Raptor\FILE0004.GLB
```

## Installation

### Method 1: Extract directly to the SD card

1. Download `Raptor_V90_v1.0_PUBLIC_no_game_data.zip` from the [Releases](../../releases) page.

2. Insert the Powkiddy V90 SD card into your computer.

3. Open the main SD-card partition in Windows Explorer.

4. Extract the ZIP directly to the root of the SD card.

5. If Windows asks whether to merge the existing `games` or `gmenu2x` folders, choose **Yes**.

6. Open the following directory on the SD card:

   ```text
   games\Raptor\
   ```

7. Copy your legally owned `FILE0000.GLB` through `FILE0004.GLB` files into that directory.

8. Safely eject the SD card and return it to the Powkiddy V90.

9. Start **Raptor: Call of the Shadows** from the Games section.

### Method 2: Prepare everything on the computer first

1. Create a temporary folder on your computer.

2. Extract `Raptor_V90_v1.0_PUBLIC_no_game_data.zip` into that folder.

3. Open:

   ```text
   games\Raptor\
   ```

4. Copy `FILE0000.GLB` through `FILE0004.GLB` into that folder.

5. Copy the prepared `games` and `gmenu2x` folders to the root of the V90 SD card.

6. Allow Windows to merge them with the folders already present on the SD card.

7. Safely eject the SD card and start the game.

On the first launch, `Raptor.sh` automatically creates `SETUP.INI` from the supplied `SETUP.V90.INI`.

Pilot saves are stored in the same game directory as:

```text
CHAR0000.FIL
CHAR0001.FIL
...
CHAR0009.FIL
```

When updating an older installation, back up `SETUP.INI` and any `CHAR*.FIL` files if you want to preserve your settings and pilots.


## License and credits

The source port is distributed under the GPL-2.0 license.

Raptor: Call of the Shadows and its original commercial assets belong to their respective copyright holders.

This is an unofficial community port and is not affiliated with the original game's publisher or developers.
