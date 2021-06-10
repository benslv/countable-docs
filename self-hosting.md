---
description: >-
  A quick guide on how to get your own, self-hosted version of the bot up and
  running!
---

# Self-hosting

I'd recommend adding the official bot to the server to ensure you get the latest updates more easily and, eventually, are able to compete against other servers using the same bot.

If you _really_ want to host your own version, however, read on to find out how!

### 1. Clone the repository

```bash
git clone https://github.com/benslv/countable.git
```

### 2. Move into the newly-created directory

```bash
cd countable
```

### 3. Install the bot's dependencies

```bash
yarn install
```

### 4. Create a config file

Create a file called `config.json` in the root of the project directory. Place the `CLIENT_ID` and `CLIENT_TOKEN` from your own bot application into it like so:

```javascript
{
  "CLIENT_ID": "ID goes here",
  "CLIENT_TOKEN": "token goes here"
}
```

{% hint style="info" %}
Follow this [guide](https://discordjs.guide/preparations/setting-up-a-bot-application.html) for instructions on how to create your own bot application.
{% endhint %}

### 5. Add your bot to a server

Use this [guide](https://discordjs.guide/preparations/adding-your-bot-to-servers.html) to add your bot to a server of your choice. Once done, you can test whether the bot works correctly with the following command.

```bash
yarn start
```

If everything is working correctly, you should see the bot appear as online in the sidebar of your server!

### 6. \(optional\) Host the bot permanently

You'll probably notice that closing the terminal window stops the bot from responding to any messages. Not exactly ideal...

There are plenty of guides out there on hosting your bot permanently somewhere, so I won't go into much detail about that here. 

If you want to get it running on your own server, the bot comes bundled with a package called `pm2` which will help you run the bot on your machine without needing to keep a terminal window open all the time. To get that running, type in the command:

```bash
yarn pm2
```

You should see a message that looks a little bit like the one below. Once that's all set up, you can go ahead and close the terminal window and your bot should continue to run like normal.

![](.gitbook/assets/pm2-guide.png)

{% hint style="info" %}
You can stop the bot running whenever you want with the command `yarn stop`, but to actually stop the `pm2` process as well, use `yarn kill.` 
{% endhint %}

