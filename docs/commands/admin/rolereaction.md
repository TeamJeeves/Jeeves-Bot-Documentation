# RoleReaction Command

This command allows you to configure `RoleReactions`.

`RoleReactions` are the term used for a reaction that when clicked assigns a role.

Jeeves supports the use of all valid discord emojis as valid RoleReaction emojis including the newly animated emojis. Emojis are linked to roles on a per-channel basis. You can use the same emoji for different roles in different channels.

The **first thing you should do** is run `!setup RoleChannel`. This tells Jeeves what channel he should monitor for incoming reaction events. Normal users are limited to 1 channel, this should be more than fine for 99% of cases. If you require more then 1 channel consider becoming a Patreon to unlock the ability to have multiple role channels.

There are 4 different actions this command can perform.

* `set`  linking an emoji to a role - When setting a role, the role must have the "Allow anyone to @mention this role" setting enabled. You can disable this after the set action has been performed.  
* `clear`  unlinking an emoji  
* `view`  getting a list of all linked emojis  
* `reset` this clears all linked emojis - **This action is not reversible**  

**NOTE** Jeeves must be listed in the server roles higher than the roles that you want him to manage.

**Patreon Users:** With multiple role channels set up, Jeeves needs to know what channel you are talking about when running the commands below. Include a channel reference like #Get-Roles in all commands OR run the commands from the role channel you wish to edit.
***
### Details

**Aliases:** `RoleReaction`  
**Available in DM:** No  
**Can Restrict to a channel:** Yes  
***
### Examples

* `!roleReaction set 💰 @GreedyGoblin`
> Links the money bag emoji to the GreedyGoblin Role  
* `!roleReaction clear 💰`
> Unlinks the money bag emoji from all roles  
* `!roleReaction view`
> Get a list of linked emojis and their role  
* `!roleReaction reset`
> Wipe all rolereaction data  
* `!roleReaction set 💰 @GreedyGoblin #Get-Roles`
> Patreon Multi-Channel example where #Get-Roles is a second channel  

***

### FAQ

#### Q) How many RoleReactions can I have?   
> 50 per channel

#### Q) Can I have 2 Emojis with the same name?    
> No, Jeeves links emojis by their name, not their icon or their ID.

#### Q) Can I have 2 Emojis with the same icon?    
> Yes, as long as the name is different you are free to have 50 emojis with the same image.

#### Q) I deleted a linked emoji from my discord server, how can I clear it without resetting everything?    
> Create a new emoji with the same name and run the clear command with that emoji.
