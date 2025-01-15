# CS2-Practice_GUI
This `practice_gui.cfg` file lets you setup a practice server very easy to tweak through console with a GUI for CS2, it does not require the other files.
Its main goal is to be noob friendly, so don't get overwhelmed by the installation, it's actually very easy !
It also fits advanced user with very in-depths functionalities !

It comes with two additional files containing utility aliases (`alias_maps.cfg` and `alias_stuff.cfg`), you should take a look at them, you might find something interesting !
One core file that allows `practice_gui.cfg` to add a visual feedback (`practice_gui_hint.cfg`).
And a `practice_gui_user.cfg` file to enable easy modifications with some documentation, this very last one should be the only one to be modified unless you want to break everything !

## POST UPDATE [19th Dec. 2024](https://steamcommunity.com/games/CSGO/announcements/detail/529833471389991083) :
Due to some changes from this update, various stuff might be broken at the moment.

Overall, great improvements can be expected soon™ thanks to the new features provided by valve !

PS : After noticing many core issues, I'm considering rewriting everything from scratch, so it might take a bit of time, I'll try to maintain this version to keep it usable until then, soon™ is an actual one.. :x

## POST UPDATE [15th January 2025](https://steamcommunity.com/games/CSGO/announcements/detail/518577002799693839) :
   **Warning : Due to the way practice_guy currently implements hud_hints when triggering an option and recent updates to VAC; it is highly recommended to restart your game before joining a VAC secured server to avoid the risks of being flagged for abusing exec_async.
   If you want to remove that risk, you can delete practice_gui_hints.cfg which reloads recursively the hud_hint entities (You won't get the HUD feedback if you do so).
   Anyone using practice_gui outside of its purposed scope will be the only one responsible of its consequences, so use it at your own risks until I get more info about it !**

## Installation
0. For experienced cfg user only : If you are using an `autoexec`, you can just paste this line into it so you just have to type `practice_gui` in console to use this config (after dropping the files into the right folder).

        alias "practice_gui" "sv_cheats 1; exec_async practice_gui"


1. Open the archive and extract its content into the following path folder :

        ...\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\

2. Launch the game, boot up a practice server where you can turn on `sv_cheats 1`.

        Game Menu -> PLAY -> Practice -> Casual -> Select Map -> GO

3.  Now that you're in the server, you can type in the following commands to your console :

        sv_cheats 1; exec_async practice_gui.cfg

4. In case your console spit a bunch of errors, just type `practice_gui` and you should be good to go !

        practice_gui

5. Your console should now display the GUI; otherwise you must have a path issue and the file did not load correctly.

6. **Due to the way practice_guy currently implements hud_hints when triggering an option, it is highly recommended to restart your game before joining a VAC secured server to avoid the risks of being flagged for abusing exec_async.
   If you want to remove that risk, you can delete practice_gui_hints.cfg which reloads recursively the hud_hint entities (You won't get the HUD feedback if you do so).**

## Customization
If you want to modify stuff in this config, I would recommend you to use `practice_gui_user.cfg`, you will find some documentation on how to do so, modifying the `practice_gui.cfg` will probably break the GUI in many ways.

## Usage
- A self explanatory documentation will be displayed through the GUI in your console under this format :
  
        VARS (STATUS) | CycleCmd / ToggleOnCmd / ToggleOffCmd

- Toggle practice mode ON and OFF by simply typing `practice` in your console for example.

- Type `helpprac` to display the GUI in your console to see the current status of the vars.

- Type `give_[nameofitem]` to get it dropped instantly. (`alias_stuff.cfg`)
- Type `[nameofmap]` to change map instantly. (`alias_maps.cfg`)

- Everytime you change map, you will need to type `practice_gui` (rebooting the cfg) in your console since the server convars gets overwritten.
- The GUI will not keep in memory any cvar that is changed manually in the console.

## Examples
Here's a few screenshots to give you an idea of how it works :

Booting up the server

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/f9fa6812-6a92-499e-b64c-d136feebe905)

Loading the config

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/361ab487-9ff1-427c-b648-8c9c422c9681)

Config has been loaded

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/de5d67f2-cba5-4304-843b-2fd7a0b0e324)

Practiceon

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/ce51ac99-a862-407d-a29c-6691248d978f)

Practiceoff

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/bdaadc34-aa8d-485f-97bb-4b2b463eaa3c)

Pracbhopon

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/2edc5d85-30dc-4e55-b95b-55b2446a21bc)

PracWb2on

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/b5c50e8c-e42f-4b16-97f5-123f8184e9ad)

Pracsound

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/db43fa95-deda-48ec-9944-93cda5aff873)


Have fun practicing for the grind ! :)


### KNOWN ISSUES
- Lastly added commands aren't included into `pracman` just yet.
- The usage of custom fonts in CS2 can break the layout of the GUI, I'm looking for a solution but different fonts can have different spacing which makes it odd to overcome. 


### FUTURE UPDATES
I'm currently working on this set of configs, I'm planning on adding :
- Current Map feedback in the GUI
- Change knife skin on a keypress
- Control over the gui_interface through custom radialradios wheel ! > `practice_gui` :
- Map configs including default map spawns aliases on radialradios wheel with map automatic detection... Maybe?
- Grenades / Wallbang setups... Maybe?

### NEW UPDATE

#### ADDED :
- Added Hint_text Feedback directly on the HUD ! 
- Added `cl_allow_multi_input_binds` support in the GUI
- Reworked the loadbar interface completely for fancier and more accurate animation, even added custom color templates !
- Added `prac_showpos` support
- Added many niche aliases to bind in `practice_gui_user.cfg` 
- Added Hitreg debugging `prachitreg`

#### MODIFIED :
- Improved the behaviour of `praccolor` in the GUI
- Updated/Tweaked many `prac_cmds` + cleanup of the `prac_help`, there might be wrong values that I missed
- Fixed various bugs/typos/missalignments
- Improved `prac_noclip` behaviour in GUI
- Modified `pracset`, added commands for faster reboot (removed game start animation screen)
- Added `praclbhop` values
- Improved `pracbot` setup in order to be able to place bots facing the player easily
- Improved `pracbuy` setup for less buy limitations, it might have unexpected repercussions, but it is now possible to buy unlimited weapons (zeus included), only buy limit will be with grenades, which is not a big deal
- Improved `pracwh`, with a new value
- A recent update broke the `practpose`, some cursed stuff will occur upon usage

#### REMOVED :
- `spec_xray_dropped_unoccluded` from prachud because valve deprecated the cvar
- `spec_xray_dropped_defusekits` from prachud because valve deprecated the cvar
- `spec_hide_players` from prachud because valve deprecated the cvar

#### NOTE :
- `pracman` has not been updated yet, consider it outdated
- `pracset` might have unexpected behaviour when used manually, will have to look into it
- It has been a big merge so some stuff might have broke without notice !

#### FIXES :
- Many aliases were not loaded properly leading to random errors in console and weird behaviours in some cases, it should all be fixed by now !
- Renamed bhop modes in GUI for better clarity.
- Cleaned up a few old deprecated commands that remained executed randomly.
- Reduced bot_quota to 20, just in case someone had the idea of launching the game with launch parameter `-maxplayers_override 64`.
- Switched Sound Feedback ON by default.
