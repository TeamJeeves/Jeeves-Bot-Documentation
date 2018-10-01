# Setup command

The setup command is the main command used when first setting up Jeeves.

This command has two modes: **Guided** and **Targeted**.

Guided setup is triggered by simply running `!setup`, which provides a prompt-based introduction and explanation of the most basic settings.  
`!setup` is recommended for all first-time fresh installs of Jeeves.

Targeted setup allows you to quickly change a given setting. For example, if you wished to change the prefix that Jeeves responds to you could target that setting with `!setup prefix`.

You can further choose to either run `!setup prefix` in which you will be shown a brief into and explanation of that setting and then prompted to change / clear it, OR you can run `!setup prefix ?` to directly change the prefix without the prompts.

Below are a list of available setup settings:

`!setup` - Enter Guided Setup  
`!setup prefix` - Prefix Configuration  
`!setup realm` - Realm Configuration  
`!setup audio-mode` - Audio Mode Configuration  
`!setup bot-channel` - Bot Channel Configuration  
`!setup audio-channel` - Music Channel Configuration  
`!setup greeting` - Welcome message configuration  
`!setup RoleManager` - Automatic Role Management Options + custom roles  
`!setup role-channel` - Reaction based role channel configuration  
`!setup lookup-mode` - Sets the default view/info displayed when running a character lookup  


#### About

**Aliases:** `setup`  
**Available in DM:** No  
**Can Restrict to a channel:** Yes  
**Global Support:** Yes  

**Examples:**  

- `!setup` - Enter guided setup  
- `!setup bot-channel` - Configure the bot-channel setting  
- `!setup bot-channel #use-bot-here` - Configure the bot-channel setting to use #use-bot-here without prompts  

***

# Prefix Setup

This command allows you to setup your servers prefix, the thing that comes before all commands.

**Examples**

* `!setup prefix` - Start the setup wizard for setting up your servers prefix, this is also done in the normal `!setup` steps.
* `!setup prefix $` - Will set your server to use $ for all commands.

***

# Realm Setup

This command allows you to setup your servers realm, the server warcraft server you want your server to default to.

**Examples**

* `!setup realm` - Start the setup wizard for setting up your servers realm, this is also done in the normal `!setup` steps.
* `!setup realm anvilmar` - Will set your server to use Anvilmar as your default realm.

***

# Audio Mode Setup

This command allows you to setup your servers audio mode.  
There are 5 different modes that can be set.  

* **Off** Audio is off. No one can use it.
* **On** Audio is on. Everyone can use it.
* **Selective** Only people you Select or Allow may use audio.
* **Restrictive** Everyone except the people you restrict can use audio.
* **DJMode** Only people with the role AudioDJ can use audio.

**Examples**

* `!setup audio-mode` - Start the setup wizard for setting up your servers audio mode, this is also done in the normal `!setup` steps.
* `!setup audio-mode Off ` - Turns off audio for your server

***

# Bot Channel Setup

This command allows you to setup your servers bot channel.

**Examples**

* `!setup bot-channel` - Start the setup wizard for setting up your servers bot channel, this is also done in the normal `!setup` steps.
* `!setup bot-channel #use-bot-here` - Limits bot commands to the channel `#use-bot-here`. **Note:** Administrator can run commands in any channel where Jeeves has able to read and send messages.

***

# Audio Channel Setup

This command allows you to set what audio channel that you want Jeeves to play music in.

**Examples**

* `!setup audio-channel` - Start the setup wizard for setting up what audio channel that you want Jeeves to play music in.
* `!setup audio-channel music ` - Sets Jeeves to play music in the channel `music`.

***

# Greeting Setup

This command allows you to configure a server greeting.  
Jeeves supports two different ways of sending a greeting to a new user. You can have him send a message to a channel or send a private message to the user.  
The first step is to run `!setup greeting`. This will start the setup wizard for setting up a greeting message.  
There are 3 different modes that can be set.  

* **Disable** This is Jeeves default setting and can be set to disable sending welcome messages.
* **DM** This setting will direct message a user when they join your server.
* **#Channel** This will post a welcome message in a channel when they join your server

Once you have setup your welcome setting in discord you want to head over to your server settings on the Jeeves site. For more info head over to the [server management](/guides/Using-Jeeves-Website/#server-management) page for more information.


**Aliases:** `none`
**Available in DM:** No
**Can Restrict to a channel:** Yes
**Global Support:** Yes

**Examples**

* `!setup greeting` - Start the setup wizard for setting up a greeting message.
* `!setup greeting DM` - Will set welcome messages to go to DM's.
* `!setup greeting #welcome-spam` - Will set welcome messages to go to #welcome-spam.
* `!setup greeting Disable` - Will disable the welcome messages

### FAQ
##### (Q) Why is Jeeves not sending a welcome message?
Make sure you have set up the welcome message on the Jeeves site.

***

# Role Manager Setup

This will setup Jeeves to manage roles on your server. See [Jeeves Role Manager](/guides/Role-Manager.md) page for more information.

**Examples**

* `!setup RoleManager` - Start the setup wizard for setting what roles Jeeves will manage.

***

# Role Channel Setup

This tells Jeeves what channel he should monitor for incoming reaction events. Normal users are limited to 1 channel, this should be more then fine for 99% of cases. If you require more then 1 channel consider becoming a Patreon to unlock the ability to have multiple role channels. See [Role Reaction](/commands/admin/rolereaction.md) page for more information.

**Examples**

* `!setup role-channel` - Start the setup wizard for setting up what channel that you want Jeeves to watch for reactions.
* `!setup role-channel #get-ranks-here` - Tells Jeeves to monitor `#get-ranks-here` for reactions.

***

# Lookup Mode Setup

Jeeves has different lookup modes, this will set what one is the default for your server. As always, you can override the lookup view locally when the command is run by adding the parameter --VIEWNAME

There are 3 different modes that can be set.

* **Default** This is Jeeves default setting. It displays Raid progression, M+ score, achievement points, character stats, boss kills, best M+ dungeon, current PvP ranking and sim string.
* **Raider** Shows current raid progression, equipped and bag item levels, artifact traits, gems socketed, enchants, M+ score, best M+ dungeon, and what legendries they have equipped.
* **MythicPlus** Shows M+ score, raid progression, best M+ dungeon weekly and season, tertiary stats, artifact traits, and what legendries they have equipped.


**Examples**

* `!setup lookup-mode` - Start the setup wizard for what setup mode you would like Jeeves to use.
* `!setup lookup-mode Raider` - Sets Jeeves to default to the raider view for character lookups.
