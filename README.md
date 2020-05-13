Adds a plethora of additional features to server queue for players with permission. This plugin aims to move the various queue plugins all into one singular queue plugin, and allow easy configuration of which players have access to each feature.

## Features

* Queue Capacity
* New players skip queue
* Skip queues
* Skip the queue if they recently disconnected
* Players with certain auth level skip queue no matter what

## Permissions

All permissions are customizable in the config files. You may use the default plugin permissions, or use permissions provided by other plugins.

## Configuration

```json
{
  "Auth Level required to skip queue no matter what (3 = none, 2 = admin, 1 = moderator)": 3,
  "Enable first connect skip queue?": true,
  "Enable Queue Capacity?": false,
  "If a player has one of the listed permissions, they are affected by queue capacity.": [
    "ultimatequeue.default"
  ],
  "Queue capacity": 50,
  "Enable Queue Holding?": true,
  "If a player has one of the listed permissions, their queue spot is held on disconnect": [
    "ultimatequeue.default",
    "ultimatequeue.vip"
  ],
  "Number of minutes to allow a user to reconnect without a queue": 5,
  "Enable Queue Skipping?": true,
  "If a player has one of the listed permissions, they will skip the queue": [
    "ultimatequeue.vip"
  ],
  "When a user joins for the first time, message the new user. Only works with first connect queue skip enabled": true,
  "When a user joins for the first time, announce it to all users. Only works with first connect queue skip enabled": true
}
```

## Localization

```json
{
  "CapacityReached": "The server's queue is full.",
  "FirstJoinMessage": "Welcome to the server!",
  "FirstJoinMessageGlobal": "Welcome {0} to the server!"
}
```