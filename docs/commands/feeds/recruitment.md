# Recruitment Command

**Powered by WoWProgress**


***
### Details
**Aliases:** `recruitment`  
**Available in DM:** No   
**Can Restrict to a channel:** Yes

* This command allows you to get notified when someone is looking for a guild based on the filters you set.
***
### Applicable filters
*  `Level` - (Excepts a number 10-120)
*  `Region` - (Expects EU, US, TW, KR)
*  `Faction` - (Expects "Horde" or "Alliance")
*  `Realm` - (Expects a realm name with no spaces, use dashes)
>  You must include the region filter if specifying a realm
*  `Realms` - (Expects multiple realms separated by commas)
*  `ItemLevel` - (expects a minimum itemlevel, 100-415 accepted)
*  `RaidLevel` - (Expects "Normal", "Heroic", or "Mythic")
 > This filter will only show people who have killed a boss on the specified difficulty within the last 2 raid tiers

### Getting Started

*  `!recruitment` - Enables the Webhook without filters in the **channel** you type this command in
*  `!recruitment stop` - Disables the Webhook
*  `!recruitment view` - View your current filters
***
### Examples
* #### `!recruitment level:120 region:us raidLevel:mythic`
* #### `!recruitment region:us faction:horde realm:malganis`
* #### `!recruitment region:us realms:duskwood,bloodhoof,bleeding-hollow`
***
### Developer Thoughts
>You may activate as many or as little filters as you want. Each time you run the command the filters within that command string will overwrite any previous filters you had in place. Make sure to run it as a single string with all the filters you want to apply.
***
