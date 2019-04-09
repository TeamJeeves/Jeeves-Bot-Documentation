# Character Command

The Character command allows you to Manager your Synced Character Sheet


***

### Details

**Aliases:** `character` | `toon`   
**Available in DM:** No   
**Can Restrict to a channel:** Yes

* View your characters
* View another users characters
* Mark certain characters as your *Main* or *Hidden*
* Request an update for your characters

**Hidden Characters:** Hidden characters will still be "Ranked/Scored/Counted" but will be hidden from other users

**Ignored Characters:** Ignored characters are treated as if they do not exist. You will not get roles for them, nor will they appear in `!toon view`. You can have as many of these as you want, but you must still have 1 character not ignored.

**Main Character:** Only 1 character can be your main. When running a command involving a character like the keystone command Jeeves will assume your main character if none are mentioned

***

### Examples

* `!toon view`
> Shows you a list of your 12 best characters
* `!toon update`
> Queues your characters for update
* `!toon set-main Deadlystrike`
> Tells Jeeves to consider Deadlystrike your main
* `!toon hide Secretsauce`
> Tells Jeeves to flag Secretsauce as hidden
* `!toon sync-account`
> Re-syncs your character sheet (Only available within 24hrs of an `!auth`, re-run `!auth` instead of this if its past 24hrs)

***

### FAQ

#### Q) Why can I only see 12 characters in `!toon view`?<br>
> Its a limitation with how many characters (2000) you can have in a discord message, 12 is the amount we could display comfortably. Rest assured your other characters are still there!
***
