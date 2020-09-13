[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
# 📇 Captcha Join 📇
Version 1.2 - Changelog below  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
## ⚠️ Important ⚠️
**Please contact me (Pike#6424) on discord or open up an issue if you experience any issues!**
  
Needs **Server Member Events** intent for the event to work.
  
These commands were all tested inside the windows command line and not ran within DBM  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## 📝Information📝
This is a captcha event + command that allows on a per server basis to setup join captchas for their members! The captchas are sent to the users (image) that is fetched directly from an api. When the user replies the correct captcha, it gives them the set role or no role depending on how the roles are set up per server.
   
Every server has the option to select a role through the setrole command. This command allows then to input a mentioned role, role id, role name. Any of these will give the user on join these roles. 
   
In special cases where the setrole is set to 0, the captcha system would be disabled completely.

In special cases where the setrole is set to 1, the captcha system would be enabled but would give no role.

The captcha currently does not work after restart and the user must rejoin to get the captcha again. It is a await response and thus would not be able to handle such thing.

By default, the user gets three attempts at the captcha. If the user fails all three, they would be automatically kicked. If the user times out, it would also use up those attempts. 

Captchas are generated via the api and stored locally in the captchas folder. On each bot start, all the files that are .png in the captchas folder are deleted to save space.
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Commands
- setrole (Starts a prompt asking you for the role)  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Events
- CaptchaStart - Ran on bot intilaization to start the event and check for updates  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
  
## Changelog
**Version 1** - Initial Release  
  
**Version 1.1**  
- Put all created captcha in new folder  
- Clear captcha folder on start (only .png affected for safety reasons)  
  
**Version 1.2**  
- Allow adding of multiple roles to the captcha command (only for if responding by id or mention)  
- setrole prompt now warns of not mixing mentions and ids  
- setrole now also shows info about the new feature allowing for multiple roles  
  
**Version 1.2.1**   
- Missing intents notifier  
  
**Version 1.2.2**  
- Allow spaces inbetween captcha letters to avoid confusion for users  
  
[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png)](#Important)
