## Realm Status Command

### Description
The realm-status command allows users to check the status of a specified World of Warcraft realm, including its online status, type, population, and connected realms.

### Usage
```
/realm-status [realm] [region]
```

### Options
- **realm** (optional): The realm you want to check. If not specified, the default realm will be used.
- **region** (optional): Choose a different region. Default is `us`. Choices:
  - `us`: US/OC
  - `eu`: EU
  - `tw`: TW
  - `kr`: KR

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

### Examples
- Check the status of the default realm:
  ```
  /realm-status
  ```
- Check the status of a specific realm in the US region:
  ```
  /realm-status realm:Area-52 region:us
  ```
- Check the status of a specific realm in the EU region:
  ```
  /realm-status realm:Draenor region:eu
  ```

### Notes
- Ensure that the specified realm and region are valid.
- The command will display the realm's online status, type, population, connected realms, and local time.
- The bot will reply with an error message if it cannot find the specified realm.