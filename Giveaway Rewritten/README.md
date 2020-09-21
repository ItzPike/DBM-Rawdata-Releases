[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
# ⚠️ Important ⚠️
**Please contact me (Pike#6424) on discord or open up an issue if you experience any issues!**
  
These commands were all tested inside the windows command line and not ran within DBM  

**All** of the events are usually required for this sytem to work!
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
# 🎉  Giveaway Rewirtten 🎉
Version 1.3 - Changelog below
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## 📝Information📝
This is a giveaway system and here are provided all the commands and events needed to have a giveaway bot. Giveaways can be easily created through the prompt through gcreate and winners would be fetched at the ened of the giveaway.

Other ways to start a giveaway prompt would be through gstart with the provided parameters as listed below.

These giveaways may be ended at max a 10 second delay due to how the event would check what giveaways have ended.

Giveaways can be ended early or redrawn from.

The **gend** command which ends the giveaway early can only work on giveaways that are in progress. It uses the **giveaway ID** at the bottom of the giveaway embed.

The **gdraw** command which redraws winners from the last giveaway embed can only work on giveaways that have ended. It uses the giveaway **message ID** which can be gotten from right clicking a message and clicking Copy ID if you have developer mode enabled.

If you have any questions, please report them to me (Pike#6424) on Discord or open up an issue on the Github!
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Commands
- gcreate - Startup the setup giveaway prompt    

- gdraw [#number of winners] [giveaway message id (optional)] - To be executed in the same channel as giveaways; grabs the latest giveaway (or selected giveaway) and draws selected amount of winners from it. 
(**Note: Giveaway has to have ended**)

- gend [giveaway embed id] - Ends a giveaway early and draws preset amount of winners  (**Note: Giveaway has to be in-progress**)

- gstart [# of winners (optional)] [time] [item] - Starts a quick giveaway in one command with only needing a item and a time
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Events
- giveawayStart - Creates and checks for required files on startup  

- giveawayCheck - Searches for giveaways that ended and draws a winner from them
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)

## Settings
Coming with this command set are multiple configurable settings at your disposal.

- In the **gcreate** script, there is a timezone setting that you can change on the first few lines. (Takes timezone abbreviations)  

- For above setting for timezones, refer to database [here](https://techsupport.osisoft.com/Documentation/PI-Web-API/help/topics/timezones/iana.html) (The string you put in is the IANA Time Zone Id (For example: "America/Sao_Paulo"))

- Do not modify anything other than the intended setting. That means nothing under **try{** as that serves as a purpose to reset the timezone to UTC if the timezone is invalid. Changing that defeats the whole purpose and can break the giveaway embeds

- In gcreate, there is a debug mode that would print all errors that may occur including when await message timers run out.

[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
# Changelog
**Changelog (v1.1)**
- Added fields displaying giveaway data
- Customizable description and title
- Added debug mode for gcreate  
  
**Changelog (v1.2)**
- Added awaitMessage functions shortening down the code massively
- Improved new debug messages
- Incorporate often used combination of functions into 1 function reducing the lines of code  

**Changelog (v1.3)**
- Fixed gdraw and gend  
- Improved code and fixed winner drawing issue (potential) (May of only drawn from the first 100 players)  
- Gave more clarity to which item someone won from gdraw and which message it came from  
- Fixed giveaway ending overwriting the intial title  
- Giveaway ending now supports the new embed layout  
- New field showing the status of the giveaway  
- Fixed gdraw filters for new format  
   
**Changelog (v1.3.1)**  
- Locally cache giveaway data  
- Removed reading of file from all commands to switch to cache system  
- Moved data folders to its own folder for organization purposes   
- Fixed the index when going through ending active giveaways getting added before the aciton is done  
