# Lookup Command

You can look up different information about a World of Warcraft player or a guild.

**Aliases:** `lookup`

**Available in DM:** No

**Can Restrict to a channel:** Yes

**Global Support:** Yes

**Examples**

* `!lookup Deadlystriké Mal'ganis US` - Lookup basic information about this character

* `!lookup Deadlystriké Mal'ganis US --mythic+`    - Get mythic+ information for this character

* `!lookup Deadlystriké Mal'ganis US --raider` - Get raiding information for this character

* `!lookup <Limit> Illidan US - Lookup basic information about this guild


**Developer Thoughts**
>The Jeeves lookup is arguably our most core fundamental feature. When designing each lookup view the ideology used was as followed. For raiding, we imagined we are in the middle of Antorus starting Argus in the face needing 1 more DPS. We have 2 960 warlocks in the queue but we only want to bring one. The information we put in the view should be enough to quickly compare between the two and pick the best one. Of course, we also included links to external sites for a more in-depth dive into their profiles.
***


### FAQ
##### (Q) Help my character is in the US but says it cannot be found on an EU server?
Check that the Discord server you're running the command on is located in one of the EU regions. You can also simply add the region tag behind the character 
name and realm.

**Example:** !lookup add Deadlystriké Mal'ganis [REGION] - either US or EU