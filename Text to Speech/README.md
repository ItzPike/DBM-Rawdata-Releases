# Text to Speech 
Version 1.2 - Bug fixes and wait time changes

## Information
This is an easy and quick Text to Speech command  
This command takes user text input and then generates an speech mp3 file  
This is done under the raw data quest of Toepas#6190  

This command generates an MP3 file locally and sends it  
Right after it sends it, it'll delete it off the local drive to not clutter anything up  

## Commands
- tts [text] - Takes input of text and turns it into a mp3 speech file, sending it to the same channel
- ttsvc [text]- Takes input of text and turns it into a mp3 speech file, sending it to the same channel and then joining command author's vc to speak the message (The input has to have more than 47 characters)

## Warning
This API can only process text that are under 200 characters  
This for the free version of the google text to speech api of course  

This command was tested inside the windows command line and not ran within DBM    
This command may not work while being ran within DBM, just be advised  

My Node Version - v10.9.0   
My NPM Version - v6.2.0  

## Required Modules
Google Text to Speech API (npm i google-tts-api)  
Execute `npm i google-tts-api` from the command line that is inside your bot directory  

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
Project started - 1/6/19 (12:30 Afternoon EST)  
Testing Completed - 1/6/19 (1:21 PM EST)  

