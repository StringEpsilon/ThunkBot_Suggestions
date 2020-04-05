**Note:** For voice chat related commands, [click here](./Vox_Commands.md).

### addcountry

**Description**: Adds the specified country "role" to your profile.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| name | string | - | Name of the country you want added to your profile.

See [this list of available countries](./CountryHelp.md) and their names / aliases.

**Aliases**: `country`, `setcountry`

### clearcountry

**Description**: Clear all countires (or just the specified one) 'roles' from your profile.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| name | string | - | Optional. Specify which of your assigned countries you want to remove.

See [this list of available countries](./CountryHelp.md) and their names / aliases.

**Aliases**: -

### roll

**Description**: Rolls the specified dice.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| dicepool | XdY\[+/-n\] | 1d6 | Describes the dicepool you want to roll. You can specify up to 1000 sides and 100 dice (100d1000). Amount defaults to 1 (!roll d8 rolls 1d8). Default die is a d6 (!roll 10 rolls 10d6)
| reporter | string | "min" | Option to change how the roll result will be presented. Available: min, verbose, average, coin, sr, unique.

**Aliases**: `r`

---
### episode

**Description**: Posts a link to the episode of the number you specified.

Note: The "THUNK 60" videos are not supported.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| episode | numeric or "random" | random | The episode number you want to see (e.g. "100" or "164.5"). "random" or "rnd" selects a random episode for you to enjoy.
| force | "force" or "true | Admin only option. | 

**Aliases**: `ep`, `thunk`, `THUNK`

---
### pun

**Description**: Quotes the intro from the specified episode.

Note: Episode 0 and the "THUNK 60" episodes don't have an intro. 

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| episode | numeric or "random" | random | The episode number you want to get the quote from (e.g. "100" or "164.5"). "random" or "rnd" selects a random episode to satiate your pun cravings.
| force | "force" or "true | Admin only option. | 

---
### goodbot

**Description**: Let's ThunkBot (and everyone else) know that he was in fact a good boy.  

ThunkBot keeps track of how often and by whom he was thanked. You can also thank him by reacting with `:heart:` emote to his messages.

**Parameters**: None.

**Aliases**: `thx`, `thanks`, `goodboy`

---
### bug

**Description**: Posts the link to this GitHub repository.

**Parameters**: None.

**Aliases**: `issue`, `feedback`, `ticket`, `idea`,

---
### ping

**Description**: Answers with "pong".

**Parameters**: None.

---

### gamelist

**Description**: Admin only. Displays the current list of games ThunkBot keeps in escrow. All game keys are kindly gifted away by other people on the server. Please say thank you to whoever gave away the game you took.

**Special note**: Unlike any other command output, ThunkBot will edit his latest reply to this particular command as people claim and donate games.

**Parameters**: None.

---

### claimgame

**Description**: ThunkBot will send you the stored game key via DM and cross the game off his list. 

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| gameId | numeric | - | The number of the game you want.

---

### donategame

**Description**: Add a new game to the give-away pile! Thank you very much!

**Special note:** ThunkBot will delete your message if you use this command in a public channel. Just to make sure nobody snags the game unnoticed. But you should just use this via DM anyway.

**Parameters**:

| name | format | default | description |
|---|---|---|---|
| name | any | - | The name of the game. If it's more than one word, use quotation marks: `"Portal 2"` is valid. `Portal 2` without the quotation marks is invalid. 
| key | any | - | The key for the game. Again, if it contains spaces, use quotation marks.
