# Channel Data (Channel Meta Data)

This feature is intended for use on servers which operate for a global audience with certain channels for Horde/Alliance EU/NA. Normally Jeeves has users setup their Realm/Faction/Region, however with channel data you can override that on a per-channel level.

At this time only certain settings are supported.

## Setting Jeeves Channel Data
1. Go to the channel you want to edit `You must have manage channels/admin to do this`
2. Click on Edit Channel
3. In the Overview tab edit the box called **Chanel Topic** to contain a line like this
```
--JeevesData Faction: Horde, Region: US
```
> The line should start with `--JeevesData` and contain settings formatted like `Setting: Value` separated by commas `,`

## Supported Settings & Commands
* **Faction** `Keystone`
* **Realm** `Lookup`
* **Region** `Lookup` | `Keystone`
