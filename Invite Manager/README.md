[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
# ⚠️ Important ⚠️
**Please contact me (Pike#6424) on discord or open up an issue if you experience any issues!**
  
This command set needs new intents to function!
The intents needed are as follows:
- **Server invite events**
- **Server member events**

You **need to enable them** on the **intents settings** under extension in the DBM software and on the **developer panel** directly!
  
These commands were all tested inside the windows command line and not ran within DBM  

**All** events are required usually for the system to work!
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)

# ✉️  Invite Manager Rewritten ✉️
Version 1.2.1.4 - Syntax fixes  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## 📝Information📝
This is the newly rewirtten Invite Manager. This system allows you to quickly manage invites through a series of commands. On user join, the system would quickly log down what invite the user joined with and who invited them.

Using this data, the invite manager can use this data in a variety of commands like `inviteinfo`. `inviteinfo` allows one to view who used what invit and the information on that invite. Currently, only non-expired invites can be looked up. This may change very soon.

The invite manager can also quickly construct a profile of a user including who they invited recently, and what invite they used.

Do note however that this only logs the joins of invites that users used after the system has been added and the bot is online. If it is offline, it cannot log this data.

If you have any questions or issues, feel free to contact me (Pike#6424) in Discord or open up an issue on this Github!
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Commands
- invitesettings - Brings up a settings menu where the user can quickly change the settings of the invite manager  

- invitetop - Brings up the leaderboard with the top 10 users who have invited the most users  

- inviteinfo [inviteURL or inviteLink] - Fetches the invite information and shows who has joined using said invite along with who created the invite  

- inviteplayer [username or @User] - Show a users invite profile with the people they invited recently  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Events
- inviteStart - One event that sets up all major systems that are required for the commands to work
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)

## API
These api functions can be ran inside of run scripts in anywhere. The main goal of thsee new functions are that any normal command developer can interact with the data of the invite manager. This allows more flexibility and wont require me to release many pieces of smaller commands.

If you call a function and the operation fails, it will return with "failed" along with the reason seperated by a -. | Example: `failed - No data found`

If you call a function and the function succeeds, it will return with the data or "success" if the change had went through. 

These functions can be ran inside of control variables through putting the function in the value section inside of a dollar sign and two opening and closing brackets (${}).  
  
```js
Actions.inviteGet(userIDHere, guildIDHere, invalidReal) 
```
  
This grabs the user data and returns it. The "invalidReal" variable here needs to be either 1 for real and 0 for invalid.  

Invalid and real here refers to the virtual counter of "real" invites and the virtual coutner of invalid invites.  
  
Example: 
```js 
Actions.inviteGet(msg.author.id, msg.guild.id, 1)
```
The above example gets the amount of "real" invites from the command author in the server the command is executed in.
  
```js 
Actions.inviteModifyData(userIDHere, guildIDHere, valueChange, invalidReal)
```
  
The above function call modifies the virtual counter of the "real" and "invalid" invites. The "invalidReal" variable here needs to be either 1 for real and 0 for invalid.  
  
The value change can be any integer and it will modify it by that integer.   
For example, if valueChange was 1, it would add 1 to either real/invalid depending on the invalidReal variable.   

Having the integer -1 will subtact 1 to either real/invalid depending on the invalidReal  
  
Example:
```js
Actions.inviteModifyData(msg.author.id, msg.guild.id, 1, 1)
```
The above function call adds 1 "real" invite to the command author in the server the command is executed in.  
  
- Example commands   
Coming soon!  

[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Changelog
**Version 1** - Intial Release  
   
**Verison 1.1** **(Credits to NiceATC#1337(213692669443047424) for the original formatting concept)**  
- Event formatting redone to make it look less bland including now the inviter's valid invites  
- Settings default format is changed to have a paragraph break to make the uses readable and not cut off 
  
**Version 1.1.1**  
- Fixed invitetop not ordering players correctly
  
**Version 1.2**  
- Add check to prevent errors from occuring if bot is missing permission to fetch invites  
- Added scrollable pages to inviteplayer and inviteinfo if the list is too long  
- Fixed inviteplayer not being able to use user id  
- Support for expired invites  
- New converter that converts the old invite data format to the new invite data format  
- Display tags next to the users dispalyed in inviteplayer and inviteinfo data in case the user is not cached on the user side causing <@id> to appear  
- Redone embed formats adding unicode to inviteplayer and inviteinfo  
- Allow the system to work after a bot reload (needs a full restart first)  
  
**Version 1.2.1**  
- Try catch for event + settings (Hopefully reduces errors in chat) when checking properties  
  
**Version 1.2.1.1**  
- Missing intents notifier  
  
**Version 1.2.1.2**  
- Moved data to its own folder to organize  
- Vanity URL support? (Not tested yet)  
- Using multiple {user1}/{user2}/{code}/{uses} in template now works  
  
**Version 1.2.1.3**  
- Fixed issue when the API accepts strings  
  
**Version 1.2.1.4**
- Fixed small syntax error for API  
  
**Version 1.2.1.5**
- inviteinfo erroring with newly created unused codes
  
**Version 1.2.2 (Planned)**  
- Add toggleable settings to enabled/disable the embed message in favour a simple message.  
- Filter users who had left out of invitetop  
