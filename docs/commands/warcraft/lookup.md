## Lookup Command

### Description
The `lookup` command allows users to look up information about a specific character or guild in World of Warcraft.

### Usage
```
/lookup <subcommand> [options]
```

### Subcommands
- **character**: Lookup a character.
  - **name** (required): The name of the character to lookup.
  - **realm** (optional): The realm of the character.
  - **region** (optional): The region of the character. Choices:
    - `us`: US/OC
    - `eu`: EU
    - `tw`: TW
    - `kr`: KR
- **guild**: Lookup a guild.
  - **name** (required): The name of the guild to lookup.
  - **realm** (optional): The realm of the guild.
  - **region** (optional): The region of the guild. Choices:
    - `us`: US/OC
    - `eu`: EU
    - `tw`: TW
    - `kr`: KR

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

### Examples
- Lookup a character:
  ```
  /lookup character name:Thrall realm:Area-52 region:us
  ```
- Lookup a guild:
  ```
  /lookup guild name:Method realm:Tarren-Mill region:eu
  ```

### Notes
- Ensure that you provide the correct realm and region for accurate results.
- The bot will reply with an error message if it cannot find the specified character or guild.
- Character lookups may take a few seconds to complete.