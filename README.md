<a name="top"></a>
<div align="center">
	<img src="https://ik.imagekit.io/3xnpqon35/clnstkr_banner.png" alt="ClonStoker Banner" width="800">
	<br>
	<br>
	<p><b>🛡️ Discord Server Backup, Restoration & Replication Tool</b></p>
	<p><i>Clone entire Discord servers — channels, roles, messages, emojis & more.</i></p>
	<p><sub>Developed by <b>SilentRoot</b></sub></p>
	<hr/>
	<br>
	<a href="https://github.com/silentrootx/DC-Cloner/stargazers">
		<img src="https://img.shields.io/github/stars/silentrootx/ClonStoker?label=%E2%AD%90%20STARS&logoColor=white&labelColor=1C2325&color=fab387&style=for-the-badge">
	</a>
	<a href="https://github.com/silentrootx/DC-Cloner/issues">
		<img src="https://img.shields.io/github/issues/silentrootx/ClonStoker?label=%F0%9F%90%9B%20ISSUES&logoColor=white&labelColor=1C2325&color=ffb29b&style=for-the-badge">
	</a>
	<a href="./LICENSE">
		<img src="https://img.shields.io/badge/📜_License-Own-FCA2AA?labelColor=1C2325&style=for-the-badge">
	</a>
	<a href="https://www.python.org/downloads/">
		<img src="https://img.shields.io/badge/🐍_Python-3.10+-C9CBFF?labelColor=1C2325&style=for-the-badge">
	</a>
	<br>
	<br>

---

[About](#about) • [Features](#features) • [Preview](#preview) • [Installation](#setup) • [Commands](#commands) • [Security](#security) • [License](#license) • [Contact](#contact)

<br>
</div>

## <a name="about"></a>📝 About

**ClonStoker** is a powerful Discord bot that lets you create **full backups** of your servers and **restore** them anywhere — including roles, channels, categories, emojis, server settings, and even **complete message history** with author names and attachments.

It also includes a **Server Replicator** module that can clone a remote server you're a member of into a portable backup file, all from within Discord itself.

> [!WARNING]
> **Use at your own risk.** This tool is provided for **educational & research purposes only.**
> Users are solely responsible for ensuring compliance with Discord's Terms of Service.

<br>

## <a name="features"></a>🚀 Features

<div align="center">

| Feature | Description |
|:---|:---|
| 🎭 **Role Backup** | Saves all roles with colors, permissions, hierarchy & mentionability |
| 📁 **Category Backup** | Preserves category structure, positions & permission overwrites |
| 💬 **Channel Backup** | Text, Voice, Forum, Stage channels with topics, slowmode & overwrites |
| 💾 **Message History** | Up to 1000 messages per channel with author names, embeds & attachments |
| 😀 **Emoji Backup** | All custom emojis backed up and restored |
| ⚙️ **Server Settings** | Name, icon, banner, verification level & content filter |
| 🔄 **Full Restore** | One-click restoration with interactive UI and live progress |
| 🌐 **Remote Cloning** | Clone any server you're in via the Replicator module |
| 📡 **Live Progress** | Real-time embed updates showing cloning progress |
| 🛡️ **Token Security** | Auto-deletion of sensitive messages, memory scrubbing |

</div>

<br>

## <a name="preview"></a>🖥️ Preview

### 🔄 Bot Startup
```
🔄 Starting Clonstoker — Server Backup Bot...
[11:33:13] [SYSTEM] 📡 Setting up Intents (Content: True)
[11:33:17] [SYSTEM] 🚀 Logged in as <bot_name> (ID: <bot_id>)
[11:33:17] [SYSTEM] 📡 Intents - Message Content: ✅ ON
[11:33:17] [SYSTEM] 📡 Intents - Server Members: ✅ ON
[11:33:17] [SYSTEM] 📂 Guilds connected: 4
[11:33:17] [SYSTEM]   • My Server (150 members)
[11:33:17] [SYSTEM]   • Test Server (6 members)
[11:33:17] [SYSTEM] === BOT READY ===
```

### 📦 Backup Flow
```
[12:01:05] [CMD] !backup triggered by User#1234
[12:01:06] [BACKUP] 🎭 Backing up 15 roles...
[12:01:06] [BACKUP]   ✅ Role: Admin (pos: 10, color: #e74c3c)
[12:01:06] [BACKUP]   ✅ Role: Moderator (pos: 8, color: #3498db)
[12:01:07] [BACKUP] 📁 Backing up 5 categories...
[12:01:07] [BACKUP]   ✅ Category: General (pos: 0)
[12:01:07] [BACKUP]   ✅ Category: Voice Channels (pos: 1)
[12:01:08] [BACKUP] 💬 Backing up 12 channels with messages...
[12:01:15] [BACKUP] ✅ Saved: backup_20260306_120105.json (245.3 KB)
```

### 🌐 Server Replicator (Live Progress)
```
═════════════════════════════════════════════════════
   ClonStoker — Server Replicator Module
   Use at your own risk.
   For educational & research purpose only.
═════════════════════════════════════════════════════
Logged in safely as User
Auto-starting export for provided guild ID: 1234567890
Starting export of My Server...
Fetching roles...
Fetching categories...
Fetching channels and messages (max 1000 per channel)...
  ⏳ Waiting 2.1s before fetching #general to avoid anti-spam bans...
  Saved # 💬 general (45 msgs)
  ⏳ Waiting 1.8s before fetching #announcements...
  Saved # 💬 announcements (12 msgs)
✅ EXPORT COMPLETE: backups/replicate_1234567890_20260306.json
Auto-export complete. Shutting down replicator.
```

### 🔁 Restore Flow
```
[12:05:30] [RESTORE] Starting restore from: backup_20260306_120105.json
[12:05:31] [RESTORE] 🎭 Restoring 15 roles...
[12:05:32] [RESTORE]   ✅ Role created: Admin (pos: 10)
[12:05:32] [RESTORE]   ✅ Role created: Moderator (pos: 8)
[12:05:33] [RESTORE] 📁 Restoring 5 categories...
[12:05:34] [RESTORE] 💬 Restoring 12 channels...
[12:05:40] [RESTORE]   ✅ Channel created: #general (text)
[12:05:41] [RESTORE]   📨 Restoring 45 messages in #general...
[12:06:15] [RESTORE] ✅ Restore complete!
```

<br>

### Setup

```bash
# 1. Clone the repository
git clone https://github.com/silentrootx/<soon>.git
cd <soon>

# 2. Install dependencies
pip install -r requirements.txt

# 3. Configure your bot token in bot.py
# Edit the BOT_TOKEN variable with your token

# 4. Run the bot
python bot.py
```

### Replicator Module (Optional)
The replicator uses a separate environment to avoid library conflicts:

```bash
# Create isolated environment
python -m venv venv_replicate

# Activate it
.\venv_replicate\Scripts\Activate.ps1   # Windows
source venv_replicate/bin/activate       # Linux/Mac

# Install self-bot library
pip install -r requirements_replicate.txt

# Deactivate (the bot will use it automatically)
deactivate
```

> [!NOTE]
> If the `venv_replicate` folder doesn't exist, the bot will automatically use your global Python installation instead.

<br>

## <a name="commands"></a> >_ Commands

<div align="center">

### 👑 Server Owner Required

| Command | Description |
|:---|:---|
| `!backup` | Open the full server backup menu |
| `!backup structure` | Fast structure-only backup (no messages) |
| `!backup delete` | Select and remove old backup files |
| `!autobackup` | Schedule daily or weekly automated backups |
| `!restore` | Open the interactive restoration menu |
| `!replicate` | Clone a remote server via the Replicator wizard |
| `!export` | Download a backup JSON file directly to your PC |
| `!wipe` | Dangerously clear specific server components |
| `!prefix <new>` | Change the bot's command prefix |

### ☠️ Administrator Required

| Command | Description |
|:---|:---|
| `!import` | Upload a backup JSON file to the bot |
| `!backup inspect` | View detailed stats and contents of a backup |
| `!backups` | List all locally stored backup files |
| `!clear <amount>` | Purge messages from the current channel |
| `!help` | Show the dynamic command reference menu |

### 🛠️ Utility & Debug

| Command | Description |
|:---|:---|
| `!check_intents` | Verify bot permissions and Gateway Intents |
| `!debug_msg <id>` | Dump raw attributes of a specific message |
| `!test_restore <id>`| Preview how a message will look when restored |

</div>

<br>

## <a name="security"></a>🔐 Security

ClonStoker takes security seriously:

| Protection | How It Works |
|:---|:---|
| 🗑️ **Auto-Delete** | User messages containing tokens are instantly deleted |
| 🛡️ **Log Masking** | Tokens are replaced with `********[HIDDEN_TOKEN]********` in live logs |
| 🧹 **Memory Scrub** | Token and Server ID are explicitly wiped from RAM after use |
| 🔒 **Owner-Only** | Sensitive commands restricted to server owner |
| 🏷️ **Tamper-Proof Branding** | Multi-layer integrity verification prevents unauthorized modifications |

<br>

## 🏗️ Project Structure

```
ClonStoker/
├── 📄 bot.py                     # Main Discord bot
├── 📄 replicate.py               # Server cloner module (self-bot)
├── 📄 requirements.txt           # Bot dependencies
├── 📄 requirements_replicate.txt # Replicator dependencies
├── 📄 LICENSE                    # Project license
├── 📄 README.md                  # This file
└── 📁 backups/                   # Backup JSON files (auto-created)
```

<br>

## 🎨 Built With

<div align="center">

<a href="https://www.python.org/">
	<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
</a>
<a href="https://discordpy.readthedocs.io/">
	<img src="https://img.shields.io/badge/discord.py-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="discord.py">
</a>
<a href="https://docs.aiohttp.org/">
	<img src="https://img.shields.io/badge/aiohttp-2C5BB4?style=for-the-badge&logo=aiohttp&logoColor=white" alt="aiohttp">
</a>

</div>

<br>

## <a name="license"></a>📜 License
<div align="left">
	
This project is licensed under a **Custom License** — see the [LICENSE](LICENSE) file for details.

**ClonStoker** | Use at your own risk. For educational & research purpose only.
<br>

<br>
<div align="center">
  <img src="https://img.shields.io/badge/DEVELOPER-SILENT_ROOT-blue?color=262626&labelColor=5865F2&style=for-the-badge" height="30">
</div>

<br>

## <a name="contact"></a>💬 Connect & Support

If you encounter any issues, have feature requests, or just want to chat about the project, feel free to join our community!

<div align="left">
  <a href="https://discord.gg/2HuaTEk9J3">
    <img src="https://img.shields.io/badge/DISCORD-blue?color=5865F2&labelColor=5865F2&logo=discord&logoColor=white&style=for-the-badge">
  </a>
</div>
<br>


## 💰 Support the Project

If you find this tool useful and want to support its development, donations are greatly appreciated!

![Bitcoin](https://img.shields.io/badge/Bitcoin-f7931a?style=for-the-badge&logo=bitcoin&logoColor=white&labelColor=1C2325)

**Bitcoin Address:**
```text
bc1q2gju5zc9jnn0zhfhdhza4vxm5zft26eew55jju
```

![Litecoin](https://img.shields.io/badge/Litecoin-345d9d?style=for-the-badge&logo=litecoin&logoColor=white&labelColor=1C2325)

**Litecoin Address:**
```text
LfmZJoJt6R2dM3TqWu27PzQfRn9T9ozPfD
```

<br>
<div align="center">
<a href="#top">
	<img src="https://img.shields.io/badge/⬆_Back_to_Top-1C2325?style=for-the-badge">
</a>
</div>






















