## Warning
This system may not perform as well as it should in larger bots. This is not tested as of yet so I will have no idea what would happen. Any bugs or feedback would be much appreciated. Bugs can be opened up on github or DMed to Pike#6424.  
  
## Note
You may need two of the intents enabled:
- Server invite events  
- Server member events  
These may be needed for the bot to run properly.
  
## Invite Manager Rewritten
Version 1.1 - Event formatting update + default formatting update  
  
## Information
A entirely new rewritten system to keep track of who invited who and how many one has invited. This new system is completely redone to be more efficient and have a new API-like system to interact with the data. With this, currently you can get invite data from users and change those invite data. This allows anyone to create custom command-sets for this that aren't avaliable. New settings menu allow you to customize what channel to send user join notifications and even allow you to change the text foramt of the notification.

## Commands  
- invitesettings - Brings up a settings menu where the user can quickly change the settings of the invite manager  
- invitetop - Brings up the leaderboard with the top 10 users who have invited the most users  
- inviteinfo [inviteURL or inviteLink] - Fetches the invite information and shows who has joined using said invite along with who created the invite  
- inviteplayer [username or @User] - Show a user's invite profile with the people they invited recently  

## Events  
- inviteStart - One event that sets up all major systems that are required for the commands to work  
  
## Settings
- Logging Channel - Logs user join to a specified channel; can be enabled and disabled; will turn off if the channel is deleted or becomes invalid   
- Logging Format - The format of the messages sent to the logging channel/join channel; can be changed in the settings menu  
- Account age check - Checks the account age on join; will only count as a "real" invite in a virutal value if this was met  

## API
These api functions can be ran inside of run scripts in anywhere.  
If the operation fails, it will return with "failed" along with the reason seperated by a -. | Example: failed - No data found  
If the function succeeds, it will return with the data or "success" if the change had went through. 
These functions can be ran inside of control variables through putting the function in the value section inside of a dollar sign and two opening and closing brackets (${}).  
  
- Actions.inviteGet(userIDHere, guildIDHere, invalidReal)  
  
This grabs the user data and returns it. The "invalidReal" variable here needs to be either 1 for real and 0 for invalid.  
Invalid and real here refers to the virtual counter of "real" invites and the virtual coutner of invalid invites.  
  
Example: Actions.inviteGet(msg.user.id, msg.guild.id, 1) - Gets the amount of "real" invites from the command author in the server the command is executed in.
  
- Actions.inviteModifyData(userIDHere, guildIDHere, valueChange, invalidReal)  
  
This modifies the virtual counter of the "real" and "invalid" invites. The "invalidReal" variable here needs to be either 1 for real and 0 for invalid.  
  
The value change can be any integer and it will modify it by that integer.   
For example, if valueChange was 1, it would add 1 to either real/invalid depending on the invalidReal variable.   
Having the integer -1 will subtact 1 to either real/invalid depending on the invalidReal  
  
Example: Actions.inviteModifyData(msg.user.id, msg.guild.id, 1, 1) - Adds 1 "real" invite to the command author in the server the command is executed in.  
  
- Example commands   
Coming soon!  

### Changelog
Version 1 - Intial Release  
   
Verison 1.1  
- Event formatting redone to make it look less bland including now the inviter's valid invites  
- Settings default format is changed to have a paragraph break to make the uses readable and not cut off  

