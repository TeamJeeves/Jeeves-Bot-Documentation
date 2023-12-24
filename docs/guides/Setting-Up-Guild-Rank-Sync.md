# Jeeves Discord Bot: Setting up the Guild Role Integration

Jeeves is able to monitor your guilds roster and automaticaly promote/demote users in your discord server to roles based on their in-game rank.

## Setting up the Guild Role Integration

1. **Link your BattleNet Account**: Run the `/authorize` command to start the process

2. **Login to Jeeves Website**: Head over to the Jeeves website and sign in.

3. **Access Server Dashboard**: Navigate to the Server Dashboard specific to your server. From there, move to the _Guild_ tab.

4. **Add your guild**: Within the Guild tab, click Add Guild and enter the Name, Realm, Region of your guild and hit save.

5. **Linking Roles** Back on the Guild Tab, Select your guild. You can now choose which roles should be applied at each rank of your guild. Be sure to save!

.... Profit?

## Common Questions

### How long does it take after being promoted in-game for Jeeves to detect the change and update their role?

**TLDR:** 1-4 hours

Blizzard refreshes guild data only once every 3 hours and only for guilds with recent activity. Due to this, Jeeves waits 3 hours after the last succesfull guild scan before trying again.

### Can I set more then 1 role per rank?

_Yes_ - This is a feature available with Premium

## Role Assignment Process

Guild Role Automation is handled automaticaly as long as Jeeves is aware of the users characters via `/authorize`. As soon as the next scan of your guild goes through if Jeeves is aware of any character belonging to the user that are reported by blizzard to have joined, left, or had a rank change, action will be taken.

**Reminder**: New Characters, Realm Transfers, and Name Changes as always require a fresh `/authorize` run by the user for Jeeves to be aware of the character.

## Important Information

- **Character Privacy**: It is impossible to hide characters that are in the guild from your guild. Running `/character view @username` within a Guild Server will ignore the hidden/ignored character settings for any characters they have that are in the guild. Hidden/Ignored characters that are not apart of the guild will not be shown.

- **Inactive Guilds**: Guilds that go inactive in-game for a extended period of time get flagged as inactive by Jeeves and will no longer get periodic scans/updates. You may run into this in cases were your guild is returning to WoW after a long break and have previously setup that same guild with Jeeves in the past. If your guild in flagged as inactive a "Reactivate" button should appear on the Guilds page in the Server dashboard next to the guild in question.

## Pro Tips

- **Be Careful with Officer Roles**: Consider the permissions you are giving to the discord roles managed via the Guild Integration. Vanity Roles, or Roles that grant access to channels are no problem, but roles that give Administrative powers are dangerous. If you have to kick out a malicious officer from your guild, it could take a few hours for Jeeves to detect that and they could use Jeeves to temporarily regain their discord roles even after manualy demoting them.

- **The Sync-Guild Command**: This command serves only 1 purpose. If you recently did some housekeeping and reorganized your Discord server, new roles, old roles, all the things have changed. This command re-evaluates all of your guild members in discord. If your in-game ranks were juggled as well you likely don't need this command, this command is only helpful if you deleted some of the roles tied to the game ranks and created new ones in their place and you need to re-sort everyone to their new roles. It does not fetch fresh data from Blizzard nor does it check roles from any other integrations besides guild roles.
