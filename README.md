# Valentines
> We're back w/Valentines 3. Yes, Valentines plugin in middle of summer but who said you can't use it. In this version, there are many updates. Everything is in GUI and there are literally two commands `/valentines` and `/vgui`.

## Features
- GUI
- Particle effects system
- Marriage system
- Statistics
- Mood system
- Chat Features (for example, Words like "love" become ♥)
- Highly customizable
- Special events (Anniversary, Marriages, 
- Update checks (Experimental(Information about new version on SpigotMC))
  
## Commands and Permissions

| Command              | Description                | Permission             |
|----------------------|----------------------------|------------------------|
| `/valentines `        | Displays commands         | `valentines.use`       |
| `/vgui`        | Opens main GUI      | `valentines.use`       |
| `-` | Enable particle effects    | `valentines.effect`    |
| `-` | Marriage system access    | `valentines.marry`    |
| `-` | Divorce capability    | `valentines.divorce`    |
| `-` | Reloads plugin    | `valentines.reload/admin`    |



<details>
<summary>Configuration - config.yml</summary>

```
# ═══════════════════════════════════════════════════════════════════════════════
#                        VALENTINES PLUGIN ver3.0.0-beta
#                          Advanced Valentines Plugin
# ═══════════════════════════════════════════════════════════════════════════════

# ═══════════════════════════════════════════════════════════════════════════════
#                             CONTACT AND SUPPORT
# Website  https://sonemcpl.pages.dev
# Discord: https://sonemcpl.pages.dev/invite
# ═══════════════════════════════════════════════════════════════════════════════

# Plugin prefix
Prefix: "&c❤&f&lValentines&c❤&r "

# ═══════════════════════════════════════════════════════════════════════════════
#                                CHAT FEATURES
# ═══════════════════════════════════════════════════════════════════════════════

# Symbol replacement in chat
symbol-change: true
symbol-color: "&c"
symbol: "♥"
words:
  - "love"
  - "valentines"
  - "heart"
  - "romance"
  - "cute"
  - "sweet"
  - "darling"
  - "honey"
  - "babe"
  - "baby"

# ═══════════════════════════════════════════════════════════════════════════════
#                               PARTICLE EFFECTS
# ═══════════════════════════════════════════════════════════════════════════════

# Effects configuration
effect:
  enabled: true
  particle-density: 2
  update-rate: 3
  max-height: 2.5
  start-height: 0.1
  radius: 1.0

# Individual effect toggles
player-effects: true
kiss-effect: true
marriage-effect: true
hug-effect: true

# ═══════════════════════════════════════════════════════════════════════════════
#                                WORLD SETTINGS
# ═══════════════════════════════════════════════════════════════════════════════

# Enabled Worlds for effects and features
enabled-worlds:
  - "world"
  - "world_nether"
  - "world_the_end"

# Disabled worlds (blacklist)
disabled-worlds: []

# ═══════════════════════════════════════════════════════════════════════════════
#                                 COOLDOWNS
# ═══════════════════════════════════════════════════════════════════════════════

# Cooldowns (in seconds)
cooldowns:
  hug: 45
  kiss: 60
  like: 240
  mood-change: 120

# ═══════════════════════════════════════════════════════════════════════════════
#                               MARRIAGE SYSTEM
# ═══════════════════════════════════════════════════════════════════════════════

# Marriage settings
marriage:
  proposal-timeout: 45
  proposal-cooldown: 30
  require-confirmation: true
  announcement: true
  divorce-confirmation: true
  divorce-cooldown: 600  # 10 minutes
  marriage-benefits:
    shared-effects: true
    mood-sharing: true
    teleport-to-partner: true
    private-chat: true

# ═══════════════════════════════════════════════════════════════════════════════
#                              ANNIVERSARY SYSTEM
# ═══════════════════════════════════════════════════════════════════════════════

# Anniversary settings
anniversary:
  enabled: true
  announcement-type: "global" # global, couple, world
  announcement-worlds:
    - "world"
  check-interval: 300 # seconds (5 minutes)

# ═══════════════════════════════════════════════════════════════════════════════
#                               MOOD SYSTEM
# ═══════════════════════════════════════════════════════════════════════════════

# Mood system (display only - no effects)
mood:
  enabled: true
  require-marriage: false  # Set to true if only married players can use moods
  partner-notifications: true  # Notify partner when mood changes
  mood-types:
    - "very-good"
    - "good"
    - "neutral"
    - "bad"
    - "very-bad"

# ═══════════════════════════════════════════════════════════════════════════════
#                                GUI SETTINGS
# ═══════════════════════════════════════════════════════════════════════════════

# GUI Settings
gui:
  update-interval: 15
  items-per-page: 28
  animated-items: true
  sound-effects: true
  custom-textures: false

# ═══════════════════════════════════════════════════════════════════════════════
#                              LEADERBOARD SYSTEM
# ═══════════════════════════════════════════════════════════════════════════════

# Leaderboard settings
leaderboard:
  enabled: true
  update-interval: 600  # 10 minutes
  max-entries: 50
  categories:
    - "total-score"
    - "hugs"
    - "kisses"
    - "likes"
    - "marriages"

# ═══════════════════════════════════════════════════════════════════════════════
#                                MISCELLANEOUS
# ═══════════════════════════════════════════════════════════════════════════════

# Debug mode
debug: false

# Auto-save interval (minutes) - saves to YAML files
auto-save: 30

# Update checker configuration
# Checks your SpigotMC resource page for new versions
update-checker:
  enabled: true
  resource-id: 126459
  # How often to check for updates (in hours)
  check-interval: 24


# Permission Messages
NoPermissionMessage: "&cYou do not have permission to use this command."
```


</details>

<details>
<summary>Configuration - lang/en.yml</summary>

```
# ═══════════════════════════════════════════════════════════════════════════════
#                        VALENTINES PLUGIN ver3.0.0-beta
#                          Advanced Valentines Plugin
# ═══════════════════════════════════════════════════════════════════════════════

# ═══════════════════════════════════════════════════════════════════════════════
#                             CONTACT AND SUPPORT
# Website  https://sonemcpl.pages.dev
# Discord: https://sonemcpl.pages.dev/invite
# ═══════════════════════════════════════════════════════════════════════════════

plugin:
  enabled: "&a💝 Valentines v3.0.0 has been enabled! Spread the love! 💝"
  disabled: "&c💔 Valentines plugin has been disabled. See you soon! 💔"
  reload: "&a🔄 Valentines plugin has been reloaded successfully!"
  update-available: "&e⚡ A new version of Valentines is available! Check SpigotMC!"

general:
  no-permission: "&c❌ You don't have permission to use this command!"
  player-offline: "&c❌ That player is not online right now!"
  player-not-found: "&c❌ Player not found or has never played before!"
  partner-offline: "&c💔 Your partner is not online!"
  cooldown: "&c⏰ You can {command} again in &d{time}&c seconds!"
  invalid-world: "&c🌍 This command cannot be used in this world!"
  feature-disabled: "&c❌ This feature is currently disabled!"

help:
  header: "&d❤ &5💝 VALENTINES v3.0.0 COMMANDS 💝 &d❤"
  valentines: "&d/valentines &f- Display help and plugin info"
  valentines-reload: "&d/valentines reload &f- Reload the plugin &7(Admin)"
  gui: "&d/vgui &f- Open the magical Valentines GUI"
  hug: "&d/hug <player> &f- Give someone a warm hug"
  kiss: "&d/kiss <player> &f- Send a sweet kiss"
  like: "&d/like <player> &f- Show appreciation"
  marry: "&d/marry <player> &f- Propose marriage"
  divorce: "&d/divorce &f- End your marriage"
  mood: "&d/mood <mood> &f- Set your current mood"

hug:
  usage: "&c💡 Usage: &d/hug <player>"
  self: "&c🤗 You can't hug yourself! Find someone else to hug!"
  sent: "&f🤗 You gave &d{player} &fa warm, loving hug! &c❤"
  received: "&d{player} &fgave you a wonderful hug! &c❤ &fYou feel loved!"
  broadcast: "&d{sender} &fand &d{receiver} &fshared a heartwarming hug! &c❤"

kiss:
  usage: "&c💡 Usage: &d/kiss <player>"
  self: "&c💋 You can't kiss yourself! That would be weird!"
  sent: "&f💋 You sent &d{player} &fa sweet, tender kiss! &c❤"
  received: "&d{player} &fsent you a magical kiss! &c❤ &fYour heart flutters!"
  broadcast: "&d{sender} &fand &d{receiver} &fshared a romantic kiss! &c❤"

like:
  usage: "&c💡 Usage: &d/like <player>"
  self: "&c👍 You already like yourself! Show love to others!"
  already-liked: "&c❤ You've already shown your appreciation to &d{player}&c!"
  cooldown: "&c⏰ You can show appreciation again in &d{time}&c seconds!"
  sent: "&f👍 You showed &d{player} &fyour appreciation! &c❤"
  received: "&d{player} &fshowed you some love! &c❤ &fYou feel appreciated!"

marry:
  usage: "&c💡 Usage: &d/marry <player> &for &d/marry confirm/deny"
  self: "&c💒 You can't marry yourself! Find your soulmate!"
  proposal-sent: "&f💍 Marriage proposal sent to &d{player}&f! Good luck! 🍀"
  proposal-received: "&d💍 {player} &fwants to marry you! &d💒\n&fType &d/marry confirm &fto accept or &d/marry deny &fto decline."
  already-married: "&c💒 You're already married to &d{partner}&c! One love at a time!"
  target-already-married: "&c💒 {player} is already taken! Find someone else!"
  no-pending-proposals: "&c💍 You have no pending marriage proposals!"
  proposer-offline: "&c💔 The person who proposed is no longer online!"
  proposal-cooldown: "&c⏰ You can propose again in &d{time}&c seconds!"
  accept-sender: "&a💒 {player} &aaccepted your proposal! You're now married! &d💕"
  accept-receiver: "&a💒 You married &d{player}&a! Welcome to married life! &d💕"
  decline-sender: "&c💔 {player} declined your proposal. Don't give up on love!"
  decline-receiver: "&c💔 You declined &d{player}'s &cproposal."
  divorce-initiator: "&c💔 You have divorced &d{player}&c. Sometimes love fades..."
  divorce-target: "&c💔 {player} &chas divorced you. Stay strong!"
  divorce-confirm: "&e⚠️ Are you sure you want to divorce &d{player}&e? Type &d/divorce confirm &eto proceed."
  not-married: "&c💔 You're not married! Find your soulmate first!"
  not-married-to: "&c💔 You're not married to &d{player}&c!"
  announcement: "&d💒 &5WEDDING BELLS! &d💒 &f{player1} &fand &d{player2} &fjust got married! &d💕 Congratulations!"
  divorce-announcement: "&c💔 {player1} &fand &c{player2} &fhave divorced. Love is complicated..."

anniversary:
  global-announcement: "&d💒 &5ANNIVERSARY CELEBRATION! &d💒 &f{player1} &fand &d{player2} &fcelebrate &d{years} &fyear(s) of marriage! &d💕"
  couple-message: "&d💒 &5Happy Anniversary! &d💒 &fYou and &d{partner} &fhave been married for &d{years} &fyear(s)! &d💕"
  world-announcement: "&d💒 &f{player1} &fand &d{player2} &fcelebrate their &d{years} &fyear anniversary! &d💕"

mood:
  not-married: "&c💔 You must be married to share your mood!"
  updated: "&f😊 Your mood has been updated to: &d{mood}"
  partner-notified: "&f💕 Your partner has been notified of your mood change!"
  partner-mood-changed: "&f💕 Your partner &d{partner} &fis now feeling: &d{mood}"
  unknown: "&7❓ Unknown"
  very-good: "&a😄 Very Good"
  good: "&e😊 Good"
  neutral: "&f😐 Neutral"
  bad: "&c😞 Bad"
  very-bad: "&4😢 Very Bad"

stats:
  usage: "&c💡 Usage: &d/valentinesplayer <player>"
  header: "&5💝 {player}'s Valentine Stats 💝"
  kisses: "&d💋 Kisses received: &f{count}"
  hugs: "&d🤗 Hugs received: &f{count}"
  likes: "&d👍 Likes received: &f{count}"
  married: "&d💒 Married to: &f{partner} &d(for {days} days)"
  single: "&d💔 Relationship status: &fSingle and ready to mingle!"
  total-score: "&d⭐ Total Love Score: &f{score}"
  mood: "&d😊 Current mood: &f{mood}"

leaderboard:
  header: "&5💝 Valentine Leaderboard 💝"
  entry: "&a#{rank} &d{player} &f- &d{score} &fpoints &7(&d{kisses}&f💋 &d{hugs}&f🤗 &d{likes}&f👍&7)"
  empty: "&c📊 No players found on the leaderboard yet!"

marriages:
  header: "&5💒 Married Couples 💒"
  couple: "&f💕 &d{player1} &f& &d{player2} &f- &d{days} &fdays together"
  none: "&d💔 There are no married couples on the server yet!"

player-search:
  prompt: "&f🔍 Please type the name of the player you want to search for:"
  not-found: "&c❌ Player '{player}' not found or is not online!"
  searching: "&f🔍 Searching for player: &d{player}&f..."

gui:
  main-menu-title: "&d❤ Valentines Menu ❤"
  stats-menu-title: "&d❤ &5📊 Player Stats 📊 &d❤"
  leaderboard-title: "&d❤ &5🏆 Love Leaderboard 🏆 &d❤"
  marriages-title: "&d❤ &5💒 Married Couples 💒 &d❤"
  settings-title: "&d❤ &5⚙️ Effect Settings ⚙️ &d❤"
  mood-title: "&d❤ &5😊 Mood Settings 😊 &d❤"
  player-profile-title: "&d❤ &5{player}'s Profile &d❤"

  stats-button-title: "&d📊 Your Stats"
  stats-button-lore:
    - "&fView your love statistics"
    - "&7See how much love you've received!"
  leaderboard-button-title: "&d🏆 Leaderboard"
  leaderboard-button-lore:
    - "&fSee the most loved players"
    - "&7Compete for the top spot!"
  marriages-button-title: "&d💒 Married Couples"
  marriages-button-lore:
    - "&fView all marriages on the server"
    - "&7See who found their soulmate!"
  settings-button-title: "&d⚙️ Settings"
  settings-button-lore:
    - "&fCustomize your particle effects"
    - "&7Make your love visible!"
  mood-button-title: "&d😊 Mood"
  mood-button-lore:
    - "&fSet your current mood"
    - "&7Let others know how you feel!"
  player-search-button-title: "&d🔍 Player Search"
  player-search-button-lore:
    - "&fSearch for other players"
    - "&7Find and interact with players!"

  hugs-title: "&d🤗 Hugs Received"
  hugs-lore:
    - "&fYou've received &d{count} &fwarm hugs"
    - "&7Everyone loves your hugs!"
  kisses-title: "&d💋 Kisses Received"
  kisses-lore:
    - "&fYou've received &d{count} &fsweet kisses"
    - "&7You're quite the charmer!"
  likes-title: "&d👍 Likes Received"
  likes-lore:
    - "&fYou've received &d{count} &flikes"
    - "&7People really appreciate you!"
  marriage-title: "&d💒 Marriage Status"
  marriage-lore:
    - "&fYou are married to &d{partner}"
    - "&fFor &d{days} &fdays"
    - "&7True love never dies!"
  single-title: "&d💔 Relationship Status"
  single-lore:
    - "&fYou are currently single"
    - "&7Your soulmate is out there!"
  mood-display-title: "&d😊 Your Mood"
  mood-display-lore:
    - "&fCurrent mood: &d{mood}"
    - "&7Let others know how you feel!"

  leaderboard-entry-title: "&a#{rank} &d{player}"
  leaderboard-entry-lore:
    - "&fTotal Love Score: &d{score}"
    - "&fHugs: &d{hugs}"
    - "&fKisses: &d{kisses}"
    - "&fLikes: &d{likes}"

  marriage-couple-title: "&d{player1} &f💕 &d{player2}"
  marriage-couple-lore:
    - "&fMarried since: &d{date}"
    - "&fDays together: &d{days}"
    - "&7A beautiful love story!"

  # Player profile buttons
  hug-button-title: "&d🤗 Hug {player}"
  hug-button-lore:
    - "&fGive them a warm hug"
    - "&7Show your affection!"
  kiss-button-title: "&d💋 Kiss {player}"
  kiss-button-lore:
    - "&fSend them a sweet kiss"
    - "&7Express your love!"
  like-button-title: "&d👍 Like {player}"
  like-button-lore:
    - "&fShow your appreciation"
    - "&7Let them know you care!"
  marry-button-title: "&d💒 Marry {player}"
  marry-button-lore:
    - "&fPropose marriage"
    - "&7Take the next step in love!"

  # Mood system (display only)
  mood-very-good-title: "&a😄 Very Good"
  mood-very-good-lore:
    - "&fSet your mood to Very Good"
    - "&7You're feeling amazing!"
  mood-good-title: "&e😊 Good"
  mood-good-lore:
    - "&fSet your mood to Good"
    - "&7You're doing well!"
  mood-neutral-title: "&f😐 Neutral"
  mood-neutral-lore:
    - "&fSet your mood to Neutral"
    - "&7You're feeling okay!"
  mood-bad-title: "&c😞 Bad"
  mood-bad-lore:
    - "&fSet your mood to Bad"
    - "&7You need some support!"
  mood-very-bad-title: "&4😢 Very Bad"
  mood-very-bad-lore:
    - "&fSet your mood to Very Bad"
    - "&7You really need help!"

  partner-mood-title: "&d💕 {partner}'s Mood"
  partner-mood-lore:
    - "&fCurrent mood: &d{mood}"
    - "&7Check on your partner!"

  effect-spiral: "&d🌀 Spiral Effect"
  effect-heart: "&d❤ Heart Effect"
  effect-cloud: "&d☁ Cloud Effect"
  effect-selected: "&a✓ Selected"
  effect-disabled: "&c❌ Disabled"

  back-button: "&c⬅ Back"
  prev-page-button: "&a⬅ Previous Page"
  next-page-button: "&a➡ Next Page"
  page-info: "&fPage &d{current}&f/&d{total}"
  close-button: "&c❌ Close Menu"

# ═══════════════════════════════════════════════════════════════════════════════
#                                SOUND EFFECTS
# ═══════════════════════════════════════════════════════════════════════════════

sounds:
  hug: "ENTITY_PLAYER_LEVELUP"
  kiss: "ENTITY_EXPERIENCE_ORB_PICKUP"
  like: "ENTITY_VILLAGER_YES"
  marry: "ENTITY_FIREWORK_ROCKET_LAUNCH"
  divorce: "ENTITY_VILLAGER_NO"
  mood-change: "BLOCK_NOTE_BLOCK_CHIME"
```

</details>



## Images
![image1](https://github.com/SoneMC/images/raw/main/valentines_images/image1.png)
![image2](https://github.com/SoneMC/images/raw/main/valentines_images/image2.png)
![image3](https://github.com/SoneMC/images/raw/main/valentines_images/image3.png)
![image4](https://github.com/SoneMC/images/raw/main/valentines_images/image4.png)
![image5](https://github.com/SoneMC/images/raw/main/valentines_images/image5.png)
![image6](https://github.com/SoneMC/images/raw/main/valentines_images/image6.png)

---

## Versions:

- Built for: **1.20.2**
- Tested versions: **1.20.2, 1.21.6**
- Should work on: **1.21.6+**

> Note: Versions that "Should work on: ..." are **NOT** tested and there **may** be some problems with plugin(s).

---

## Useful Links

- **Discord**: [Invite](https://sonemcpl.pages.dev/invite)
- **GitHub**: [Look](https://github.com/SoneMC)
- **Website**: [Look](https://sonemcpl.pages.dev)
- **License**: [MIT](https://github.com/SoneMC/SoneMC/raw/main/LICENSE)

---
