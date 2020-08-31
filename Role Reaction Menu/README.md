# New Setup Step (IMPORTANT)
Due to the recent Discord API update, this command set will now require a few intents  
They are  
- Server Events  
- Server Member Events   
- Both server Message Events  
  
Make sure to have these enabled in your developer portal and intents under the extensions tab of your DBM software.

# Warning
Old files from version 1 will not be compatible with version 1.1 due to strucuturing overhauls.  
All role menus from version 1 will no longer work with the set of new events  
   
# Role Reaction Menu
- Version 1.4.5  
  
## Information
This is the reaction role command.  
This command allows you to create a reaction menu where a player can react to get a specfic role.  
Many built in failsafes, including one to shutdown the embed when the role is invalid/removed are also built in.  
If you have any suggestions or issues, feel free to contact me or open an issue on this github  

## Commands
- rolemenu (Prompts you with a prompt to go through to add differnt roles and emoijs)

## Events
These events that are **REQUIRED** for the command to work

- reactionStart - Intilizes a file stored in /data folder to store information about the role menus, handles reaction add + remove
  
## Warning
These commands were all tested inside the windows command line and not ran within DBM  

## Settings
- In the reactionGet and reactionRev scripts, you can edit what the bot sends to the players when they add/remove a reaction/role.
- In the same part you can enable/disable if the bot dms the user at all.  
- In setuptch you can enable/disable if multiple channels can be set per server.  
- In rolemenu you can set how many max roles to reactions in embeds you can have.  
- In rolemenu you can set debug mode to true to print all errors that occur with await messages including it running out of time.

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders

## Changelog
- Version 1.4 - Cleanup + Further Simplification   
- Version 1.4.1 - Code cleanup with some visual changes  
- Version 1.4.2 - Further code cleanup + simplification  
- Version 1.4.3 - Minor fixes and updated setup  
- Version 1.4.4 - Reduced API load and added more failsafes to prevent erroring  
- Version 1.4.5 - Fixed small bug and style changes  
  
Changelog (1.4)
- Removed some excess functions and code, simplifying it  
- Support for roles with spaces in their name when not tagging it  
- Removed format prompt question to avoid further confusion  
- Added title and description customization prompt questions  
- Added debug mode for rolemenu command  
  
Changelog (1.4.1)  
- Simplified parts of the code increasing effiency and shortening it in the process  
- Added bold text formatting to highlight what the prompt expects  
- Threw error catches into a function thus cleaning up some clutter with the code    
   
Changelog (1.4.2)
- Simplified asking prompts into functions shortening the code massively
- Made "prompt cancelled" prompts more clear, stating if it was by user request or some other reason  
   
Changelog (1.4.3)  
- v12 Fixes that cuase major issues  
- Reduced load and requests to the api  
  
Changelog (1.4.4)
- Reduced API calls to the API (Use more cache) 
- Prevent adding roles that position is higher than the bot (does not allow bot to add role) in role menu  
- Added bot perimssion check on rolemenu to make sure the bot can even add roles  
- Added safety-nets in place when reacting and sending an error message to console and player to notify them of either the lack of permissions causing the inability to add roles.  

Changelog (1.4.5)
- Fixed allowance of foramtting error causing the menu to bug (emoji first and then mention role)  
- Final menu has mentions instead of just text now (style changes)  