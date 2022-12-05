# Metal Gear Solid 3 Cheat Engine Trainer
## Description
This is a Cheat Engine table for MGS3. It's more of a debug and testing tool than a trainer in most conventional senses, as it was not intended for cheating, but can still be used for cheats if desired. This table is also the foundation for [my chat-controlled chaos speedruns](https://youtu.be/Vusag34b8zU?t=59), along with [LioranBoard](https://github.com/LioranWaters/Lioranboard2Update/blob/main/README.md). It allows the user to control most aspects of Snake, his stats, and many of the aspects of the game world. Since this is just a Cheat Engine table with very few scripts, a basic understanding of Cheat Engine may be required to use this table—for users who don't know how to use Cheat Engine, see the Usage section, and don't be afraid to experiment to learn what something does.

This table is only compatible with the pre-patched (v1.01) digital US-region version of Metal Gear Solid 3: HD Edition, title ID NPUB30610, being emulated with RPCS3. It is not compatible with any other version of MGS3, nor is it likely to ever be compatible with any other PS3 emulator. The table can be ported to those versions, but this is not something I will ever do. This table can also be used as a tool to help with directly editing the game's memory on real PS3 hardware, as all of the base addresses are the same.

## Features
This trainer offers the ability to view and manipulate:

- The coordinates of Snake, Snake's aiming point, the camera, & Eva
- Snake's current items and weapons for each slot
- Current and max health & stamina
- Current room & subarea
- Game difficulty
- 'Game Over If Discovered' status
- All game statistics (continues, saves, alerts, kills, special items used, plants & animals captured, serious injuries sustained, damage taken, meals eaten, in-game time elapsed, life medicine used)
- Snake's velocity
- The availability of Survival Viewer menu options
- How long Snake will sleep, vomit, or be on fire for, and trigger these events
- Oxygen and grip gauge depletion
- Weapon magnification
- Weapon and item weight
- Map magnification
- Which camouflages and face paints have been obtained
- Which camouflage and face paint is currently equipped or selected
- Camo index
- The quantities and max quantities for all weapons and items, including ones not normally obtainable
- The contents of all 3 cages and 16 food slots
- The state of all 50 injury slots, including X, Y, and Z position of injuries, all 19 unique injury types and their 4,865 variants, treatments applied to injuries, and injury health

Also included are some in-development features which either might not function as expected, or might not be completed, such as:
- Caution, evasion, and alert timers
- Boss fight variables such as health, stamina, and coordinates
- Entity visiblity
- Camera type
- Guard coordinates
- Story flags
- Camera overlays
- Guard stats
- Room states

## Usage
1. Install RPCS3 and MGS3 HD (NPUB30610)
1. Install Cheat Engine version 7.2 or newer
1. Configure Cheat Engine to interpret 2 byte big endian, 4 byte big endian, and float big endian value types by following [these instructions](https://gist.github.com/jordanbtucker/384b67d2b7ccf4e478fb20ae86b13a41)
1. In Cheat Engine, navigate to _Edit_ > _Settings_ (or click the _Settings_ button in the top right of the main Cheat Engine window), navigate to the _Scan Settings_ section, and ensure that _MEM_PRIVATE_, _MEM_IMAGE_, and _MEM_MAPPED_ are all ticked
1. Download this trainer (MGS3__NPUB30610_.CT) and double click it to open it. When prompted, allow the script to run. This script is required for most of the trainer's features to function. See the Potentially Asked Questions to learn more about it.

All done! Enjoy the trainer.

**Example usage:** to give Snake pseudo-God mode, open the `Stats` section by clicking the box to the left of the `Stats` label, click on `Current Health`, then press `Enter` and type any big number that is smaller than 32,767. Press `Enter` again to confirm the value change, then click the box to the left of the `Current Health` label to activate the entry, which causes Cheat Engine to repeatedly write its value to memory.

To configure the trainer for use with LioranBoard (or similar stream decks), simply
1. Right click an entry that you want to control with the stream deck and click _Set/Change hotkeys_, then set a hotkey and action as desired
1. Configure your stream deck to actuate that key when the desired conditions are met.

**For example:** to allow a Twitch chat to kill Snake by redeeming channel points, right click `Current Health` within the `Stats` section, click `Set/Change hotkeys`, click `Create hotkey` in the popup window, and assign a key. Select `Set value to:` in the dropdown, and type `0` in the box beneath that. Then, within your stream deck software, configure a trigger that activates when someone redeems the appropriate channel point reward, and have the trigger actuate the hotkey defined for the entry in Cheat Engine.

## Potentially Asked Questions
**Q:** When I open the table, it asks me to run a script. What is it?<br>
**A:** Cheat Engine interprets all pointers as little endian, and is not natively capable of interpreting them as big endian, which is how the PS3 architecture interprets its values. In order to interpret pointers as big endian automatically, a script is required to convert them. The script was written by [bmn](https://github.com/bmn), author of the [MGS2 PC Trainer](https://mgs.w00ty.com/mgs2/trainer/) and other Metal Gear tools.

**Q:** Will you add [feature]?<br>
**A:** Maybe. Check the extras section on the table (bottom right of the main Cheat Engine window) to see if I already have it planned. Send feature requests to `Major Zero#1516` on Discord.

## Support
The best place to learn Cheat Engine basics is YouTube. Barely any Cheat Engine knowledge or experience is required to use this, so just experiment to learn how it works. If you're really stuck, message `Major Zero#1516` on Discord.

## Attribution
- apel for general Cheat Engine advice, and for showing me how to find pointers manually. The table would have never gotten anywhere without him.
- bmn for writing the script to convert pointers to big endian. Likewise, he was instrumental in this table's progress.
- Dark Byte and all other Cheat Engine contributors for making Cheat Engine.


## License
Do whatever you want with this, I don't care. There's probably an applicable license for this. Just don't pretend you made it yourself.
