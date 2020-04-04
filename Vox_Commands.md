### vox_notify

**Description**: Enables notifications via DM for people joining a voice channel.

This can also be used to change the status at which you want to be notified. See the `status` parameter.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| status | string | "Idle" | Specifies the status you have to be at to be notified. Available values: Online, Idle, Busy, DoNotDisturb, Offline

The status values are treated hierarchical. If you specify "Idle" you will be notified when you are either Online or Idle. If you specify "Offline", you will always get a DM.

**Example usage**: `!vox_notify Online`

### vox_unnotify

**Description**: Disables notifications for voice activity. This command also clears your whitelist (compare `!vox_addusers`)

**Example usage**: `!vox_unnotify`

### vox_addusers

**Description**: Add people to the whitelist for voice chat notifications, so that you'll only be notified about them.

| name | format | default | description |
|---|---|---|---|
| users | list of strings | - | The users you want to be notified about, as plain text. No @Mentions!

**Example usage 1**: `!vox_addusers JustJosh` - to add just Josh.
**Example usage 2**: `!vox_addusers John Will` - to add both "John" and "Will".
**Example usage 3**: `!vox_addusers "Generic User"` - to add "Generic User" - for when a username contains a space.
### vox_removeusers

**Description**: Remove people from the notification whitelist.

Note: If this clears your whitelist, ThunkBot will then again notify you about all voice chat activity.

| name | format | default | description |
|---|---|---|---|
| users | list of strings | - | The users you want to remove from the whitelist. No @Mentions!

**Example usage 1**: `!vox_removeusers JustJosh` - to remove just Josh.
**Example usage 2**: `!vox_removeusers John Will` - to remove both "John" and "Will".
**Example usage 3**: `!vox_removeusers "Generic User"` - to remove "Generic User" - for when a username contains a space.
