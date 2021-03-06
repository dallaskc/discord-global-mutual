# discord-global-mutual

## Important

Recent changes to the discord api essentially rendered this tool incapable of fetching needed data, hence the reason for archiving the repo.

## Description

Get the list of people that you have shared servers with. And it works for all users, not just friends.

**Note:** It's not a nodejs module, as you might expect, it's just a set of few scripts. However if you want to make it a module, please do, any contributions are welcomed!

Repo consists of 3 different scripts.

1. **export** - lists and exports all people from all guilds/servers you are joined to, in the json format
2. **compare** - compares people across all servers, and reduces list to people that have one than more shared server with you, saves in the json format
3. **print** - prints list in the console sorted by amount of shared servers (from biggest to lowest)

# Installation

1. Clone/download repository
2. Get in the downloaded directory: `$ cd discord-global-mutual`
2. While in the folder, run `$ npm install`
3. Run each of the scripts like shown below

# Usage

```sh
$ node export.js [YOUR_DISCORD_USER_AUTH_TOKEN]
$ node compare.js
$ node print.js > output.txt
```

# Getting Token

To get Discord user auth token, you can just get the one, that is used in your browser/discord client.
Open Chrome Dev Tools -> Network tab, find any Discord API request, click on it, scroll to Request Headers, and there it is, the "authorization" header.
Just copy the value and use it ;)
