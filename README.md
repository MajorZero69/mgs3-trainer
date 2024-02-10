# Metal Gear Solid 3 Cheat Engine Trainer
## Description
This is a Cheat Engine table for MGS3. It's more of a debug and testing tool than a trainer in most conventional senses, as it was not intended for cheating, but can still be used for cheats if desired. This table is also the foundation for [my chat-controlled chaos speedruns](https://youtu.be/Vusag34b8zU?t=59), along with [LioranBoard](https://github.com/LioranWaters/Lioranboard2Update/blob/main/README.md). It allows the user to control most aspects of Snake, his stats, and many of the aspects of the game world. Since this is just a Cheat Engine table with very few scripts, a basic understanding of Cheat Engine may be required to use this table—for users who don't know how to use Cheat Engine, see the Usage section, and don't be afraid to experiment to learn what something does.

This table is only compatible with the PC version of Metal Gear Solid 3: Snake Eater - Master Collection Version. It is not compatible with any other version of MGS3; for the existing PS3 version of this table, see the PS3 Version folder in this repo. The table can be ported to other versions, but this is not something I will ever do.

## Features
This trainer offers the ability to view and manipulate:

- The coordinates of Snake, Snake's aiming point, the camera, & Eva
- Snake's current items and weapons for each slot
- Boss fight variables such as health, stamina, and coordinates
- Guard variables such as health, stamina, and coordinates
- Current and max health & stamina
- Current room & subarea
- Game difficulty
- All game statistics (continues, saves, alerts, kills, special items used, plants & animals captured, serious injuries sustained, damage taken, meals eaten, in-game time elapsed, life medicine used)
- How long Snake will sleep, vomit, or be on fire for, and trigger these events
- Oxygen and grip gauge depletion
- Which camouflages and face paints have been obtained
- Which camouflage and face paint is currently equipped or selected
- Camo index
- The quantities and max quantities for all weapons and items, including ones not normally obtainable
- The contents of all 3 cages and 16 food slots
- The state of all 50 injury slots, including X, Y, and Z position of injuries, and injury stats

Also included are some in-development features which either might not function as expected, or might not be completed, such as:
- Caution, evasion, and alert timers
- Entity visiblity
- Camera type
- Story flags
- Camera overlays
- Room states

## Usage
1. Install MGS3 Master Collection Version (1.3.0 or newer, preferably newer)
1. Install Cheat Engine
1. Download this trainer and double click it to open it.
1. Click the glowing button in the top left of the Cheat Engine window and select the MGS3 process (METAL GEAR SOLID3.exe)

All done! Enjoy the trainer.

**Example usage:** to give Snake pseudo-God mode, open the `Stats` section by clicking the box to the left of the `Stats` label, click on `Current Health`, then press `Enter` and type any big number that is smaller than 32,767. Press `Enter` again to confirm the value change, then click the box to the left of the `Current Health` label to activate the entry, which causes Cheat Engine to repeatedly write its value to memory.

To configure the trainer for use with LioranBoard (or similar stream decks), simply
1. Right click an entry that you want to control with the stream deck and click _Set/Change hotkeys_, then set a hotkey and action as desired
1. Configure your stream deck to actuate that key when the desired conditions are met.

**For example:** to allow a Twitch chat to kill Snake by redeeming channel points, right click `Current Health` within the `Stats` section, click `Set/Change hotkeys`, click `Create hotkey` in the popup window, and assign a key. Select `Set value to:` in the dropdown, and type `0` in the box beneath that. Then, within your stream deck software, configure a trigger that activates when someone redeems the appropriate channel point reward, and have the trigger actuate the hotkey defined for the entry in Cheat Engine.

## Potentially Asked Questions
**Q:** Will you add [feature]?<br>
**A:** Maybe. Check the extras section on the table (bottom right of the main Cheat Engine window) to see if I already have it planned. Send feature requests to `major.zero` on Discord.

## Support
The best place to learn Cheat Engine basics is YouTube. Barely any Cheat Engine knowledge or experience is required to use this, so just experiment to learn how it works. If you're really stuck, message `major.zero` on Discord.

## Attribution
- apel for general Cheat Engine advice, and for showing me how to find pointers manually. The table would have never gotten anywhere without him.
- bmn for writing the script to convert pointers to big endian, which was used in the original PS3 version of this table. Likewise, he was instrumental in this table's progress.
- Dark Byte and all other Cheat Engine contributors for making Cheat Engine.


## License
Do whatever you want with this, I don't care. There's probably an applicable license for this. Just don't pretend you made it yourself.
