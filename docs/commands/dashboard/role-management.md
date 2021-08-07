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

## Achievements

The Achievements integration assigns roles based on the number of achievement points a player has.
## Class

The Class integration assigns roles based on the classes of the characters a player has.
## Faction

The Faction integration assigns roles based on the faction of the characters a player has.
## Guild

The Guild integration assigns roles based on guild rank of the characters a player has. For more information see the [Guild](guild.md) dashboard page.
## Mounts

The Mounts integration assigns roles based on the total number of mounts a player has associated to their account.
## Mythic Plus

The Mythic Plus integration assigns roles based on the (raider.io)[https://raider.io] score a player has.
## Pet Score

## Pets

The Pets integration assigns roles based on the total number of pets a player has associated to their account.
## Professions

The Professions integration assigns roles based on the primary professions the characters of a player has.
## Region/Factions

The Region/Factions integration assigns roles based on the region of a players account as well as the faction that their characters are.
## Regions

The Region integration assigns roles based on the region of a players account.

## Verified

The Verified integration assigns the 'Verified' role to all users that have linked their discord account to a battle.net account via `!auth`