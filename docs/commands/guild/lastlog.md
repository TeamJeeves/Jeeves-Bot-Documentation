## LastLog Command

### Description
The `lastlog` command fetches the most recent uploaded WarcraftLogs report for your guild.

### Usage
```
/lastlog
```

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Fetch the most recent WarcraftLogs report for your guild:
  ```
  /lastlog
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- Your guild must be registered with Jeeves to use this command. If your guild is not registered, you will receive an error message.
- The bot will reply with an error message if there is an issue fetching data from WarcraftLogs.
- The command will provide a link to the most recent log report if available.