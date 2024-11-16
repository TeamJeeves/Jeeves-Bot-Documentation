## Authorize Command

### Description
The `authorize` command links your BattleNet account with Jeeves, allowing the bot to access your World of Warcraft character information.

### Usage
```
/authorize [region]
```

### Options
- **region** (optional): Choose a different region. Default is `us`. Choices:
  - `us`: US/OC
  - `eu`: EU
  - `tw`: TW
  - `kr`: KR

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

### Examples
- Link your BattleNet account with the default region:
  ```
  /authorize
  ```
- Link your BattleNet account with the EU region:
  ```
  /authorize region:eu
  ```

### Notes
- Ensure that your Discord privacy settings allow DMs from server members.
- The bot will send you a DM with a personalized link to authorize your BattleNet account.
- If the bot is unable to send you a DM, it will notify you to check your privacy settings.