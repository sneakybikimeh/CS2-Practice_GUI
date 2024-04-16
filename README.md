# CS2-Practice_GUI
This practice_gui.cfg file lets you setup a practice server very easy to tweak through console with a GUI for CS2, it does not require the other files.
Its main goal is to be noob friendly, so don't get overwhelmed by the installation, it's actually very easy !

It comes with two additional files containing utility aliases, and a practice_gui_user.cfg file to enable easy modifications with some documentation.

## Installation
0. If you are using an autoexec, you can just paste this line into it so you just have to type "practice_gui" in console to use this config (after dropping the files into the right folder).

        alias "practice_gui" "sv_cheats 1; exec_async practice_gui"


1. Open the archive and extract its content into the following path folder :

        ...\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\

2. Launch the game, boot up a practice server where you can turn on sv_cheats 1.

        Game Menu -> PLAY -> Practice -> Casual -> Select Map -> GO

3.  Now that you're in the server, you can type in the following commands to your console :

        sv_cheats 1; exec_async practice_gui.cfg

4. In case your console spit a bunch of errors, just type "practice_gui" and you should be good to go !

        practice_gui

5. Your console should now display the GUI; otherwise you must have a path issue and the file did not load correctly.

## Customization
If you want to modify stuff in this config, I would recommend you to use practice_gui_user.cfg, you will find some documentation on how to do so, modifying the practice_gui.cfg will probably break the GUI in many ways.

## Usage
- A self explanatory documentation will be displayed on the GUI in your console under this format :
  
        VARS (STATUS) | CycleCmd / ToggleOnCmd / ToggleOffCmd

- Toggle practice mode ON and OFF by simply typing "practice" in your console for example.

- Type helpprac to display the GUI in your console in order to see the current status of the vars.

- Type give_[nameofitem] to get it dropped instantly. (alias_stuff.cfg)
- Type [nameofmap] to change map instantly. (alias_maps.cfg)

- Everytime you change map, you will need to type "practice_gui" in your console since the server convars gets overwritten.
- The GUI will not keep in memory any var that is changed manually in the console.

## Examples
Here's a few screenshots to give you an idea of how it works :

Booting up the server

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/f9fa6812-6a92-499e-b64c-d136feebe905)

Loading the config

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/361ab487-9ff1-427c-b648-8c9c422c9681)

Practiceon

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/3422238f-e3d3-4362-a0f5-5201796c084e)

Practiceoff

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/3fdd3b6b-be07-4960-a942-97408763e3d6)

Pracbhopon

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/3cc19b99-de9e-4e5d-a2bd-13f10f8b878b)

PracWb2on

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/60056e53-fee8-4ef6-930a-53ce2fa193ef)

Pracsound

![image](https://github.com/sneakybikimeh/CS2-Practice_GUI/assets/151694137/9f5af7e8-1b65-4b9d-a021-88635dbc6d51)


Have fun practicing for the grind ! :)



### FUTURE UPDATES
I'm currently working on this set of configs, I'm planning on adding :
- Flashlight pointer bind
- Lock Camera bind
- Unlock yaw limits + mouse invert
- New features I haven't though of just yet / that gets requested > practice_gui :

### NEW UPDATE
(+/-) improved the behaviour of a lot of stuff, almost everything have been reworked/improved, replacing practice_gui.cfg is highly recommended
(+/-) an update will follow for practice_gui_user.cfg and README.md in the upcomming days.
(+/-) mp_match_end_restart added into pracset
(+/-) improvements to the loadbar + loadicon (@Lund1337)
(+) a lot of documentation (pracman/pracman2)
(+) specific commands manual => praccmd_help
(+) praccolor + advanced color customization for the GUI
(+) pracwh
(+) pracsmokehide
(+) pracpov
(+) practpose
(+) pracpitch
(+) prachud
(+) pracvm
(...) probably forgot about something...
