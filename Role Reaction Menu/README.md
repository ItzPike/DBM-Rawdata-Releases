# Warning
Old files from version 1 will not be compatible with version 1.1 due to strucuturing overhauls.  
All role menus from version 1 will no longer work with the set of new events  
  
# Role Reaction Menu
Version 1.1 - Performance + Structuring Overhaul

Changelog
- Optimized storing of reaction roles, removing some unnececary data
- Moved data storage to a whole seperate file
- Switched to raw JSON storage, no text for easier diagnosis and preventing any major parsing issues
- Assigned player reaciton list per emoji, fixing many unreaction issues
- Every message is now a JSON object and is now not in an list, to further increase performance removing the need to loop through items
- Fixed 4th item not working at all due to player list overwriting important information
- Removed rate limit as it causes issues if bot goes down, user will never be allowed to recieve a role from a reaction menu again   
  
Upcoming Plans  
- None at the moment, feel free to dm me Pike#0001 for any suggestions!
  
## Information
This is the reaction role command.  
This command allows you to create a reaction menu where a player can react to get a specfic role.  
Many built in failsafes, including one to shutdown the embed when the role is invalid/removed are also built in.  
If you have any suggestions or issues, feel free to contact me or open an issue on this github  

## Commands
- rolemenu (Prompts you with a prompt to go through to add differnt roles and emoijs)
- setuptch (Sets the channel mentioned to an update channel. This means the reaction roles in this channel will stay alive after a restart. This is set per server.)

## Events
These events that are **REQUIRED** for the command to work

- reactionGet - Stores and checks the reaction, adding a role if reacted on a menu
- reactionRev - Stores and checks the reaction, removing a role if reacted on a menu
- reactionStart - Intilizes a file stored in /data folder to store information about the role menus, used by other commands
  
## Warning
These commands were all tested inside the windows command line and not ran within DBM  

## Settings
In the reactionGet and reactionRev scripts, you can edit what the bot sends to the players when they add/remove a reaction/role.
In the same part you can enable/disable if the bot dms the user at all.

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders


