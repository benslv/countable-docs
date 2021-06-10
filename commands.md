---
description: Here are all the commands you can use with Countable!
---

# Commands

## ping

Pings to bot to make sure it's running. Will reply with a message if working.

**Example: `ping`**

## set-count

Sets the next expected count for the server \(i.e. setting the count to **100** means that the next number that should be typed in the counting channel is **100**\).

**Example:** `set-count 100`

**Aliases:** `count`, `=`

| Argument | Type | Description |
| :--- | :--- | :--- |
| count | number | The value you want the next expected count to be set to. |

## set-channel

Sets the counting channel for your Discord server.

**Example:** `set-channel #counting`, `set-channel 722159296934183012`

**Aliases:** `channel`

| Argument | Type | Description |
| :--- | :--- | :--- |
| channel | channel mention or channel ID | The channel you want to count in. |

