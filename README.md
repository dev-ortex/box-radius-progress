# 📌 Box Radius Progress

A Pawn include to create progress bars with borders using `TextDraws`. Perfect for HUD systems, timed actions, or visual feedback for players.

## Installation

1. Download the latest version of the `box_radius.inc` include.
2. Place the file inside your server’s `include/` folder.
3. Include it in your gamemode or filterscript:

```pawn
#include <box_radius>
```
4. Install [YSF](https://github.com/IllidanS4/YSF).


---

## ⚙️ Natives Functions

```pawn
native CreatePlayerBoxRadius(playerid, Float:pos_x, Float:pos_y, color = 0x1E90FFFF, bgcolor = 0x1C1C1CFF, Float:size = 5.0);
native UpdatePlayerBoxRadiusProgress(playerid, id, Float:value);
native DestroyPlayerBoxRadiusProgress(playerid, id);
native DestroyPlayerBoxRadiusAll(playerid);
```

> [!IMPORTANT]
> * `color`: Progress bar color.
> * `bgcolor`: Background color.
> * `size`: Base size of the bar.
> * `value`: Progress value from 0 to 100.

## 📝 Example Usage

```pawn
CMD:progress(playerid, const params[])
{
    new id = CreatePlayerBoxRadius(playerid, 320.0, 150.0);
    UpdatePlayerBoxRadiusProgress(playerid, id, 50.0); // 50%
    return 1;
}
```

## 📷 Demo Video

https://github.com/user-attachments/assets/26d3ed26-a75f-4dba-983d-481b4e50b5b3

## 📝 Credits

* Ortex – Original author of the code.

## 🌐 Other languages
* [Português](https://github.com/dev-ortex/box-radius-progress/blob/main/READMPT.md)
* [Inglês](https://github.com/dev-ortex/box-radius-progress/blob/main/README.md)
