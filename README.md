# Create Discord Bot

Create Discord bots using a simple widget-based framework.

## Bot Setup

### Create Bot

1. Go to Discord's [Developer Portal](https://discordapp.com/developers/applications/).
2. Create a new application.
3. Add a bot user to your app.
4. Invite your bot to a server using: [https://discordapp.com/oauth2/authorize?scope=bot&client_id=COPY_PASTE_YOUR_DISCORD_BOT_CLIENT_ID_HERE](https://discordapp.com/oauth2/authorize?scope=bot&client_id=COPY_PASTE_YOUR_DISCORD_BOT_CLIENT_ID_HERE)

> A Discord bot's client ID is not the same as the bot's token!

5. `Click to Reveal Token` to view your bot token, you will need this in the next section.

> Keep this token and any file containing it **private**! If your token ever leaks or you suspect it may have leaked, simply `regenerate` a new token to invalidate your old token.

### Get Bot

1. Download the project: `git clone https://github.com/peterthehan/create-discord-bot.git`
2. Navigate into the project: `cd create-discord-bot/`
3. Install project dependencies: `npm install`
4. Rename [example.token.json](https://github.com/peterthehan/create-discord-bot/blob/master/example.token.json) to `token.json`.
5. Open the file and add the bot token found in the previous section:

```js
{
  "TOKEN": "COPY_PASTE_YOUR_DISCORD_BOT_TOKEN_HERE"
}
```

### Run Bot

1. Start the bot: `npm start`

> The bot should go from offline to online. Verify the bot is working by using the `ping` command.

> The default command prefix is `.`. You can configure the `command` widget's settings in [src/widgets/command/config.js](https://github.com/peterthehan/create-discord-bot/blob/master/src/widgets/command/config.js).

🎉 You're ready to create your own widgets! 🎉

## Widgets Setup

### Design

`create-discord-bot` comes with a [command](https://github.com/peterthehan/create-discord-bot/blob/master/src/widgets/command/) widget. Simply follow the design of the `ping` command to start building your own commands.

Widgets **must** live under the [src/widgets](https://github.com/peterthehan/create-discord-bot/blob/master/src/widgets/) folder and each widget **must** have a `handlers` folder.

For example:

```
widgets
├───widgetProject1
│   ├───handlers
|   |   ├───eventHandler1.js*
|   |   ├───eventHandler2.js
|   |   └───etc
├───widgetProject2
│   ├───handlers
|   |   ├───eventHandler1.js
|   |   ├───eventHandler2.js
|   |   └───etc
```

> \*: All event handler files must be named exactly the same as the event emitted found on the [Client](https://discord.js.org/#/docs/main/master/class/Client) page.

### Examples

The following widgets have been made using this framework:

- https://github.com/peterthehan/discord-active-role-bot
- https://github.com/peterthehan/discord-audit-log-bot
- https://github.com/peterthehan/discord-birthday-role-bot
- https://github.com/peterthehan/discord-emoji-log-bot
- https://github.com/peterthehan/discord-reaction-role-bot
- https://github.com/peterthehan/discord-region-role-bot

Visit for more help or information!

<a href="https://discord.gg/WjEFnzC">
  <img src="https://discordapp.com/api/guilds/258167954913361930/embed.png?style=banner2" title="Discord Server"/>
</a>
