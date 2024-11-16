## WorldBoss Command

### Description
The `worldboss` command allows users to check which world boss is currently active and view the upcoming schedule for world bosses in a specified region.

### Usage
```
/worldboss [region]
```

### Options
- **region** (optional): Choose a different region. Default is `us`. Choices:
  - us: US/OC
  - eu: EU
  - tw: TW
  - kr: KR

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Check the current world boss for the default region (US/OC):
  ```
  /worldboss
  ```
- Check the current world boss for the EU region:
  ```
  /worldboss region:eu
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- The command will display the current week's world boss and the upcoming schedule for the next few weeks.
- The bot will reply with an error message if it is unable to retrieve data for the current world boss.