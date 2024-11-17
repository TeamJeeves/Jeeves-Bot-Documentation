# Troubleshooting Common Problems

## User Issues

### I Linked my Account but see no characters
There are 2 common causes for this issue. 

1. Wrong Account - Ensure you are logged into the correct account over at Battle.Net
2. Permissions - The **first** time you go through the Authorization process you get sent over to the Battle.Net website for Authorization & Confirmation. If you unselected the check box that grants Jeeves access to view your characters, things will fail. To correct this you will need to head over to Battle.Net, Login, Goto Connected Applications, Remove Jeeves, then Authorize again. 

### The bot is sending "Emtpy" messages.
Jeeves uses "Embeds" for many responses due to the greater formating they allow. 

Enable the following setting in discord:

`User Settings > Chat > Embeds and Link Previews`

## Server Issues

### It won't let me add my WoW Guild
We only allow Officers and the GM to add a guild. This is for security and privacy reasons. Unfortunatly blizzard doesn't tell us the name or permissions attached to a given guild rank. We have no way of knowing if Rank 2 is Officer, or if Rank 2 is Co-GM, or GM-Alt. As such we only the GM and the rank directly under GM to add their guild. Once the guild is added to Jeeves anyone with "Manage Server" permissions in the discord can take over and configure and manage settings from there reguardless of their in-game rank. 