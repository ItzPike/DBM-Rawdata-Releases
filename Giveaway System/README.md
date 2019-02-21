# Giveaway System

## Version
Version 1.2 - Non-beta user fix

## Information
This is new giveaway system with the latest await response  
There is only 1 command, and that is to setup the giveaway  
It will loop you through prompts that ask you for information and it'll setup the giveaway for you  
You will respond with the information it asks you  

First, it'll ask for you what you are giving away  
Secondly, it'll ask you for how many winners you want (As many as you want)  
Then, it'll ask you for how long the giveaway will last in days/hours/minutes [1d,5m,3h, etc.]  
After that, I'll ask you for what channel you want the giveaway to be hosted in  

There is a failsafe along the setup to make sure you did it correctly  
Make sure you use this command in a chat where there are little to no chatting at all  

The command will "timeout" after 20 messages that are sent in the channel or 20 seconds to prevent any API spam and issues seeing the prompt itself

This system **WILL** check if the message is sent by the command author for the await responses  
You need the **Manage Messages** permission to use the gcreate command unless changed  
If you have any suggestions or issues, feel free to contact me or open an issue on this github  

Also, please do not contact me for a giveaway end command, I am looking into it already

## Commands
 - gcreate

## Folders
(O) Commands are seperated by folder  
(O) Commands/Events are seperated in their own folders  

## Problems | Q/A

Q: DBM Errors out whenever I try to run the command  
A: Try running the command with the command line, node bot.js instead of running it from within DBM

Q: Client is not defined  
A: Make sure you have DBM Beta installed/on  


