# Warning
Old files from version 1 will not be compatible with version 1.1 due to strucuturing overhauls.  
All role menus from version 1 will no longer work with the set of new events  
  
# Role Reaction Menu
Version 1.3 - Cleanup + Simlification

Changelog
- Removed two excess events and simplified everything under one event
- Added menus to work without doing the **setuptch** command
- Removed the setuptch command
- Added bolding to the two fields when sending messages after reacting.
  
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

## Example
[![Example](https://i.ibb.co/ccfCvHV/RDFa-Wnd-Oq-F-online-video-cutterco.gif)](http://s1.webmshare.com/ojN40.webm)
  
## Warning
These commands were all tested inside the windows command line and not ran within DBM  

## Settings
In the reactionGet and reactionRev scripts, you can edit what the bot sends to the players when they add/remove a reaction/role.
In the same part you can enable/disable if the bot dms the user at all.  
In setuptch you can enable/disable if multiple channels can be set per server.  
In rolemenu you can set how many max roles to reactions in embeds you can have.  

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders


