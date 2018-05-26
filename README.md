# ChatDefender-Release-Command-Documentation

# About ChatDefender
ChatDefender has been long coded since the summer of 2017. *There is no set date for it*<br>
ChatDefender is a high-end chat moderation bot. This bot goes from command logging to timers. All commands are stored in seperate files for great organization. The permissions for commands are customizeable, except for a few due to abuse or just should not be in the wrong hands of others. You will see an error that says "so and so cannot be changed". Due to many people being confused as to how things work, I have made this guide that shows how a command should be used alongside all options of it. They are in order as `Manager, Staff, and User` with a little description about each of them.

> Note: These are examples on how to use the commands. There are a few restrictions and I will note them.

# Manager
Command Name | Description | Usages
-------------|-------------|-------
allowbypass | Allows uses with roles or messages in channels to bypass the filters. | allowbypass swear channel add #general<br>allowbypass swear channel remove #general<br>allowbypass link channel add #general<br>allowbypass link channel remove #general<br>allowbypass link role add @role<br>allowbypass link role remove @role<br>allowbypass link channel add #general<br>allowbypass link channel remove #general
blacklist | Adds words that are not allowed to be said, like shit | blacklist add shite<br>blacklist remove shite<br>blacklist show
command | Adds, Removes, Disables, and Enables commands | command add Hello Hello everyone!<br>command remove Hello<br>command disable 8ball<br>command enable 8ball<br>command disable 8ball -c #general (Restricts the command to only be used in that channel)<br>command enable 8ball -c #general<br>command disable 8ball -r @role (Restricts the command to uses who do not have that role)
config | One of the most important commands. This configures the bot within the discord client. No website needed! | config [option] [add/remove (only for staff roles)] [new value]
perms | Another important command. This allows you to configure permissions amoungst commands | perms [command] [value 1-3]
sendMessage | Sends a message in a specified channel. | sendMessage #general Hey all! This is just a test message.
timer | A command that adds a timer. This command sends a message in a specified channel with a given interval | timer add thisisatimer #general 30m This is totally not a timer

# Staff 
Command Name | Description | Usages
-------------|-------------|-------
ban | Bans a user for a specified amount of time | ban @user 15m Take a timeout<br>ban 123456789123456789 0 Malicious Intent
cc | Clears a specified amount of messages, even filtered through ID or Mention | cc @user 50<br>cc 123456789123456789 100<br>cc 100
kick | Kicks a mentioned user with a reason | kick @user You annoy me<br>kick 123456789123456789 you talk too much
mute | Mutes a mentioned user for a specified amount of time | mute @user 15m Spamming<br>mute @user 0 Too many punishments
punishments | A command to check punishments, either staff or user or all, and delete if needed | punishments search staff @user<br>punishments search staff 123456789123456789<br>punishments search user @user<br>punishments search user 123456789123456789<br>punishments search all<br>punishments delete [PunishmentID - obtained from the search]
unban | unbans a user with a provided ID | unban 123456789123456789 Appealed
unmute | Unmutes a mentioned user | unmute @user Appealed
warn | Warns a user. They must acknowledge it in the bot DMs, given the mute role until acknowledged | warn @user Spamming

# User
Command Name | Description | Usages
-------------|-------------|-------
8ball | Answers with a randomized response | 8ball Do you love me?
botinfo | Gives information about the bot | botinfo
give | gives a user a role, if you have `Manage Server` perm, you can add or remove from the database | give add @role<br>give remove @role<br>give rolename
help | Shows all available commands for a user | help
permlvl | Shows the user thier perm lvl | permlvl
take | Removes a role from a user, as long as it is in the database | take rolename
uptime | Shows the bot's uptime | uptime
userinfo | Shows user info, if no user is present, itll show the author's user information | userinfo<br>userinfo @user<br>userinfo 123456789123456789

