# Setting up your keyboard

In Jeeves 3.1, we now allow you to have a static board.  A static board is a channel on discord that no one can post in and has just 1 info post.  This post is managed by the Jeeves system to show current info. The first one is just for keystones.  This is a patreon only feature.

***

# Setup
##Step One
The first step you need to do is invite Jeeves's little helper Keystone bot.

[Click here to invite KeystoneBot](https://discordapp.com/oauth2/authorize?client_id=393186410548690953&scope=bot&permissions=2080374975)

## Step Two

You need to make a channel that ``@everyone`` does not have permission to post to and you need to edit the channels topic and add some channel data to it [Channel Data](Channel-Data.md)

IE: ``--JeevesData Faction: Horde, Region: US``

## Step Three

You need to run ``!install-keyboard`` in the channel that you have just set up.  This will tell the bot to post in this channel.

## Further Information
* Your members still have to do the [keystone commands](../commands/warcraft/keystone.md) in a valid bot channel to add the keys. Blizzard does not provide an API for use to get this data.
