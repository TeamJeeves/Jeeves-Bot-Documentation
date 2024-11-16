## Gambling Command

### Description
The 

gambling

 command starts a new gambling session in your server. Users can join the session and participate in a gambling game.

### Usage
```
/gambling
```

### Permissions
- **User**: No special permissions required.
- **Bot**: `ManageChannels`, `SendMessages`, `DeleteMessages`, `EmbedLinks`, `ManagePermissions`

### Examples
- Start a new gambling session:
  ```
  /gambling
  ```

### How It Works
1. **Channel Creation**: The command checks for a channel named gambling. If it doesn't exist, the bot attempts to create it.
2. **Session Check**: If a gambling session is already ongoing, the bot will notify the user and provide a link to the existing session.
3. **Game Start**: The bot sends a message to the channel, inviting users to join the gambling session.
4. **User Intake**: Users can join or leave the session by sending `1` to join or `-1` to leave.
5. **Gambling Time**: Once enough users have joined, the bot rolls the dice and determines the winner.
6. **Result Announcement**: The bot announces the winner and the results of the rolls.
7. **New Round**: The bot asks if users want to start another round. If yes, a new game starts; if no, the session ends.

### Notes
- Ensure that Jeeves has the necessary permissions to manage channels and send messages.
- The bot will reply with an error message if it fails to create the gambling channel or if there is an ongoing session.