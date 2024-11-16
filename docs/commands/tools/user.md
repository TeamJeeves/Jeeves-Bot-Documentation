## User Command

### Description
The user command provides information about a specific user in the server.

### Usage
```
/user <user>
```

### Options
- **user** (required): The user you want to get information about.

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Get information about a specific user:
  ```
  /user user:@Username
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- The command will display information such as the user's name, roles, server join date, Discord join date, and whether the user is authorized with Jeeves.
- The bot will reply with an error message if the specified user is not found.