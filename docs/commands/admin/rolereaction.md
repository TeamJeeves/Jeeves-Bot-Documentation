# Reaction-Role Command

`Reaction-Role` are the term used for a reaction that when clicked assigns a role.

Jeeves supports the use of all valid discord emojis as valid RoleReaction emojis including the newly animated emojis. Emojis are linked to roles on a per-channel basis. You can use the same emoji for different roles in different channels.

### Details
 
**Available in DM:** No  
**Can Restrict to a channel:** Yes  
***

## Listen

The **first thing you should do** is run `/reaction-role listen`. This command has a required channels parameter. You should enter the channel name like `#roles` This tells Jeeves what channel he should monitor for incoming reaction events. This command can be run form any channel as it is pointed to the channel to monitor. Normal users are limited to 1 channel, this should be more than fine for 99% of cases. If you require more then 1 channel consider becoming a [Patreon](../../guides/Supporting-Jeeves.md) to unlock the ability to have multiple role channels.

## Set

The set command tells Jeeves what role to link to which emoji. It takes 2 required parameters `emoji:` and `role:`. The emoji just needs to be typed in and Discord will provide you a list of roles to select from that can be assigned for the command.

`/reaction-role add emoji:💰 role:@GreedyGoblin`

If you are a Patreon you have the ability to have multiple role channels, you need to also include the optional parameter of `channel:`. Discord will display a list of channels to select from.

`/reaction-role add emoji:💰 role:@GreedyGoblin channel:#role-channel-2`
## Remove

The remove command tells Jeeves to stop assigning a role based on one emoji. It has one required parameter of `emoji:` Type the emoji into this parameter.

`/reaction-role remove emoji:💰`

If you are a Patreon you have the ability to have multiple role channels, you need to also include the optional parameter of `channel:`. Discord will display a list of channels to select from.

`/reaction-role remove emoji:💰 channel:#role-channel-2`
## View

The view command will show you all currently setup emojis for your server and the roles that Jeeves grants when they are selected.

`/reaction-role view`
## Clear

The clear command removes all emojis setup on your server for all channels. This command can not be undone and should be used carefully. It will also cause Jeeves to stop listening to all channels for Reaction-Role selections. Once this command has been run you will need to setup Reaction-Role again from scratch.

`/reaction-role clear`

## To Note

Jeeves must be listed in the server roles higher than the roles that you want him to manage.

***

### FAQ

#### Q) How many RoleReactions can I have?   
> 50 per channel

#### Q) Can I have 2 Emojis with the same name?    
> No, Jeeves links emojis by their name, not their icon or their ID.

#### Q) Can I have 2 Emojis with the same icon?    
> Yes, as long as the name is different you are free to have 50 emojis with the same image.

#### Q) I deleted a linked emoji from my discord server, how can I clear it without resetting everything?    
> Create a new emoji with the same name and run the remove command with that emoji.
