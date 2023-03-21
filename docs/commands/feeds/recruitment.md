# Recruitment Command

**Powered by WoWProgress**

The Recruitment command sets up a feed of players that have set themselves as looking for a guild on [WoWProgress.](https://www.wowprogress.com/)

## Find-Players

The Find-Players command sets up what types of players you would like displayed in your channel. It takes multiple optional parameters to define what you are looking for, `item-level:`, `faction:`, `prog:`, `realms:` and `region:`. Running the find-players command a second time will override the filters you have in place.

`item-level:` allows you to set a minimum item level for characters. For example `item-level:220` means that Jeeves will only display characters with at least 220 item level

`faction:` allows you to set whether you are looking for Alliance or Horde players. If have this filter set, you will not get posts of people in the other faction who are open to faction changes. You will only see players that are currently this faction.

`prog:` allows you to set a filter on the characters progression in the current tier. 5/10M would filter to characters that have 5 Mythic kills this tier. 2/10H would filter to characters with 2 Heroic kills this tier.

`realms:` allows you to filter which realms the characters are currently on. If you are on a merged realm you will want to include all realms in your group. 

`region:` allows you to filter which region you are looking for characters in.

`/recruitment find-players item-level:235 faction:Horde` This will display all Horde characters with an item level of at least 235.

## View

The view command will display your current filters.

## Stop

The stop command will turn off the incoming feed of characters

![Recruitment](../img/recruitment.jpg "recruitment!:)
***
### Developer Thoughts
>You may activate as many or as little filters as you want. Each time you run the command the filters within that command string will overwrite any previous filters you had in place. Make sure to run it as a single string with all the filters you want to apply.
***
