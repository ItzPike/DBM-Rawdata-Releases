# Deathbattle 
Version 1.1 - File failsafe fixes

## Information
This is an Deathbattle system that allows users to "fight" each other using bot narrated events  
Each attack/event can be customized, removed, added, etc.  
Each attack does a specfic amount of damage    
This command also allows you to restore the default actionPossibilities.json file which is the file that manages all possible acitons/events that happen in a battle

Remember to drag the components in the resources folder to the bot resource folder!  
Do not drag the resources folder itself but the things inside it  

## Commands
- deathbsettings help - Displays this help message with command information and usage  
- deathbsettings add - Starts a prompt where you can add your own events/actions onto the current deathbattle events/actions  
- peathbsettings list - Displays a lsit of deathbattle events/actions  
- deathbsettings remove {event/action} - Removes a certain action from the deathbattle events/actions  
- deathbsettings info [action/event] - Shows info for provided action/event  

- deathbattle [@player] || deathbattle [@player] [@player]  

- deathbattlerestore - Brings up a prompt to restore default files that are needed to run the command  

## Events
- deathBattleCheck - Check all files on startup that are needed for the commands to work properly and if the check fails it will disable all deathbattle commands
- deathBattleCheck|Interval - Check all files on an interval that are needed for the commands to work properly and if the check fails it will disable all deathbattle commands

## Warning
These commands were all tested inside the windows command line and not ran within DBM  
These commands may not work while being ran within DBM, so just be advised

My Node Version - v10.9.0   
My NPM Version - v6.2.0  

## Required Modules
Jimp (npm i jimp)  
Execute `npm i jimp` from the command line that is inside your bot directory  

File System (npm i fs)
Execute `npm i fs` from the command line that is inside your bot directory

Request (npm i request)
Execute `npm i request` from the command line that is inside your bot directory

## Folders
(O) Commands are separated by folder   
(O) Events are separated in their own folders  
(O) Resources are separated in ther own folders  

## Issues
Please if you have any issues open up an issue on this github and I will help/respond as soon as possible.  
If you would like to DM directly for anything, go ahead!  

## Progress
Project started - 12/26/18  
Finishing Date - 1/5/19  
Testing Phase - 1/5/19 | Status: ~ In Progress ~ 9:24PM EST  
(Update) Testing Phase - 1/6/19 | Status: Finished 2:25AM EST  
  
Secondary Testing - 1/6/19 | Status: ~ In Progress ~ 2:26 AM EST | Update Status: Cancelled 

## Preview
https://rem-best-girl.anime-chan.xyz/u/21.04.24-06.01.19.mp4

