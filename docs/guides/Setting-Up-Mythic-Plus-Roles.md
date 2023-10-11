# Jeeves Discord Bot: Setting up Mythic Plus (M+) Role Integration

With the Jeeves Discord bot, you can enrich your server experience by assigning roles based on a player's M+ Score for the current season. Here's how you can set it up:

## Step-by-step Guide

1. **Add Jeeves to Your Discord Server**: Start by inviting Jeeves bot to your server.

2. **Login to Jeeves Website**: Head over to the Jeeves website and sign in.

3. **Access Server Dashboard**: Navigate to the Server Dashboard specific to your server. From there, move to the _Role Management_ tab.

4. **Activate M+ Integration**: Within the Role Management tab, enable the `Role Management` feature. Subsequently, activate the `M+ Integration`.

## Default Role Settings

By default, Jeeves provides roles based on the following naming formats:

- `2500+ Mythic Score`
- `2500+ Mythic+ Score`
- `2500 Mythic Score`
- `2500 Mythic+ Score`
- `Below 200`

**Remember**: You're required to manually create roles for these ranks on your server.

## Custom Role Settings

If you wish to designate custom names for the roles:

1. Enable the `Custom Role Map` option within the M+ Integration page.

2. Specify the role you'd like to assign at each rank.

## Role Assignment Process

- **For New Users**: After joining your server, users should either execute the `/authorize` command or click the _Authorize_ button. Once they link their accounts, Jeeves will automatically assign the appropriate roles within a 60-second window.

- **For Existing Users**: If they've authorized in the past, they can use the `/roles update` command. This will refresh their data and ascertain if they qualify for a role update.

**Note**: Servers with a _Premium_ status benefit from automatic character data refreshes and routine role updates. After the initial authorization, no further commands are necessary.

## Important Information

- **Character Knowledge**: Jeeves only recognizes characters available at the time of authorization. Any changes to a character's name or realm, or the addition of new characters, will necessitate re-authorization for detection.

## Pro Tips

- **Sync Role Colors**: Execute `/role-tools mythic-plus sync-colors` to align the colors of your M+ Roles with the current raiderio score shades.

- **Reset Ranks at Season's End**: The command `/role-tools mythic-plus reset-ranks` is handy for resetting everyone's rank at the conclusion of each season. Please be cautious with this command and ensure you read its accompanying documentation.
