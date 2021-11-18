# Authorize Command

The authorize command links your Battle.net account to Jeeves. This allows Jeeves to access your character list for up to 24 hours. This is how Jeeves monitors and knows who your characters are.

There is one optional parameter to this command, `region:`. This is the region your WoW account is associated with. Without this parameter Jeeves will send you a link based on your [server setup](../../configuration/settings.md) or your Discord server region.

`/authorize`

Jeeves will send you a DM with a link to click on to start the process of authorizing Jeeves to see your characters in WoW.

When you create new characters in the future, you will need to run `/authorize` again, as this command only allows Jeeves to see your characters for 24 hours.
***
