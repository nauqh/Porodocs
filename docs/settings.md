# :fontawesome-solid-flask: Configuration

Porobot supports a few options when it comes to customizing its behavior in your server. You must have admin permissions to change any of these settings.

## Installation

Create a `.env` file to store the application authentication token and guild ids

```sh
TOKEN = BOT_TOKEN
GUILD = DISCORD_SERVER_ID
STDOUT_CHANNEL_ID = OUTPUT_CHANEL_ID
VOICE_CHANNEL_ID = VOICE_CHANNEL_ID
RIOT = RIOT_TOKEN
```

Install dependencies:

```sh
$ pip install -r requirements.txt
```

Start the bot

```sh
$ python -m porobot
```

## Lavalink server

The server configuration is done in `application.yml`. You can find an example configuration [here](https://github.com/lavalink-devs/Lavalink/blob/master/LavalinkServer/application.yml.example).

- [x] Lavalink's port will always 443
- [x] Default password youshallnotpass
- [x] Using custom lavalink client if your client doesnt support secure options

## Dashboard
Welcome to your Poro Dashboard! This page allows you to view and edit a few different core server settings. This page also shows you recent activity on your Dashboard, so you can view recent changes which have been made by other Administrators.

The top part of your Dashboard will list simple server info. This includes how many channels/roles your server has.

There is also an Announcements box that shows recent updates to Dyno.

## Permission
Porobot's permissions can be configured the same way as any other Discord bot which uses slash commands. If you have both the **Manage Server** and **Manage Roles** permissions in a Discord server, you are able to define which Discord users and roles are allowed to use which commands, and in which channels. You can define permissions in the Integrations menu of the Server Settings. Then click Manage next to Porobot. See also [Discord's guide](https://support.discord.com/hc/en-us/articles/4644915651095-Command-Permissions).

Before slash commands were introduced, Porobot had a different permission system with predefined levels. This system has been completely removed.