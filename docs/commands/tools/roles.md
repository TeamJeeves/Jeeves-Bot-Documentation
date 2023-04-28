# Roles Command

The Roles command allows users to assign administrator defined roles to themselves.

## Setup

The first step required in order for users to be able to assign roles to themselves is for an admin to configure which roles are available. This is done in the dashboard. Follow the [guide](../../configuration/role-management.md) for more instructions on setting it up.

## Add

To assign roles to yourself use the `/roles add` command. Jeeves will then present you a drop down of the available roles.
## Remove

To remove a role from yourself use the `/roles remove` command. Jeeves will then present you a drop down of the roles you have assigned yourself.
## Update

The update command tells Jeeves to check your account against the role management integrations that your admin has configured. This will assign roles that are not manually assignable.

## Tools

Jeeves has a couple of Role Tools to help create default roles for Professions/Classes as well as sync M+ colors relative to the current season score. The Sync-colors command comes with a reset-rank if the newest season has a color shift for the scores. Typing in `/role-tools` will show in the window the entirety of the role-tool commands on Discord, simply selecting the tool you want to utilize will allow Jeeves to fire up the Mk.3.

****
