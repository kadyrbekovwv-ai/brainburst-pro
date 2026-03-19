# 🧠 BrainBurst Pro — Quiz Game

**The World's Smartest Quiz App**  
Single-file HTML/CSS/JS • 8 Languages • 4500+ Questions • PWA Ready

---

## 📋 What's Included

- `index.html` — Complete app (all code, styles, and questions in one file)
- 8 interface languages: English, Russian, Chinese, Hindi, Portuguese, French, Turkish, Kyrgyz
- 4500+ questions across 13 categories
- Firebase-powered: real-time chat, battle mode, global leaderboard
- PWA support (installable on Android/iOS)

---

## ⚙️ Setup (Required)

### Step 1 — Firebase Setup

1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Click **"Add project"** → enter a name → **Continue**
3. Disable Google Analytics (optional) → **Create project**
4. In the left menu: **Build → Realtime Database → Create database**
5. Choose region (e.g. `europe-west1`) → **Next**
6. Select **"Start in test mode"** → **Enable**
7. Copy your database URL (e.g. `https://your-project-default-rtdb.europe-west1.firebasedatabase.app`)

### Step 2 — Update Firebase URL in index.html

Open `index.html` in any text editor and find this line near the top of the `<script>` section:

```javascript
const FIREBASE_BASE_URL = 'https://brainburst-pro-default-rtdb.europe-west1.firebasedatabase.app';
```

Replace it with your own Firebase URL:

```javascript
const FIREBASE_BASE_URL = 'https://YOUR-PROJECT-default-rtdb.YOUR-REGION.firebasedatabase.app';
```

### Step 3 — Firebase Security Rules

In Firebase Console → **Realtime Database → Rules**, paste:

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

Click **Publish**.

---

## 🚀 Deployment

### GitHub Pages (Free)

1. Create a GitHub account at [github.com](https://github.com)
2. Create a new repository (e.g. `brainburst-pro`)
3. Upload `index.html` to the repository
4. Go to **Settings → Pages → Source → Deploy from branch → main**
5. Your app is live at: `https://YOUR-USERNAME.github.io/brainburst-pro`

### Any Web Hosting

Upload `index.html` to any hosting (Netlify, Vercel, etc.)  
No server-side code required — it's a single file.

---

## 🎮 Features

| Feature | Description |
|---------|-------------|
| 📝 Classic Mode | 15 questions per session |
| ⏱️ Timed Mode | 15 seconds per question |
| 🏃 Marathon Mode | All questions in one session |
| 💀 Sudden Death | One mistake = game over (PRO) |
| ⚔️ Battle Mode | Real-time online 1v1 (Firebase) |
| 🤜 Duel Mode | Two players, one phone |
| 💬 Global Chat | Real-time chat by country (Firebase) |
| 🏆 Leaderboard | Global & country rankings (Firebase) |
| 🎯 Daily Quests | Earn coins every day |
| ❤️ Lives System | Lose a life on wrong answer |
| 🪙 Coins | Earn and spend in-game |
| 👑 PRO System | Unlock all categories |

---

## 🌍 Languages & Questions

| Language | Questions |
|----------|-----------|
| 🇷🇺 Russian | 652 |
| 🇬🇧 English | 613 |
| 🇨🇳 Chinese | 601 |
| 🇧🇷 Portuguese | 576 |
| 🇰🇬 Kyrgyz | 576 |
| 🇫🇷 French | 553 |
| 🇮🇳 Hindi | 526 |
| 🇹🇷 Turkish | 521 |

---

## 📂 Categories (13)

Capitals • Mathematics • Science • Space • History • Animals  
Sports • Culture • Food • Technology • Music • Geography • Misc

---

## 🛠️ Tech Stack

- **Frontend:** Vanilla HTML/CSS/JavaScript (no frameworks)
- **Database:** Firebase Realtime Database
- **Hosting:** Any static hosting (GitHub Pages recommended)
- **No build step required** — just open index.html

---

## ⚠️ Important Notes

- Firebase is required for: Chat, Battle mode, Leaderboard, Online presence
- Without Firebase: all quiz modes, XP system, achievements, and lives still work
- Firebase free tier (Spark plan) is sufficient for most use cases
- For production use, consider adding Firebase Authentication for better security

---

## 📄 License

This source code is sold as-is. You may modify and use it for your own projects.  
Reselling the original source code without modification is not permitted.

---

*BrainBurst Pro — Built with ❤️*
