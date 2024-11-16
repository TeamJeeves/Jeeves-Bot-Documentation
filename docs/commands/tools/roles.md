## Roles Command

### Description
The roles command allows users to manage their roles within the server. Users can update their roles, add custom roles, or remove custom roles.

Role Managment is one of the most powerful and systems features Jeeves has. Implementations can be simple and straight forward, or deep and complex depending on your servers need. If setting up Role Managment through Jeeves for the first time, checkout the full indepth Role Managment Guide [HERE](../../configuration/role-management) 
### Usage
```
/roles <subcommand> [options]
```

### Subcommands
- **update**: Checks for roles you're automatically eligible for and updates them.
- **add**: Add a custom role to yourself.
- **remove**: Remove a custom role from yourself.

### Permissions
- **User**: No special permissions required.
- **Bot**: `ManageRoles`

### Examples
- Update your roles:
  ```
  /roles update
  ```
- Add a custom role to yourself:
  ```
  /roles add
  ```
- Remove a custom role from yourself:
  ```
  /roles remove
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to manage roles.
- The bot will reply with an error message if the server does not have custom roles set up.
- When adding or removing a role, the bot will prompt you to select a role from a list of available custom roles.