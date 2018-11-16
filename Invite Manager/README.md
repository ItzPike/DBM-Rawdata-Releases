# Invite Manager

## Version
Version 1.2

Updates
Fixed command **invitelk** command's check command parameter jumping to a non-existant action

## Information
This is an invite manager that keeps track of an player's invites
This also keeps tracks of how many players a user has invited
A new function is getting what invite code/link a playeru used to join the server

Remember, this pulls from a list of ACTIVE invites so if an invite expired, it wouldn't show.

To use these commands, please make sure you have the npm module **"array-sort"**

If you want to change how many people are shown on the leaderboard at once, go to the invitetop run script and change the 10 in "let maxLeaderboardSpots = 10;" to whatever number of people you want to be displayed on the leaderboard.

If you have any suggestions, or problems, open an issue on this github


## Commands
inviteinfo [@player] or !inviteinfo - To check a player's invites 
inviteclear - Clear a player's invites (Requires manage server permission to use)
invitetop - Players with the most invites
invitelk [invite code/invite link] - Gives information about the invite
playerinvite [@player] - Shows what invite the player used to join the server

## Events
These events that are **REQUIRED** for the **playerinvite** command to work

storeInvites - Store invites for all servers
serverJoin - Stores the invites for the server
memberJoin - Stores which invite the member used to join

## Folders
Commands are seperated by folder
Commands/Events are seperated in their own folders


