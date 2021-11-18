### Lookup
Looks up a specific toon or guild for all their juicy info!
***

## Character

The character command allows you to lookup a character. This command requires the `name:` parameter and optionally accepts `realm:` and `region:` parameters.

`/lookup character name:Deadlystriké realm:Mal'ganis region:US`

If the `realm:` and `region:` parameters are not supplied the default realm and region from your [server setup](../../configuration/setup.md) or [channel data](../../guides/Channel-Data.md) will be used instead.

***
**Developer Thoughts**
>The Jeeves lookup is arguably our most core fundamental feature. When designing each lookup view the ideology used was as followed. For raiding, we imagined we are in the middle of Antorus starting Argus in the face needing 1 more DPS. We have 2 960 warlocks in the queue but we only want to bring one. The information we put in the view should be enough to quickly compare between the two and pick the best one. Of course, we also included links to external sites for a more in-depth dive into their profiles.
***

## Guild

The guild command allows you to lookup a guild. This returns the guilds progression, ranking and Armory, RaiderIO and WowProgress links. This command requires the `name:` parameter and optionally accepts `realm:` and `region:` parameters.

`/lookup guild name:Complexity Limit realm:Illidan region:us` 

If the `realm:` and `region:` parameters are not supplied the default realm and region from your [server setup](../../configuration/setup.md) or [channel data](../../guides/Channel-Data.md) will be used instead.