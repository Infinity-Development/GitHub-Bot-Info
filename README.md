# GitHub Updates

- Displays notifications in your Discord channels when selected events are triggered.
- Can utilise GitHub Webhook "secrets" to secure your updates for private or public repositories.

---

## Setup

1. Add a webhook to your repository pointing to https://github.dbots.site. Select any events you would like to listen for.
    > To add a webhook, visit your repository on github.com, click the settings tab, then webhooks.
2. Set the content type to `application/json`.
3. Authorise the bot on your server by clicking [this link](https://discord.com/api/oauth2/authorize?client_id=896602816838250549&permissions=545057538016&scope=bot%20applications.commands).
4. Once the bot is active on your Discord server, you can use the slash commands listed below.

---

## About secrets

You can specify a secret value when subscribing to receive webhook events. Keep in mind this secret will be stored in plain text on a server somewhere.

Don't just enter your "default password" as the secret, use some random value, unrelated text, or best of all: [a hashed value](https://emn178.github.io/online-tools/sha256.html).

> If anyone guesses your secret, they can also subscribe to your webhook events!

---

## Usage

Commands all start with `/` and will give you tool-tips if you start typing in Discord.

Command | Description
--------|------------
`/sub <org> <name> [secret] [previews]` | Subscribe the current channel to the repo webhook events. Optionally takes a secret. Optionally enable link previews.
`/unsub <org> <name>` | Unsubscribe the current channel from the repo webhook events.
`/help` | View the bots Help Command
`/invite` | Get a Link to Invite the Bot

> Previews will not display if your repo is set to private.
