## Trivia Command

### Description
The trivia command starts a new trivia game session in your server. Users can join the session and answer trivia questions to earn points.

### Usage
```
/trivia
```

### Permissions
- **User**: No special permissions required.
- **Bot**: `ManageChannels`, `SendMessages`, `DeleteMessages`, `EmbedLinks`, `ManagePermissions`

### Examples
- Start a new trivia game session:
  ```
  /trivia
  ```

### How It Works
1. **Channel Creation**: The command checks for a channel named trivia. If it doesn't exist, the bot attempts to create it.
2. **Session Check**: If a trivia session is already ongoing, the bot will notify the user and provide a link to the existing session.
3. **Game Start**: The bot sends a message to the channel, inviting users to join the trivia session.
4. **User Commands**: Users can start the game by typing `start`, stop the game by typing stop, and configure game settings such as time limit, question time limit, deck size, and flood control.
5. **Trivia Questions**: The bot asks trivia questions, and users can answer by typing their responses. The first correct answer earns a point.
6. **Result Announcement**: The bot announces the correct answer and updates the scoreboard.
7. **New Round**: The bot asks if users want to start another round. If yes, a new game starts; if no, the session ends.

### Notes
- Ensure that Jeeves has the necessary permissions to manage channels and send messages.
- The bot will reply with an error message if it fails to create the trivia channel or if there is an ongoing session.
- Users can configure game settings by typing specific commands in the trivia channel:
  - time limit <minutes>: Set the game time limit.
  - question time limit <seconds>: Set the time limit for each question.
  - deck size <number>: Set the number of questions in the game.
  - `flood control <on/off>`: Enable or disable flood control.