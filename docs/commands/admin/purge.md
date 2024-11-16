## Purge Command

### Description
The purge command allows you to bulk delete messages from a channel. By default, pinned messages will not be deleted.

### Usage
```
/purge <limit> [filter]
```

### Options
- **limit** (required): The number of messages to remove. Must be between 1 and 500.
- **filter** (optional): Apply a filter to specify which messages to delete. Available filters:
  - **Bots**: Removes only messages posted by bots.
  - **Me**: Removes only your messages.
  - **You**: Removes only Jeeves' messages.
  - **Uploads**: Removes only messages with attachments.
  - **Links**: Removes only messages with links.
  - **Pinned**: Removes only pinned messages.

### Permissions
- **User**: `ManageMessages`
- **Bot**: `ManageMessages`

### Examples
- Purge 100 messages:
  ```
  /purge 100
  ```
- Purge 50 messages posted by bots:
  ```
  /purge 50 filter:bots
  ```
- Purge 20 messages with links:
  ```
  /purge 20 filter:links
  ```