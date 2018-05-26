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
