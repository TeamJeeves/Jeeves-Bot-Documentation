# Jeeves Role Manager

The Jeeves role manager allows small guilds and large communities alike to effortlessly administer roles based on in-game stats and achievements. The role manager also supports the manual assignment of custom per-server roles as well as assigning a role to new members on-join.

The "Jeeves Role Manager" is broken into two segments. The user `!role` command, and the server admins `!setup RoleManager` command.

**Developer Thoughts**
>Many servers have some mechanism in place to issue custom roles. Some even require you "Apply" for a role by submitting your character info, and then a moderator manually assigns you a role based on some metric or stat. The Jeeves Role Manager seeks to use its large audience to unify the "Gimme A Role" experience across many servers.

***
# Role Manager scope control

99% of people should be fine with just turning on the integration with no extra options and using the default settings, but for the 1% who need ultimate customization and tuning, jeeves offers the following options

**Character scope**

* This allows you to tell Jeeves which characters should count toward roles per-integration (All Characters, Main Only, Max Level Characters) 
* to use this, add [max] [all] or [main] after the intergration, ie: class [main]. it defaults to max if not specified

**Management scope**
* This allows you to specify Jeeves management of the integrations, [full] [promote] [demote], with a secondary ssytem to determine if jeeves can automate the integration or if jeeves only handles it on a persons toon update request, [auto] [manual]
* defaults to full and auto if not specified
* an example of full control use would be:Mythicplus [max] [full] [manual]

***
# Role Manager

The Role Manager interface can be brought up with `!setup RoleManager` The interface is broken up into 6 sections

* **Available Integrations** - These are non-active available integrations for use.
* **Active Integrations**- These are the active integrations running on your server.
* **Custom Roles** - These are the custom roles you want users to be able to opt-into.
* **On-Join** - This, if any, is the role Jeeves should assign new members when they join your server.
* **Streaming Rank** - Adds the specified rank to a user who goes live, and removes it when they stop.
* **Temporary Guest Rank** - Determines if the on-join role is temporary or not.

## Integrations
**Requirements**    
 *  Valid Role Created    
 * Jeeves is above said role in the role "Hierarchy"     
 * Role is Uniquely Named


## *Guild*
The guild integration allows Jeeves to assign guild ranks based on someone's respective role in their guild.

Head on over to [guild-roles](../commands/Setup/guild-roles.md) to set up the respective roles for jeeves to track!

To toggle this integration on/off Type `guild` with the Role Manager open.

## *Mythic+ Score*
The Mythic+ Score Integration uses the score generated by RaiderIO to assign ranks to your members

Acceptable Role Formats
```
2500+ Mythic Score
2500+ Mythic+ Score
2500 Mythic Score
2500 Mythic+ Score
Below 200
```
**Note:** You may also use the world "Rank" instead of score. Supported Scores are 100-9999. Below 200 is literal and if used must be exactly that.


To toggle this integration on/off Type `mythicplus` with the Role Manager open.

## *Combo(Region-Faction)*
The Combo Region-Faction Role is useful for community servers who cater to a global audience.
This integration can help assign users to their respective group allowing them to meet up and chat with people who play in the same region as them.

Acceptable Role Formats
```
NA-Horde
US-Horde
EU-Alliance
USHorde
EUHorde
```
**Note:** Regions supported: US, NA, EU, TW, KR - Blizzard considers Oceanic part of the US/NA


To toggle this integration on/off Type `Combo(Region-Faction)` with the Role Manager open.

## *Verified*
The Verified integration adds a role by the same name to every user that successfully completes the `!authorize` process.


To toggle this integration on/off Type `Verified` with the Role Manager open.

## *Region*
The Region Integration is a simple Integration. Users will be assigned a role matching their region based on the toons added.

Acceptable Role Formats
```
EU
US
NA
TW
KR
```
**Note:** Regions supported: US, NA, EU, TW, KR - Blizzard considers Oceanic part of the US/NA


To toggle this integration on/off Type `Region` with the Role Manager open.


## *Faction*
The Faction  Integration is a simple Integration. Users will be assigned to either **Horde**, **Alliance**, or Both based on the toons they added.

Acceptable Role Formats
```
Horde
Alliance
```

To toggle this integration on/off Type `Faction` with the Role Manager open.

## *Class*
The Class Integration adds roles representing classes the user has level 60 characters of.

Acceptable Role Formats
```
Death Knight
Demon Hunter
Paladin
Warlock
Priest
....
```

To toggle this integration on/off Type `Class` with the Role Manager open.

## *Achievements*
The achivements integrations lets you show everyone just how much better at the game you are than everyone else.

Acceptable Role Formats
```
10000+ achievement score
10000 achievement score
Below 2000 achievement score
....
```

To toggle this integration on/off Type `achievements` with the Role Manager open.

## *Pet Score*
The Pet Score Integration uses your battle pet score to assign a rank.

Acceptable Role Formats
```
1500+ Pet score
1500 Pet Score
Pet Score 1500
Pet Score 1500+
Below 500 pet score
```

To toggle this integration on/off Type `petscore` with the Role Manager open.

## *Pets*
The pets integration assigns a role based the number of pets you have.

Acceptable Role Formats
```
100+ pets
100 Pets
...
```
To toggle this integration on/off Type `Pets` with the Role Manager open.


## *Mounts*
The Mounts integration assigns a role based the number of mounts you have.

Acceptable Role Formats
```
20+ mounts
20 mounts
...
```
To toggle this integration on/off Type `mounts` with the Role Manager open.

## Custom Roles

#### Adding Custom Roles

**Requirements**    
 * Valid Role Created    
 * Jeeves is above said role in the role "Hierarchy"   
 * Role is Uniquely Named

To add / remove a Custom Role simply type the name of the role like `Tank Master` with the Jeeves Role Manager window open.

## Streaming Rank

#### Adding Streaming Rank

**Requirements**  
 * Valid Role Created    
 * Jeeves is above said role in the role "Hierarchy"   
 * Role is Uniquely Named

The Streaming Rank integration allows a role to automatically be assigned to a member of your server when they go live and to be removed when they stop streaming. This can be used to allow them to gain access to private rooms, control a channel, or simply for listing them above everyone else.

To add / remove Streaming Rank type `streamer rankname`, where rankname is the role you want to use, while the RoleManager window is open.

## On-Join Roles

#### Setting your On-Join Role
**Requirements**  
 * Valid Role Created  
 * Jeeves is above said role in the role "Hierarchy"  
 * Role is Uniquely Named

To add / remove your **On-Join** Role simply type "on-join" then the name of the role you want to add / remove like `on-join New Member`
**Note:** You can only have 1 on-join role at this time.

## Temporary Guest Rank
The temporary Guest Rank integration allows you to chose whether or not the on-join rank is temporary or not. If it is set to true then the on-join rank will be removed when the user receives a role from another RoleManager integration.

To toggle this on / off simply type `Guest Rank`

### User Role Handler

### First Steps

Users must first add their toon to Jeeves. This is done through the !authorize command. You will be directed to https://jeeves.bot/go/auth/bnet and asked to log in to your Discord account. You'll then be prompted to allow Jeeves to access information from Battle.net about your character(s) / guild(s). This is the only information about your account Jeeves will EVER have access to.

## Getting a Role from a Integration
EZ  `!roles update` BOOM DONE

## Getting / Removing a Custom Role
In the case where the custom role is called **T Rex**
`!role T Rex`

### FAQ
##### Q) I saw a server running what appears to be an integration that's not listed here, can I use that?
>Let us know in the Discord server that you want it. We have developed a small few "private" integrations for more "specialized" community servers.
##### Q) Can you add an integration for XXXXXX?
>Maybe, let us know what you would like to see. The role manager tries to appeal to the greatest audience. If we are missing a key area, we want to hear about it.
##### Q) Jeeves says my server doesn't have the roles setup, what's going on?
>Jeeves will not create roles for you. Discord roles & permissions can be a sticky land mine, and I don't want to take responsibility for messing up your server. You create the roles, Jeeves will manage them.
