## Unmute Command

### Description
The `unmute` command unmutes all non-admin members in the voice channel you are currently in.

### Usage
```
/unmute
```

### Permissions
- **User**: `MuteMembers`
- **Bot**: `MuteMembers`

### Examples
- Unmute all non-admin members in your current voice channel:
  ```
  /unmute
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to mute and unmute members.
- You must be in a voice channel to use this command.
- The bot will reply with an error message if you are not in a voice channel.
- The bot will attempt to unmute all users who were previously muted in the voice channel.