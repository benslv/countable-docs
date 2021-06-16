---
description: Here are all the commands you can use with Countable!
---

# Commands

## ping

Pings to bot to make sure it's running. Will reply with a message if working.

**Example: `ping`**

**Aliases:** none

## set-count

Sets the next expected count for the server \(i.e. setting the count to **100** means that the next number that should be typed in the counting channel is **100**\).

**Example:** `set-count 100`

**Aliases:** `count`, `=`

| Argument | Type | Description |
| :--- | :--- | :--- |
| count | number | The value to set as the next expected count. |

## set-channel

Sets the counting channel for your Discord server.

**Example:** `set-channel #counting`, `set-channel 722159296934183012`

**Aliases:** `channel`

| Argument | Type | Description |
| :--- | :--- | :--- |
| channel | channel mention or channel ID | The channel you want to count in. |

## set-emoji

Sets the reaction used by the bot when a user sends a count with no message \(if `set-nomessage` is **true**.\)

**Example:** `set-emoji 👋`, `set-emoji :custom_emoji:`

**Aliases:** `emoji`

| Argument | Type | Description |
| :--- | :--- | :--- |
| emoji | emoji | The emoji to react with. |

## set-prefix

Sets the bot's prefix \(to invoke commands with\).

**Example:** `set-prefix !`, `set-prefix c$`

**Aliases:** `prefix`

| Argument | Type | Description |
| :--- | :--- | :--- |
| prefix | string | The prefix to use commands with. |

## set-highestcount

Sets the highest count reached in the server.

**Example:** `set-highestcount 100`

**Aliases:** `highest`, `highestcount`

| Argument | Type | Description |
| :--- | :--- | :--- |
| count | number | The value to set as the highest count. |

## set-nomessage

Sets whether to react to counts which don't contain a message.

**Example:** `set-nomessage true`

**Aliases:** `nomessage`

| Argument | Type | Description |
| :--- | :--- | :--- |
| value | true/false | Whether to enable this option or not. |

## set-numbersonly

Sets whether users can include a message with their count, or if it has to be the count only.

**Example:** `set-numbersonly false`

**Aliases:** `numbersonly`

| Argument | Type | Description |
| :--- | :--- | :--- |
| value | true/false | Whether to enable this option or not. |

## set-failrole

Sets the role to be applied when a user gets the count wrong.

Providing no argument will _disable_ this feature.

**Example:** `set-failrole @role`, `set-failrole`

**Aliases:** `failrole`

| Argument | Type | Description |
| :--- | :--- | :--- |
| role \(optional\) | role mention | The role to be applied to users. |

## stats

Returns the stats for yourself or another user in the current server.

**Example:** `stats`, `stats @poisonwasp`

**Aliases:** none

| Argument | Type | Description |
| :--- | :--- | :--- |
| user \(optional\) | user mention | The user you want to get the stats for. |

## serverinfo

Returns information about the current server as a whole \(e.g. current count, highest count, prefix etc.\)

**Example:** `serverinfo`

**Aliases:** `server`, `info`

## leaderboard

Display the leaderboard for the current server.

**Example:** `leaderboard`

**Aliases:** `board`, `top`, `scoreboard`

## milestone

A collection of commands related to adding/deleting/listing milestones. Milestones are currently used to change the channel name upon reaching specified counts.

**Aliases:** none

### milestone add

Adds a milestone to the current server.

**Example:** `milestone add 100 intense-counting`

| Argument | Type | Description |
| :--- | :--- | :--- |
| count | number | The count to add a milestone at. |
| name | string | What to rename the channel to. |

### milestone remove

Removes a milestone from the current server.

**Example:** `milestone remove 100`

| Argument | Type | Description |
| :--- | :--- | :--- |
| count | number | The count to remove the milestone from. |

### milestone list

Lists the milestones added in the current server.

**Example:** `milestone list`

