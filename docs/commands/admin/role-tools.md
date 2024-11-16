## Role Tools Command

### Description
The role-tools
 command provides various subcommands to manage roles within your server. This includes creating authorization buttons, managing Mythic Plus roles, and generating default roles for classes and professions.

### Usage
```
/role-tools <subcommand> [options]
```

### Subcommands
- **create-auth-button**: Creates an authorization button for role management.
- **mythic-plus**: Group of subcommands for managing Mythic Plus roles.
  - **sync-colors**: Synchronize the colors of Mythic Plus roles with the current Raider.IO score colors.
  - **reset-ranks**: Reset the ranks of Mythic Plus roles. Options:
    - **method**: How to reset the ranks. Choices:
      - `delete`: Delete the roles.
      - `rename`: Rename the roles.
    - **warning**: Type "I Understand" to confirm the action.
- **class**: Group of subcommands for managing class roles.
  - **generate-default-roles**: Generate default roles for each class with the correct class color and default permissions. Option:
    - **template-role**: (Optional) Choose an existing role to clone permissions from.
- **professions**: Group of subcommands for managing profession roles.
  - **generate-default-roles**: Generate default roles for each profession with default permissions. Option:
    - **template-role**: (Optional) Choose an existing role to clone permissions from.

### Permissions
- **User**: `ManageRoles`
- **Bot**: `ManageRoles`, `EmbedLinks`

### Examples
- Create an authorization button:
  ```
  /role-tools create-auth-button
  ```
- Synchronize Mythic Plus role colors:
  ```
  /role-tools mythic-plus sync-colors
  ```
- Reset Mythic Plus ranks by deleting roles:
  ```
  /role-tools mythic-plus reset-ranks method:delete warning:"I Understand"
  ```
- Generate default class roles:
  ```
  /role-tools class generate-default-roles
  ```
- Generate default profession roles with a template role:
  ```
  /role-tools professions generate-default-roles template-role:@TemplateRole
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to manage roles and send embedded messages.
- The bot will reply with an error message if it lacks the required permissions or if the action requires additional confirmation.