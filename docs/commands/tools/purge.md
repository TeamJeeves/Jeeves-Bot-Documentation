# Purge Command

The Purge command allows you to quickly clear messages from a text channel. It has a required parameter of `limit:` for the number of messages you wish to delete, and an optional parameter of `filter:` to filter which messages are deleted.

`/purge limit:10` will delete the 10 most recent messages in the channel the command is run.

## Filter option

* Bots - This filter will only delete messages from bots
* Me - This filter will only delete message you sent
* You - This filter will only delete messages that Jeeves sent
* Uploads - This filter will only delete messages that have attachments
* Links - This filter will only delete messages that have links in them
* Pinned - This filter will only delete messages that are pinned.
***
