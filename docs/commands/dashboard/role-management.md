# Dashboard Role Management

The Jeeves role manager allows small guilds and large communities alike to effortlessly administer roles based on in-game stats and achievements. The role manager also supports the manual assignment of custom per-server roles as well as assigning a role to new members on-join.

## Getting started

For Jeeves to be able to manage roles, Jeeves needs to be assigned to a role above the ranks you want it to manage.
<!--- #TODO: Add roles listing picture --->

Jeeves will also not create the ranks. This is the responsibility of Discord server admin. All integrations require uniquely named roles in order for Jeeves. 

The first step for any role management to occur is to enable role management. This will give you the options for Streamer role, On-join role and Custom roles.

### Streamer role

The Streaming Role integration allows a role to automatically be assigned to a member of your server when they go live and to be removed when they stop streaming. This can be used to allow them to gain access to private rooms, control a channel, or simply for listing them above everyone else.

Select the role you wish streamers to have in the drop down to enable this feature

### On-join role

The On-join role integration assigns a role to a user when they join the discord server. This role is selected via the 'On-join role' dropdown.

Jeeves can either apply this role indefinitely, or it can remove this role when another integration assigns a role to the user. This option is chosen via the 'Should on-join be temporary?' toggle.

### Custom roles

The Custom role integration allows users without role management permissions to assign roles to themselves on your discord server. The roles that a user can assign are controlled by the custom roles that are setup in Jeeves.

To setup a role you need to enter a name and the role.
<!--- #TODO: Add example screenshot --->
For a user to grant themselves a role they need to type `!role {name}`. For the example above they would type `!role `

## Integrations

There are a number of integration that Jeeves has available to use. For more instructions on each one please see its page.

- [Achievements](role-management/achievements.md)
- [Class](role-management/class.md)
- [Faction](role-management/faction.md)
- [Guild](role-management/guild.md)
- [Mounts](role-management/mounts.md)
- [Mythic Plus](role-management/mythic-plus.md)
- [Pet Score](role-management/pet-score.md)
- [Pets](role-management/pets.md)
- [Professions](role-management/professions.md)
- [Region/Factions](role-management/region-factions.md)
- [Regions](role-management/regions.md)
- [Verified](role-management/verified.md)

## Integration scope

All Jeeves Role Management integration have scope options. These options allow you to choose how Jeeves handles assigning the roles for that integration.

![Screenshot](../../../img/role-management-scope.png)

The Characters drop down allows you to limit which characters a player has that the integration should apply to. Please note, not all options are available or applicable to all integrations.

- All - This will mean that the integration will apply the roles that apply for all characters on the players account
- Max Level - This means the integration will only apply to max level characters that the player has on their account
- Main Only - This means the integration will only look at the character that the player has [set as their main](../warcraft/character.md).

The Management drop down allows you to decide how Jeeves should apply the integration.

|Option|Description|
|------|-----------|
|Fully Managed|This option means that Jeeves will add and remove the roles associated with this integration as they change for the characters of the users account.|
|Only Promote|This option means that Jeeves will only add roles to the user and will not remove those that no longer apply.|
|Only Demote|This option means that Jeeves will only remove roles from the user and will not add new roles that apply to the user.|
    
The Mode drop down allows you to decide if Jeeves should automatically update the roles of a player or if the user needs to run `!toon update`. 
- Auto
    * This means that as Jeeves scans the characters it will automatically update the roles assigned to the player
- Manual
    * This means that a user will need to run `!toon update` in order for new roles to be assigned to them.
## FAQ
#### Q) I saw a server running what appears to be an integration that's not listed here, can I use that?
>Let us know in the Discord server that you want it. We have developed a small few "private" integrations for more "specialized" community servers.
#### Q) Can you add an integration for XXXXXX?
>Maybe, let us know what you would like to see. The role manager tries to appeal to the greatest audience. If we are missing a key area, we want to hear about it.
#### Q) Jeeves says my server doesn't have the roles setup, what's going on?
>Jeeves will not create roles for you. Discord roles & permissions can be a sticky land mine, and I don't want to take responsibility for messing up your server. You create the roles, Jeeves will manage them.