## Time Command

### Description
The `time` command displays the current time and converts it across different timezones.

### Usage
```
/time [time]
```

### Options
- **time** (optional): The time you want to convert (e.g., `9pm CDT`). If not provided, the current time will be used.

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Display the current time in various timezones:
  ```
  /time
  ```
- Convert a specific time to various timezones:
  ```
  /time time:9pm CDT
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- The command will display the time in various timezones including Eastern, Central, Mountain, and Pacific for the Americas, and GMT, Central, Eastern, and Moscow for Europe.
- The bot will also provide a Discord timestamp that can be pasted in chat to share the time.