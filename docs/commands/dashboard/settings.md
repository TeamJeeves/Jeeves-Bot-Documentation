# Dashboard Settings

This section of the Dashboard allows you to set the Prefix of Jeeves, default region and realm Jeeves will use with your discord server, and the welcome message Jeeves will greet new members to your server with.

## Prefix

Don't run two or more bots with the same prefix. In the context of `!help` **!** is the prefix. These should be unique to each bot. On the settings page you can set the prefix you would like Jeeves to use on your discord server.

If you run into an issue where you cant remember Jeeves' prefix, run `@Jeeves#2457 prefix` and it will return the servers prefix for Jeeves, assuming there is one.

## Default Region and Realm

The default region and realm for your discord server saves you from having to tell Jeeves which realm you are on each time you run a command.

You can only setup a single realm as your default realm. If you play on a cross-realm server it's highly advised that you set your main realm as the realm your guild was created on.

## Welcome Message

The welcome message is a message that Jeeves will either put in a channel or DM to the user when a user joins your discord server. This message can be up to 3500 characters. Jeeves will split the message into multiple message if it is above 2000 characters. This is the discord message limit.

Jeeves will automatically mention the new user in the message. You can mention other users and roles in this message if you wish. To do this you will need the user id or role id in discord. This can be found by turning on [Devleoper Mode](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-). For a user, enter the id as `<@{user id}>` for example `<@1234>`. For a role, enter the id as `<@&{role id}>` for example `<@&1234>`