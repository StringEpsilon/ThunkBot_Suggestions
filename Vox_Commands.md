### vox

**Description**: Group of commands to manage your voice chat notification settings.

**Note**: If used on it's own, it works like `!vox settings`.

---

### vox settings

**Description**: Tells you what your current settings are.

**Example**: `!vox settings`

---

### vox notify

**Description**: Enables notifications via DM for people joining a voice channel.

This can also be used to change the status at which you want to be notified. See the `status` parameter.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| status | string | "Idle" | Specifies the status you have to be at to be notified. Available values: Online, Idle, Busy, DoNotDisturb, Offline

The status values are treated hierarchical. If you specify "Idle" you will be notified when you are either Online or Idle. If you specify "Offline", you will always get a DM.

**Example usage**: `!vox notify Online`

---

### vox unnotify

**Description**: Disables notifications for voice activity. Thunkbot will remember your settings for re-activation.

**Example usage**: `!vox unnotify`

---

### vox filter

**Description**: Commands to modify your filter settings for notifications

### vox filter whitelist

**Description**: Only receive notifications currently on your filter list.

**Note**: Doesn't change the content of your filter.

---

### vox filter blacklist

**Description**: You won't receive notifications currently on your filter list.

**Note**: Doesn't change the content of your filter.

---

### vox filter disable

**Description**: Disable filtering, but keeps the list intact for later reactivation

---

### vox filter add

**Description**: Add people to the filter for voice chat notifications.

| name | format | default | description |
|---|---|---|---|
| users | list of strings | - | The users you want to be notified about, as plain text. No @Mentions!

**Example usage 1**: `!vox filter add JustJosh` - to add just Josh.

**Example usage 2**: `!vox filter add John Will` - to add both "John" and "Will".

**Example usage 3**: `!vox filter add "Generic User"` - to add "Generic User" - for when a username contains a space.


---

### vox filter remove

**Description**: Remove people from the notification filter.

Note: If this clears the list and you've set it up as a whitelist, ThunkBot will then again notify you about all voice chat activity.

| name | format | default | description |
|---|---|---|---|
| users | list of strings | - | The users you want to remove from the filter. No @Mentions!

**Example usage 1**: `!vox filter remove JustJosh` - to remove just Josh.

**Example usage 2**: `!vox filter remove John Will` - to remove both "John" and "Will".

**Example usage 3**: `!vox filter remove "Generic User"` - to remove "Generic User" - for when a username contains a space.
