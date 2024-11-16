## Attendance Command

### Description
The `attendance` command allows users to update their attendance status for upcoming raids and allows officers to audit the current attendance in a voice channel.

This command integrates with WoWAudits Raid Roster Planner. Create a Roster on WoWAudit and Manage it in discord via Jeeves.
### Usage
```
/attendance <subcommand> [options]
```

### Subcommands
- **update**: Update your attendance status for an upcoming raid.
  - **status** (required): Your attendance status. Choices:
    - `available`: You can attend.
    - `tentative`: You might attend.
    - `late`: You will be late.
    - `unavailable`: You cannot attend.
  - **date** (required): The date you are updating for. Accepts common date formats such as `today` or `5/25/2025`.
  - **reason** (optional): Provide a reason for your status.
- **audit**: Perform an audit of who is currently in the voice channel (Officer Only).
  - **channel** (optional): The voice channel to audit. If not specified, the bot will audit the channel the user is currently in.

### Permissions
- **User**: 
  - `update`: No special permissions required.
  - `audit`: `ManageGuild`
- **Bot**: `EmbedLinks`

### Examples
- Update your attendance status to available for today:
  ```
  /attendance update status:available date:today
  ```
- Update your attendance status to unavailable for a specific date with a reason:
  ```
  /attendance update status:unavailable date:5/25/2025 reason:On vacation
  ```
- Audit the current voice channel:
  ```
  /attendance audit
  ```
- Audit a specific voice channel:
  ```
  /attendance audit channel:#VoiceChannelName
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to send embedded messages.
- The bot will reply with an error message if it fails to create the `trivia` channel or if there is an ongoing session.
- Users must link their Battle.net account to Jeeves using the `/authorize` command to update their attendance status.
- Officers can only audit the voice channel if they have the `ManageGuild` permission and are currently in a voice channel.