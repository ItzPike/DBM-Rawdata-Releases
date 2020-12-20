[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
# ⚠️ Important ⚠️
**Please contact me (Pike#6424) on discord or open up an issue if you experience any issues!**
  
This command set needs new intents to function!
The intents needed are as follows:
- **Server Events**  
- **Server Member Events**   
- **Both server Message Events** 

You **need to enable them** on the **intents settings** under extension in the DBM software and on the **developer panel** directly!
  
These commands were all tested inside the windows command line and not ran within DBM  

**All** events are required usually for the system to work!
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
# 📇  Role Reaction Menu 📇
Version 1.5.1 - QoL Changes + Role Menu on Old Messages + Bug Fixes
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## 📝Information📝
This is the role reaction menu system. Using this set of commands and events, every server can set up their own embeds with users being able to react with emojis to receive a certain role. The setup command (rolemenu) gives the user a clear prompt and a way to set up the menu. 

Many checks are in place to check the format of what the users put in and will warn them if any errors are detected. If roles are deleted or are missing, the system can detect this and would remove that prompt.

This menu allows servers to set up say color roles in any way they want and users can freely react and unreact to recieve and remove those roles. It is pretty straight forward and easy to use.

Any questions can be directly towards me (Pike#6424) or an issue can be opened on this Github.

As a guide through the role menu prompt, it would first ask you to set the title and descripton of the embed that is going to be created.

After that and you typing **confirm**, it would proceed you to the next step where you can add in the roles and emoji individually.

Currently, you can provide the name of the role, the id, or even just mention it directly. The format is strictly **role emoji**.

For example, if I wanted to assign the emoji 😃 to the role exampleRole, I would have to type the following:
**exampleRole 😃**
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Commands
- rolemenu (Prompts you with a prompt to go through to add differnt roles and emoijs)
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Events
- reactionStart - Intilizes a file stored in /data folder to store information about the role menus. It also handles the reactions and is responsible for giving the users the roles.
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Changelog
**Changelog (1.4)**
- Removed some excess functions and code, simplifying it  
- Support for roles with spaces in their name when not tagging it  
- Removed format prompt question to avoid further confusion  
- Added title and description customization prompt questions  
- Added debug mode for rolemenu command  
  
**Changelog (1.4.1)**
- Simplified parts of the code increasing effiency and shortening it in the process  
- Added bold text formatting to highlight what the prompt expects  
- Threw error catches into a function thus cleaning up some clutter with the code    
   
**Changelog (1.4.2)**
- Simplified asking prompts into functions shortening the code massively
- Made "prompt cancelled" prompts more clear, stating if it was by user request or some other reason  
   
**Changelog (1.4.3)**  
- v12 Fixes that cuase major issues  
- Reduced load and requests to the api  
  
**Changelog (1.4.4)**
- Reduced API calls to the API (Use more cache) 
- Prevent adding roles that position is higher than the bot (does not allow bot to add role) in role menu  
- Added bot perimssion check on rolemenu to make sure the bot can even add roles  
- Added safety-nets in place when reacting and sending an error message to console and player to notify them of either the lack of permissions causing the inability to add roles.  

**Changelog (1.4.5)**
- Fixed allowance of foramtting error causing the menu to bug (emoji first and then mention role)  
- Final menu has mentions instead of just text now (style changes)  
  
**Changelog (1.4.6)**  
- Fixed the menu not recognizing ids and role names   
  
**Changelog (1.4.6.1)**  
- Missing intents notifier  
  
**Changelog (1.4.6.2)**  
- Moved data files to individual folders  
  
**Changelog (1.5)**  
- New NPM module check/install for those who don't have the request module and some new ones required by the system  
- Steno file write allowing for more safety in writing files; hopefully less failures  
- Allow existing messages to be role menued  
- Auto cleanup of reactionRole data file when reaction menus are deleted  
- Small minor instruction syntax fixes  
- Reduce load to API and use cache instead of fetch  
  
**Changelog (1.5.1)**  
- Fixed file/folder not being created  
- Fixed path issues for Linux and Windows (hopefully)
  
