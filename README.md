#
## Installation Guide

- Have **node.js v16.6**. (To get on Replit, join this [Discord Server](https://dsc.gg/botsway))


- `node .` to Start The Bot.


- `npm start` for replit. (Run button)


- `npm install` to Install Packages/dependencies. 


- If your having `node:events` error then update your node version.   [Support Server](https://dsc.gg/botsway)


- If your using SlashCommands for your bot using this handler, Please make sure to **Invite your bot from discord.dev Oauth Section with `application.commands` scope**! ([Learn more](https://discordjs.guide/interactions/registering-slash-commands.html#guild-commands))


- Put Your Bot Token in `./botconfig/main.json` inside the clienttoken string. If your using replit, it's suggested to keep your token in env. So leave the string empty and make new secret inside Secrets, name it `clienttoken` and put your token inside it. Either you can go to `index.js` And Set It There (Not Recommended). 


- Go to `./botconfig/main.json` and set your  __ClientName__ (Bot Name), __ClientID__ (Bot ID), Most importantly the **TestingServerID** (The bot's support/test server where it will load slash commands), and the **Prefix** (Default: *?*). 


- When Setting up `./botconfig/main.json`, Also Set The 
**DeveloperIDs** (Bot Owners), **clientavatar** (Bot's PFP Link For Embeds), **randomMessages_Cooldown** (Messages For Cooldown Like Dank Memer). Not necessary.


- Also Set Your Bot's Status In `./events/ready.js`


- Note : You have to make folders in `lowercase` to use the help command otherwise it will throw errors.
#
## Features

- **Aliases**, **Cooldowns**, **Descriptions**, **Usages** And More Systems.
- **ToggleOff** CMD System (*If your command is bugged or in beta, it's a good suggestion to keep it "Un-usable" for the users.*)
- **DevelopersOnly** System (*You should use this for commands like eval etc. It makes it "Un-usable" for the users, but not for the developers of the bot.*)
- **Sub-Folders** (*Make as many folders as you want, just keep it clean `;)`*) 
- **Dynamic Help Command** With Menus [*Works With Reload CMD /Sub-Folders Aswell*] (*To use it, please read a little below for the guide...*) 
- **Command help** (*Tells Information About Command*)
- **Reload Command** (*Inside Sub-folders aswell*)
- **Anti-Crash** System (*Doesn't let your bot crash...*)
- **Event Handler**
- **Permission Handler** (*Manages user-perms and bot-perms for cmds.*)
- **Slash Command Handler** (*Manage Slash Commands*)
- **OP Ready Message** (*When your bot is ready, it pops up some information/statistics about it on the console...)*
- **Eval Command** (*For Evaluating Some Code*)
- **Buttons**, **SelectMenus**, **ContextMenus** Handling
- And Much More...

#
## More Information
- Use command template from `command-template.js` file for making new commands!
- `command-format.js` file is for explanation of the template.
- If you do not fill the stuff in `./botconfig/main.json`, you'll get some errors. Please put your testing server id and client token to fix it.
- if you do not mention the folders for help command it will throw an error!
- Make your code look clean using [prettier.io](https://prettier.io/)
- If you want your **Slash Commands** to be global then just change line 74 in `./handler/index.js` to 
```javascript
await client.application.commands.set(arrayOfSlashCommands)
```
