this is a super basic modified psych engine build meant specifically for recording nice looking videos of charts (like for [rips](https://youtu.be/3UCLI7tq7SQ) and stuff)

if you're looking for thumbnails, they're right [here](https://github.com/albert-softie/albab-s-cool-and-amazing-fnf-engine/tree/main/thumbnails)


## changes made:
 * removed the `BOTPLAY` text that normally appears while botplay is enabled
 * removed the miss count and rating % next to the score at the top so that it looks closer to vanilla fnf (and so that it doesn't always say `Rating: ?` at all times)
 * made it so that the score updates even while botplay is enabled
 * replaced the vanilla versions of bopeebo and fresh with the ost versions (because the ones in the vanilla game are early versions that suck)

## preview:
![psych test5](https://user-images.githubusercontent.com/13923537/134419590-4032b6a4-b7ff-4673-840f-a08825575196.gif)

#### bucket list of additions/changes which will probably never happen but y'know a guy can dream:
 * have botplay enabled by default when selcting a song (definitely the most possible out of all of these ~~or at least it would be if i knew what i was doing~~)
 * add in the week 7 checkboxes and note splash effects that were in early versions of psych engine but removed (for literally no other reason than fuck gamebanana)
 * ~~`week 7 (would be nice but more than likely not happening until week 7 comes to psych engine itself)`~~ ~~`(if that ever happens)`~~ 
     
     turns out shadowmario ported week 7 to psych as a mod. not sure if i'm allowed to post it here but it's in the basement club discord.

## disclaimer:
 * i am not a programmer. the most i can do is comment out lines and ask then people who know what they're doing why my changes break everything. so don't expect that many huge updates to this that aren't just updates to psych engine itself
 * would probably recommend against making any actual big boy mods with this. as stated above, this fork exists for the sole purpose of looking good in videos. if for whatever reason you were looking at this thinking you should make a mod using this engine, [og psych engine is right here.](https://github.com/ShadowMario/FNF-PsychEngine) besides it's not like i made any substantial changes to psych engine or anything like that (in fact as of writing this literally every change i made is in one file lmao)
 * if you do use this for videos, you don't *have* to give credit to me or link back here, but i wouldn't mind if you did
 * i used psych engine instead of something like kade engine because i like the little changes it makes to the vanilla game and also all the de-hardcoding stuff  ~~(and also kade engine botplay kinda sucks lmao)~~
 

special thanks to the people who actually made the engine that i more or less took a hacksaw to in order to make this, and also shoutouts to [noosh](https://www.youtube.com/channel/UCot9XXES2wpXePQ-s7O8T6g) for putting up with my code illiteracy and telling me how to make the game not break.


original readme below:
_____________________________________

# Friday Night Funkin' - Psych Engine
Engine originally used on [Mind Games Mod](https://gamebanana.com/mods/301107), intended to be a fix for the vanilla version's many issues while keeping the casual play aspect of it. Also aiming to be an easier alternative to newbie coders.

## Installation:
You must have [the most up-to-date version of Haxe](https://haxe.org/download/), seriously, stop using 4.1.5, it misses some stuff.

Follow a Friday Night Funkin' source code compilation tutorial, after this you will need to install LuaJIT.

To install LuaJIT do this: `haxelib install linc_luajit` on a Command prompt/PowerShell

...Or if you don't want your mod to be able to run .lua scripts, delete the "LUA_ALLOWED" line on Project.xml

## Credits:
* Shadow Mario - Coding
* RiverOaken - Arts and Animations
* bbpanzu - Assistant Coding

### Special Thanks
* shubs - New Input System
* SqirraRNG - Chart Editor's Sound Waveform base code
* iFlicky - Delay/Combo Menu Song Composer + Dialogue Sounds
* PolybiusProxy - .MP4 Loader Extension
* Keoiki - Note Splash Animations
* Smokey - Spritemap Texture Atlas support
_____________________________________

# Features

## Attractive animated dialogue boxes:

![](https://user-images.githubusercontent.com/44785097/127706669-71cd5cdb-5c2a-4ecc-871b-98a276ae8070.gif)


## Mod Support
* Probably one of the main points of this engine, you can code in .lua files outside of the source code, making your own weeks without even messing with the source!
* Comes with a Mod Organizing/Disabling Menu. 


## Atleast one change to every week:
### Week 1:
  * New Dad Left sing sprite 
  * Unused stage lights are now used
### Week 2:
  * Both BF and Skid & Pump does "Hey!" animations
  * Thunders does a quick light flash and zooms the camera in slightly
  * Added a quick transition/cutscene to Monster
### Week 3:
  * BF does "Hey!" during Philly Nice
  * Blammed has a cool new colors flash during that sick part of the song
### Week 4:
  * Better hair physics for Mom/Boyfriend (Maybe even slightly better than Week 7's :eyes:)
  * Henchmen die during all songs. Yeah :(
### Week 5:
  * Bottom Boppers and GF does "Hey!" animations during Cocoa and Eggnog
  * On Winter Horrorland, GF bops her head slower in some parts of the song.
### Week 6:
  * On Thorns, the HUD is hidden during the cutscene
  * Also there's the Background girls being spooky during the "Hey!" parts of the Instrumental

## Cool new Chart Editor changes and countless bug fixes
![](https://github.com/ShadowMario/FNF-PsychEngine/blob/main/docs/img/chart.png?raw=true)
* You can now chart "Event" notes, which are bookmarks that trigger specific actions that usually were hardcoded on the vanilla version of the game.
* Your song's BPM can now have decimal values
* You can manually adjust a Note's strum time if you're really going for milisecond precision
* You can change a note's type on the Editor, it comes with two example types:
  * Alt Animation: Forces an alt animation to play, useful for songs like Ugh/Stress
  * Hey: Forces a "Hey" animation instead of the base Sing animation, if Boyfriend hits this note, Girlfriend will do a "Hey!" too.

## Multiple editors to assist you in making your own Mod
![Screenshot_3](https://user-images.githubusercontent.com/44785097/144629914-1fe55999-2f18-4cc1-bc70-afe616d74ae5.png)
* Working both for Source code modding and Downloaded builds!

## Story mode menu rework:
![](https://i.imgur.com/UB2EKpV.png)
* Added a different BG to every song (less Tutorial)
* All menu characters are now in individual spritesheets, makes modding it easier.

## Credits menu
![Screenshot_1](https://user-images.githubusercontent.com/44785097/144632635-f263fb22-b879-4d6b-96d6-865e9562b907.png)
* You can add a head icon, name, description and a Redirect link for when the player presses Enter while the item is currently selected.

## Awards/Achievements
* The engine comes with 16 example achievements that you can mess with and learn how it works (Check Achievements.hx and search for "checkForAchievement" on PlayState.hx)

## Options menu:
* You can change Note colors, Delay and Combo Offset, Controls and Preferences there.
 * On Preferences you can toggle Downscroll, Middlescroll, Anti-Aliasing, Framerate, Low Quality, Note Splashes, Flashing Lights, etc.

## Other gameplay features:
* When the enemy hits a note, their strum note also glows.
* Lag doesn't impact the camera movement and player icon scaling anymore.
* Some stuff based on Week 7's changes has been put in (Background colors on Freeplay, Note splashes)
* You can reset your Score on Freeplay/Story Mode by pressing Reset button.
* You can listen to a song or adjust Scroll Speed/Damage taken/etc. on Freeplay by pressing Space.
