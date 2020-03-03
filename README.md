# Create Discord Bot

Create Discord bots using a simple widget-based framework.

## Create Bot

1. Go to Discord's [Developer Portal](https://discordapp.com/developers/applications/).
2. Create a new application.
3. Add a bot user to your app.
4. Invite your bot to a server using: [https://discordapp.com/oauth2/authorize?scope=bot&client_id=COPY_PASTE_YOUR_DISCORD_BOT_CLIENT_ID_HERE](https://discordapp.com/oauth2/authorize?scope=bot&client_id=COPY_PASTE_YOUR_DISCORD_BOT_CLIENT_ID_HERE)

> A Discord bot's client ID is not the same as the bot's token!

5. `Click to Reveal Token` to view your bot token. You will need this in the next section.

> Keep this token and any file containing it **private**! If your token ever leaks or you suspect it may have leaked, simply `regenerate` a new token to invalidate your old token.

## Get Bot

1. `git clone https://github.com/peterthehan/create-discord-bot.git && cd create-discord-bot/ && npm install`
2. Rename [example.config.json](https://github.com/peterthehan/create-discord-bot/blob/master/example.config.json) to `config.json`.
3. Open the file and add your bot token:

```js
{
  "TOKEN": "COPY_PASTE_YOUR_DISCORD_BOT_TOKEN_HERE"
}
```

## Run Bot

1. `npm start`
2. The bot should go from offline to online. Verify the bot is working by using the `ping` command.

> The default command prefix is `.`. You can configure your own bot settings in [src/config.js](https://github.com/peterthehan/create-discord-bot/blob/master/src/widgets/command/config.js).

🎉 You're ready to create your own Discord bot! 🎉

## Examples

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
