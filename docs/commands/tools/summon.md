## Summon Command

### Description
The `summon` command moves users from other voice channels into your current voice channel. This is useful for gathering members for events like raids.

### Usage
```
/summon <role>
```

### Options
- **role** (required): The role of the users you want to summon.

### Permissions
- **User**: `MoveMembers`
- **Bot**: `MoveMembers`

### Examples
- Summon all users with a specific role to your voice channel:
  ```
  /summon role:@Raiders
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to move members.
- You must be in a voice channel to use this command.
- The bot will reply with an error message if you are not in a voice channel.
- The bot will attempt to move all users with the specified role who are currently in a voice channel to your voice channel.