# Jeeves Permissions

By default, Jeeves requests full admin rights to your discord server when you add it. This is due to the vast array of functions that Jeeves can perform and results in less support issues for things not working.

## Basic functions

The basic functions of Jeeves require Jeeves to have _View Channels_, _Send Messages_ and _Embed Links_ permissions

## Alerts

Any alert functions in Jeeves, such as [Realm](../commands/feeds/realm-alerts.md), [Affix](../commands/feeds/affix-alerts.md), [Recruitment](../commands/feeds/recruitment.md) or [WoWHead](../commands/feeds/wowhead-webhook.md), require Jeeves to have the _Manage Webhook_ permission so that the Jeeves can add the webhook to the channel you are wanting the information to be in.

## Role Management

Role management requires Jeeves to have _Manage Roles_ permissions on your discord server. It also requires Jeeves to have a role higher in the role list than the roles that it will be assigning.

## Nicknames

For Jeeves to manage nicknames of players, Jeeves requires the _Manage Nicknames_ permission

## Permissions

| Permission                 | Required | Reason                                                                                                        |
| -------------------------- | :------: | ------------------------------------------------------------------------------------------------------------- |
| Administrator              |    No    |                                                                                                               |
| Manage Server              |    No    |                                                                                                               |
| Manage Roles               |   Yes    | This permission is required in order for Jeeves to assign roles                                               |
| Manage Channels            |    No    |                                                                                                               |
| Kick Members               |    No    |                                                                                                               |
| Ban Members                |    No    |                                                                                                               |
| Create Invite              |    No    |                                                                                                               |
| Manage Nicknames           |   Yes    | This permission is required in order for Jeeves to assign nicknames to users                                  |
| Change Nickname            |    No    |                                                                                                               |
| Manage Emojis and Stickers |    No    |                                                                                                               |
| Manage Webhooks            |   Yes    | Jeeves setups webhooks for many Alert functions                                                               |
| View Audit Log             |    No    |                                                                                                               |
| Read Messages              |   Yes    | This basic permission allows Jeeves to see commands in chat                                                   |
| Send Messages              |   Yes    | This basic permission allows Jeeves to send messages in chat                                                  |
| Embed Links                |   Yes    | This permission is required for Jeeves to embed data in posts                                                 |
| Read Message History       |    No    |                                                                                                               |
| Use External Emojis        |   Yes    | Jeeves makes use of external emojis for the `!keystone list` command                                          |
| Connect                    |    No    | Jeeves no longer has audio functions                                                                          |
| Speak                      |    No    | Jeeves no longer has audio functions                                                                          |
| Move Members               |   Yes    | This permission is required in order for Jeeves to perform the [Summon](../commands/tools/summon.md) function |
| Use Voice Activity         |    No    |                                                                                                               |
