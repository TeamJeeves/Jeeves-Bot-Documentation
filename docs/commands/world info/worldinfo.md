## WorldInfo Command Documentation

### Overview
The `worldinfo` command provides information about current and upcoming world events across various World of Warcraft expansions, including **Legion**, **Battle for Azeroth (BFA)**, and **Shadowlands (SL)**. Users can check schedules, current events, and region-specific details.

---

### Key Features
- **Event Tracking**: Stay informed about world bosses, faction assaults, invasions, and more.
- **Region-Specific Data**: Choose between US, EU, TW, and KR regions.
- **Customizable Schedule**: View current events or upcoming schedules.

---

### Command Syntax
```
/worldinfo <expansion> event:<event> [region:<region>] [schedule:<true/false>]
```

---

### Subcommands and Events

#### 1. **Legion**
Provides information about world events in Legion areas such as the Broken Isles and Argus.

- **Events**:
  - `archeology`: Displays the schedule for the weekly Archeology quests.
  - `fishing`: Shows the schedule for Fishing Friend daily quests.
  - `greater-invasion`: Lists the weekly Argus Greater Invasions.
  - `invasion`: Details Broken Isles invasions.
  - `karazhan`: Displays the rotation for the Karazhan Opera Event.
  - `worldboss`: Shows the weekly rotation of Legion world bosses.

- **Example**:
  ```
  /worldinfo legion event:worldboss region:us schedule:true
  ```

#### 2. **Battle for Azeroth (BFA)**
Provides information about current events in Kul Tiras and Zandalar.

- **Events**:
  - `freehold`: Displays the Freehold Boss schedule.
  - `faction-assaults`: Lists the current and upcoming Faction Assaults.
  - `worldboss`: Shows the weekly rotation for world bosses in BFA zones.
  - `warfront`: Displays the status and schedule of Warfronts.

- **Example**:
  ```
  /worldinfo bfa event:faction-assaults region:eu schedule:true
  ```

#### 3. **Shadowlands (SL)**
Provides information about world events in Shadowlands zones.

- **Events**:
  - `worldboss`: Displays the weekly rotation of Shadowlands world bosses.

- **Example**:
  ```
  /worldinfo sl event:worldboss
  ```

---

### Optional Parameters

- **region**: Specifies the region for the event data. Defaults to the server’s region.
  - Available options: `us`, `eu`, `tw`, `kr`.
  - **Example**:
    ```
    /worldinfo legion event:archeology region:eu
    ```
- **schedule**: Shows the schedule for upcoming events if set to `true`. Defaults to `false`.
  - **Example**:
    ```
    /worldinfo bfa event:freehold schedule:true
    ```

---

### Examples
- Check the current Legion worldboss in the US region:
  ```
  /worldinfo legion event:worldboss region:us
  ```
- View the upcoming schedule for BFA faction assaults in the EU region:
  ```
  /worldinfo bfa event:faction-assaults region:eu schedule:true
  ```
- Display the Karazhan Opera Event rotation in Legion:
  ```
  /worldinfo legion event:karazhan
  ```
- View the Shadowlands world boss for the week:
  ```
  /worldinfo sl event:worldboss
  ```

---

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks` permission required.

---

### Notes
- Ensure that Jeeves has the `EmbedLinks` permission to display event details correctly.
- Data is region-specific and updated according to the latest available information.
- If data is unavailable for a specific event or region, the bot will return an error message.

---

### Quick Reference Table

| Expansion  | Event             | Description                          |
|------------|-------------------|--------------------------------------|
| **Legion** | `archeology`      | Weekly Archeology quests schedule    |
|            | `fishing`         | Fishing Friend daily quests schedule |
|            | `greater-invasion`| Argus Greater Invasion schedule      |
|            | `karazhan`        | Karazhan Opera Event rotation        |
|            | `worldboss`       | Weekly world boss rotation           |
| **BFA**    | `freehold`        | Freehold Boss schedule               |
|            | `faction-assaults`| Faction Assault schedule             |
|            | `worldboss`       | Weekly world boss rotation           |
|            | `warfront`        | Warfront status and schedule         |
| **SL**     | `worldboss`       | Weekly world boss rotation           |

