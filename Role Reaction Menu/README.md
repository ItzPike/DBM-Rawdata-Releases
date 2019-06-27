# Role Reaction Menu
Version 1 - Initial Release

## Information
This is the reaction role command.  
This command allows you to create a reaction menu where a player can react to get a specfic role.  
Many built in failsafes, including one to shutdown the embed when the role is invalid/removed are also built in.  
If you have any suggestions or issues, feel free to contact me or open an issue on this github  

## Commands
- autorole (Prompts you with a prompt to go through to add differnt roles and emoijs)
- setuptch (Sets the channel mentioned to an update channel. This means the reaction roles in this channel will stay alive after a restart. This is set per server.)

## Events
These events that are **REQUIRED** for the command to work

- reactionGet - Stores and checks the reaction, adding a role if reacted on a menu
- reactionRev - Stores and checks the reaction, removing a role if reacted on a menu
- reactionStart - Intilizes an arary for data to be stored upon by autrole and is used by reactionGet

## Warning
These commands were all tested inside the windows command line and not ran within DBM  
Thanks to Akira#1234, it does seem to be workin from within DBM (horray)

## Settings
In the reactionGet and reactionRev scripts, you can edit what the bot sends to the players when they add/remove a reaction/role.
In the same part you can enable/disable if the bot dms the user at all.

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders


