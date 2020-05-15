## Warning
Please note that this new system will have a slight delay of 10-15 seconds of drawing a winner.  
This is due to the fact that every 10 seconds the event checks for giveaways that needs to be drawn and draws each one with a second interval in between to not flood the Discord api.
When the amount of total giveaways grow, this delay may increase depending on when the giveaways are set to end.

# Giveaway Rewritten
Version 1 - Release

Changelog
- Redone the entire command for a system that works after restart
- Moved to an giveaway ID based system attached to servers
- Giveaway command setup moved to a embed  
- Added in gdraw and gend  
  
Upcoming Plans  
- None at the moment, feel free to dm me Pike#3369 for any suggestions!
  
## Information
This is a giveaway command rewritten from the original version improving many aspects of it.  
With this, it allows users to setup giveaways with timers that automatically end and draw winners that react using an emoji.  

## Commands
- gcreate - Startup the setup giveaway prompt    
- gdraw [#number of winners] [giveaway message id (optional)] - To be executed in the same channel as giveaways; grabs the latest giveaway (or selected giveaway) and draws selected amount of winners from it. (**Note: Giveaway has to have ended**)
- gend [giveaway embed id] - Ends a giveaway early and draws preset amount of winners  
- gstart [item] [time] [# of winners (optional)] - Starts a quick giveaway in one command with only needing a item and a time

## Settings
- In gcreate, there is a timezone setting that you can change on the first few lines. (Takes timezone abbreviations)  
- For above setting for timezones, refer to database [here](https://gist.github.com/aviflax/a4093965be1cd008f172)

## Events
These events that are **REQUIRED** for the command to work
- giveawayStart - Creates and checks for required files on startup  
- giveawayCheck - Searches for giveaways that ended and draws a winner from them
  
## Warning
These commands were all tested inside the windows command line and not ran within DBM  

## Folders
(O) Commands are separated by folder  
(O) Commands/Events are separated in their own folders


