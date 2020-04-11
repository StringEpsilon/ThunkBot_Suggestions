## Privacy

The Bot keeps track of the following data:

0) Exception and error handling.

In order to diagnose problems and malfunctions, I write [exceptions](https://en.wikipedia.org/wiki/Exception_handling) into a logfile. I try my best to keep user relevant information out of that logfile. I also clear the logfile pretty regularly.

1) Statistics about command usage.

The bot tracks how many times each command was used. And entirely separate from that, the bot keeps a list of users who used any command and how many times they have done so. I can not reconstruct how many times user A has used command Y.

2) How many times the bot was thanked (but not by whom)

The bot keeps a simple counter for !goodbot and `:heart:` reactions to his messages. Again, no user information is safed for this purpose.

3) Game giveaway claims and donations.

People can give game keys away through the bot via `!DonateGame`. The bot will then keep the necessary data (name of the game, name of the donor and the game key). The bot will also record who claimed that game key via `!claimgame`.

4) How many messages are posted to each channel per day. Looks like this: "thunkbucket, 2020-102, 42 messages".

5) User specific settings.

For the [voice chat notifications](./Vox_Commands.md) and the `!remindme`  command, the bot needs to keep some data for the respecitve user. These are:

**!vox_notify**

* The unique user ID used internally in the Discord APIs (just a long random looking number)
* The desired minimum availability status you want to be notified at ("Idle", "Online", etc.)
* A whitelist of people you want to be notified about, if you configured that.
* Whether you were recently notified by the bot or not.

You can clear this data entirely with `!vox_unnotify`.

**!remindme**

* The unique user ID used internally in the Discord APIs (just a long random looking number)
* The message you left for yourself, if you left any.
* The time of the desired notification.

You can clear this data entirely with `!ClearReminders`. 



### Privacy and  `!census`

The `!census` command (admin only) iterates through each member of the discord server and counts the assigned roles. This information is available to any user of the server anyway. ThunkBot does not keep any additional records.
