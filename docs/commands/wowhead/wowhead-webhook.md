## Wowhead Webhook Command

### Description
The `wowhead-webhook` command allows users to subscribe to Wowhead news updates via a webhook. Users can choose to receive updates for all news or specific categories.

### Usage
```
/wowhead-webhook [news]
```

### Options
- **news** (optional): Choose the type of news you want to receive. Default is `all`. Choices:
  - `all`: All news
  - `retail`: Retail news
  - `classic`: Classic news
  - `development`: Development news
  - `other`: Other Blizzard games news

### Permissions
- **User**: `ManageWebhooks`
- **Bot**: `ManageWebhooks`

### Examples
- Subscribe to all Wowhead news:
  ```
  /wowhead-webhook
  ```
- Subscribe to Wowhead retail news:
  ```
  /wowhead-webhook news:retail
  ```

### Notes
- Ensure that Jeeves has the necessary permissions to manage webhooks.
- If a subscription already exists, using the command will delete the existing subscription.
- The bot will reply with a success message when a subscription is created or deleted.