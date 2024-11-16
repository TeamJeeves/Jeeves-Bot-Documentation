## Mute Command

### Description
The mute command mutes all non-admin members in the voice channel you are currently in. Optionally, you can specify a role to mute only members with that role.

### Usage
```
/mute [role]
```

### Options
- **role** (optional): Specify a role to mute only members with that role.

### Permissions
- **User**: `MuteMembers`
- **Bot**: `MuteMembers`

### Examples
- Mute all non-admin members in your current voice channel:
  ```
  /mute
  ```
- Mute all members with a specific role in your current voice channel:
  ```
  /mute role:@RoleName
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to mute members.
- You must be in a voice channel to use this command.
- The bot will reply with an error message if you are not in a voice channel.
- To unmute the members, use the `/unmute` command.