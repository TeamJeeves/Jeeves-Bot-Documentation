# Setting up your Guild

In Jeeves 3.1, we now allow you to setup a guild, and integrate with the Role Manager to provide roles based on ranks within your guild, as well as setting discord nicknames.

***

# Initial Setup

To setup your initial guild, type the following:

For the guided process, you can simply use:

`!setup guild`

Or for quick setup, you can specify the guild name right into the `!setup` command:

`!setup guild <Guild Name> Realm Region`

At this point, your guild name is set. `!lastlog` should now pull your latest log from warcraftlogs.com


## Integrations

To enable guild rank syncing, you need to first enable the guild sync in the role manager. Type the following:

```
!setup rolemanager
guild
stop
```

This should now show Guild in the list of active integrations. Now you can set your guild role links via the following:

```
!setup guild-roles
```

From there, it's completely interactive. Just type the rank, and the name of the rank to link the 2. For example:

* `0 Guild Master` Link Rank #0 (The Guild Master), to the `@Guild Master` role on discord.
* `1 Officer` Link Rank #1, to the `@Officer` role on discord.

To enable the role manager to auto assign a nickname on !auth or !role update, use `enable-nicknames` during the guild-roles setup process.

## Further Information
* The guild rank sync happens automatically every 3 hours (This is not something we can change, as it has been decided by blizzard.)
* The guild rank will only look at your highest character in the guild, that is linked to a role on discord. For instance, if you are the guild master, and have no rank linked as a guild master, an alt of yours may be chosen as the "main", and assign you the officers rank as well as attempt to change your nickname to your officer name.
* The nickname setting will happen only on `!role update`, `!auth` or when a new user (Already !auth'd to Jeeves) enters your server. This will not happen on the guild sync that happens every 3 hours.
* To do a manual sync, use `!syncranks`.
