## SyncGuild Command

### Description
The `sync-guild` command attempts to re-sync your guild and linked Discord ranks. This process is usually done automatically.


### Usage
```
/sync-guild
```

### Permissions
- **User**: `ManageRoles`
- **Bot**: `ManageRoles`

### Examples
- Re-sync your guild and linked Discord ranks:
  ```
  /sync-guild
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to manage roles.
- The bot will reply with an error message if the guild ranks integration is disabled or if there is a permissions issue.
- The guild ranks integration must be enabled from your server's dashboard for this command to work.