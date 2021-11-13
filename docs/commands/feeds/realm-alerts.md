# Realm Alerts

Get notified of the status of a realm. This will create notifications in a channel when the realm goes offline and when it comes back online. Useful for maintenance periods (especially the long ones)

This command has one required parameter `realm:` and one optional parameter `region:`. For Realm enter the name of the realm you wish to monitor. The region parameter allows you to specify which region the server is in.

`/realm-alerts realm:Proudmooore region:US`

Multiple commands can be run in one channel to receive alerts for multiple realms.

## Stop alerts

To stop the alerts just run the same command again, Jeeves will remove the alert setup if it is already setup.

![Realm-Alerts]('../../img/realm-alerts.png')