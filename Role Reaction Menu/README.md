# Warning
Old files from version 1 will not be compatible with version 1.1 due to strucuturing overhauls.  
All role menus from version 1 will no longer work with the set of new events  
  
# Role Reaction Menu
- Version 1.4 - Cleanup + Further Simplification  
- Version 1.4.1 - Code cleanup with some visual changes
- Version 1.4.2 - Further code cleanup + simplification

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
  
Upcoming Plans  
- None at the moment, feel free to dm me Pike#3369 for any suggestions!
  
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


