## Affix Alerts Command

### Description
The `affix-alerts` command allows users to subscribe to weekly alerts for new Mythic+ affixes in a specified region. The bot will send alerts to the channel where the command is used.

### Usage
```
/affix-alerts [region]
```

### Options
- **region** (optional): Choose a different region. Default is `us`. Choices:
  - `us`: US/OC
  - `eu`: EU
  - `tw`: TW
  - `kr`: KR

### Permissions
- **User**: `ManageWebhooks`
- **Bot**: `ManageWebhooks`

### Examples
- Subscribe to affix alerts for the default region (US/OC):
  ```
  /affix-alerts
  ```
- Subscribe to affix alerts for the EU region:
  ```
  /affix-alerts region:eu
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to manage webhooks.
- If a subscription already exists, using the command will delete the existing subscription.
- The bot will reply with a success message when a subscription is created or deleted.