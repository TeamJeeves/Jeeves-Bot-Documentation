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
- 'Achievements': 'commands/dashboard/role-management/achievements.md'
- 'Class': 'commands/dashboard/role-management/class.md'
- 'Faction': 'commands/dashboard/role-management/faction.md'
- 'Guild': 'commands/dashboard/role-management/guild.md'
- 'Mounts': 'commands/dashboard/role-management/mounts.md'
- 'Mythic Plus': 'commands/dashboard/role-management/mythic-plus.md'
- 'Pet Score': 'commands/dashboard/role-management/pet-score.md'
- 'Pets': 'commands/dashboard/role-management/pets.md'
- 'Professions': 'commands/dashboard/role-management/professions.md'
- 'Region/Factions': 'commands/dashboard/role-management/region-factions.md'
- 'Regions': 'commands/dashboard/role-management/regions.md'
- 'Verified': 'commands/dashboard/role-management/verified.md'