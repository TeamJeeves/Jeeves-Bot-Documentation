### Lookup
Looks up a specific toon or guild for all their juicy info!
***
### Details
**Aliases:** `wowprog` | `armory` | `wow-lookup` | `pug` | `wowlookup`    
**Available in DM:** No   
**Can Restrict to a channel:** Yes

* You can lookup different information about a World of Warcraft player or a guild.
* General information: `!lookup Character Realm Region`
* If you are looking up data about a character or guild on your same realm & region, you will only need to specify the name of the character or guild if your [channel data](../../guides/Channel-Data.md) and [realm](../../dashboard/settings.md) were set up correctly.
* The lookup command also supports special parameters
>-- raider (Shows a raiding info)   
-- mythic+ (Shows mythic+ info)   
-- transmog (Generates a screenshot of the characters appearance)
***
**Developer Thoughts**
>The Jeeves lookup is arguably our most core fundamental feature. When designing each lookup view the ideology used was as followed. For raiding, we imagined we are in the middle of Antorus starting Argus in the face needing 1 more DPS. We have 2 960 warlocks in the queue but we only want to bring one. The information we put in the view should be enough to quickly compare between the two and pick the best one. Of course, we also included links to external sites for a more in-depth dive into their profiles.
***
### Examples

* `!lookup Deadlystriké Mal'ganis US`
  > Perform a basic character lookup for this toon
* `!lookup Deadlystriké Mal'ganis US --mythic+`
  > Perform a character lookup targeting Mythic+ data
* `!lookup Deadlystriké Mal'ganis US --raider`
  > Perform a character lookup targeting Raid data
* `!lookup <Strawberry Puppy Kisses> Area 52 US`
  > Perform a guild lookup on Limit
***
### FAQ
#### Q) Help my character is in the US but says it cannot be found on an EU server?
>Check that the Discord server you're running the command on is located in one of the EU regions. You can also simply add the region tag behind the character
name and realm.

**Example:** `!lookup add Deadlystriké Mal'ganis [REGION]` - either US or EU
***
