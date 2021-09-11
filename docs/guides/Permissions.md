# Jeeves Permissions

By default, Jeeves requests full admin rights to your discord server when you add it. This is due to the vast array of functions that Jeeves can perform and results in less support issues for things not working.

## Basic functions

The basic functions of Jeeves require Jeeves to have *View Channels*, *Send Messages* and *Embed Links* permissions

## Alerts

Any alert functions in Jeeves, such as [Realm](../commands/feeds/realm-alerts.md), [Affix](../commands/feeds/affix-alerts.md), [Recruitment](../commands/feeds/recruitment.md), [Twitter](../commands/feeds/twitter.md) or [WoWHead](../commands/feeds/wowhead-webhook.md), require Jeeves to have the *Manage Webhook* permission so that the Jeeves can add the webhook to the channel you are wanting the information to be in.

## Role Management

Role management requires Jeeves to have *Manage Roles* permissions on your discord server. It also requires Jeeves to have a role higher in the role list than the roles that it will be assigning.

## Nicknames

For Jeeves to manage nicknames of players, Jeeves requires the *Manage Nicknames* permission