<div align="center">

# 📱 ReelWise — Reels Counter

### *Track. Limit. Take Control.*

**ReelWise** is an Android digital-wellbeing app that helps you understand and manage your short-form video scrolling habits — across **Instagram Reels, Facebook Reels, YouTube Shorts, TikTok, and Snapchat Spotlight**.

Set daily limits, get alerts or blocks when you hit them, and turn raw scrolling into statistics, goals, streaks, challenges, and rankings.

<a href="https://play.google.com/store/apps/details?id=com.dvexo.reelguard">
  <img src="https://img.shields.io/badge/Google%20Play-Download%20ReelWise-0A6C64?style=for-the-badge&logo=google-play&logoColor=white" alt="Download on Google Play">
</a>

<br><br>

<img src="assets/images/reelwise-banner.png" alt="ReelWise Banner" width="1024">

</div>

<br>

## 📑 Table of Contents

- [About ReelWise](#-about-reelwise)
- [Key Features](#-key-features)
- [Statistics & Analytics](#-statistics--analytics)
- [Goals, Challenges & Streaks](#-goals-challenges--streaks)
- [Leaderboards & Rankings](#-leaderboards--rankings)
- [Privacy & Data](#-privacy--data)
- [How ReelWise Works](#-how-reelwise-works)
- [Screenshots](#-app-screenshots)
- [Technology](#️-technology)
- [Architecture](#️-architecture)
- [Permissions & Accessibility](#️-permissions--accessibility)
- [Supported Platforms](#-supported-platforms)
- [Product Design](#-product-design)
- [Third-Party Services](#-third-party-services)
- [Get ReelWise](#-get-reelwise)
- [Product Vision](#️-product-vision)
- [Future Improvements](#-future-improvements)
- [Privacy Policy](#-privacy-policy)
- [Contact & Support](#-contact--support)

---

## ✨ About ReelWise

Short-form videos are engineered to keep you scrolling. ReelWise takes a different approach to digital wellbeing — instead of only measuring **how much time** you spend in an app, it measures **how many Reels and Shorts you actually scroll through**.

With ReelWise, you can:

| | |
|---|---|
| 📊 | Track your Reels and Shorts |
| 🎯 | Set daily scrolling limits |
| 🔔 | Receive alerts when your limit is reached |
| 🛑 | Block further short-form scrolling after your limit |
| 📈 | Analyze detailed scrolling statistics |
| 📅 | Review your activity history |
| 📱 | See platform-specific activity breakdowns |
| 🏆 | Maintain streaks and complete challenges |
| 🎯 | Set and track personal goals |
| 🌎 | Explore aggregate leaderboard rankings |
| 🔐 | Use optional account and cloud features |

> **Know your scrolling. Set your limits. Take control.**

---

## 🚀 Key Features

### 📊 Reel & Shorts Counter

ReelWise automatically detects supported short-form scrolling activity and keeps a running daily count.

| Platform | Supported Content |
|---|---|
| 📸 Instagram | Reels |
| 🔵 Facebook | Reels |
| ▶️ YouTube | Shorts |
| 🎵 TikTok | Short-form Videos |
| 👻 Snapchat | Spotlight |

> Counting behavior may vary depending on the installed version of each third-party app and your Android version.

### 🎯 Daily Scrolling Limits

Set your own daily Reel/Short limit — for example, **100 Reels a day** — and monitor your progress toward it in real time.

### 🔔 Limit Alerts

Get notified the moment you hit your configured daily limit, so you can pause and decide whether to keep scrolling.

### 🛑 Scrolling Limit Blocking

Want stronger control? Blocking mode restricts further supported scrolling once your daily limit is reached.

| Mode | Behavior |
|---|---|
| **Alert Mode** | Reach limit → Get notified → Decide what to do |
| **Block Mode** | Reach limit → Further scrolling is blocked |

---

## 📈 Statistics & Analytics

ReelWise turns raw scrolling activity into clear, understandable statistics:

- Daily Reel/Short count
- Scrolling trends over time
- Platform-specific activity
- Historical activity logs
- Goal and limit progress
- Long-term behavior changes

Instead of guessing how much you scroll, you can actually see the numbers.

### 📅 History

Reviewing past activity helps you spot:

- High-scrolling days
- Progress toward your limits
- Day-to-day behavior changes
- Platform-specific patterns
- Long-term consistency

---

## 🏆 Goals, Challenges & Streaks

A motivational layer on top of your raw data:

| Feature | Description |
|---|---|
| 🎯 **Goals** | Create personal targets and track your progress |
| 🔥 **Streaks** | Build consistency across multiple days |
| 🏅 **Challenges** | Take part in challenges built around your scrolling goals |

The idea isn't just to count numbers — it's to turn those numbers into actionable habits.

---

## 🌎 Leaderboards & Rankings

Where enabled, ReelWise offers aggregate ranking features:

- 🌍 Global rankings
- 🇧🇩 Country-based rankings
- 📱 Platform-based rankings
- 📈 Rank history

> Leaderboards rely on aggregate statistics only — ReelWise never needs access to your social-media account credentials.

---

## 🔐 Privacy & Data

Privacy and data minimization are core design principles behind ReelWise.

ReelWise uses Android's **AccessibilityService** solely to recognize supported scrolling activity for its counting and control features. It is **not** intended to collect unrelated content from the apps you use.

**ReelWise does not require:**
- Your Instagram, Facebook, or YouTube password

**ReelWise's counting system is not intended to collect or upload:**
- Screenshots or screen recordings
- Video or audio files
- Captions, comments, or direct messages
- Passwords
- General third-party app content

Optional account features (sync, aggregate stats) use **Firebase Authentication** and cloud services. Advertising is served through **Google Mobile Ads (AdMob)**.

📄 Full details are available in the [Privacy Policy](#-privacy-policy).

---

## 🧩 How ReelWise Works

```text
Supported Social App
        │
        ▼
Android AccessibilityService
        │
        ▼
Detect Supported Short-Form Content
        │
        ▼
Count Scrolling Activity
        │
        ├──────────────► Daily Limit
        │                    │
        │                    ├── Alert
        │                    └── Block
        │
        ▼
Local Activity Data
        │
        ▼
Statistics & History
        │
        ├── Goals
        ├── Challenges
        ├── Streaks
        └── Rankings
```

---

## 📱 App Screenshots

<div align="center">

| Home Dashboard | Statistics | Platform Stats | Daily Limits | Leaderboard |
|:---:|:---:|:---:|:---:|:---:|
| <img src="assets/screenshots/home.png" width="160"> | <img src="assets/screenshots/statistics.png" width="160"> | <img src="assets/screenshots/platform-stats.png" width="160"> | <img src="assets/screenshots/daily-limit.png" width="160"> | <img src="assets/screenshots/leaderboard.png" width="160"> |
| Quick overview of activity, progress & limits | Explore trends via statistics & history | See usage distributed across platforms | Configure limits & response behavior | Aggregate rankings & position over time |

</div>

---

## 🛠️ Technology

| Technology | Purpose |
|---|---|
| **Kotlin** | Primary programming language |
| **Jetpack Compose** | Modern declarative UI |
| **MVVM / Clean Architecture** | Application architecture |
| **StateFlow / Flow** | Reactive state and data streams |
| **Room** | Local database |
| **DataStore** | Local preferences and settings |
| **Hilt** | Dependency injection |
| **Retrofit / OkHttp** | Network communication |
| **Firebase Authentication** | Optional account authentication |
| **Firebase Realtime Database** | Cloud/aggregate data |
| **WorkManager** | Background tasks |
| **Android AccessibilityService** | Reel/Short detection and control |
| **Google Mobile Ads / AdMob** | In-app advertising |

---

## 🏗️ Architecture

```text
┌─────────────────────────────┐
│     Jetpack Compose UI      │
└──────────────┬──────────────┘
               ▼
┌─────────────────────────────┐
│   ViewModel (UI State /     │
│         Events)             │
└──────────────┬──────────────┘
               ▼
┌─────────────────────────────┐
│  Use Cases / Domain Logic   │
└──────────────┬──────────────┘
               ▼
┌─────────────────────────────┐
│  Repository (Data Layer)    │
└───────┬───────────┬─────────┘
        ▼           ▼
   Local Data    Remote Data
  (Room/DataStore) (Firebase/API)
```

> 📌 This repository serves as a **product showcase**. Application source code is not publicly distributed here.

---

## ⚙️ Permissions & Accessibility

ReelWise requires **Android Accessibility access** for its core tracking and control functionality.

**Why is this required?** Android doesn't expose a public API that tells an app how many Reels or Shorts a user has scrolled through inside another app. ReelWise's AccessibilityService fills this gap by recognizing supported UI activity needed for counting.

Users remain fully in control and can enable or disable Accessibility access anytime via Android Settings.

---

## 📲 Supported Platforms

| Platform | Content Type |
|---|---|
| **Instagram** | Reels |
| **Facebook** | Reels |
| **YouTube** | Shorts |
| **TikTok** | Short-form Videos |
| **Snapchat** | Spotlight |

> Third-party UIs change over time — detection accuracy may vary by app version, Android version, and platform updates.

---

## 🎨 Product Design

ReelWise follows a clean, modern digital-wellbeing visual language.

**Primary Palette**

| Color | Hex |
|---|---|
| 🟢 Primary Teal | `#0A6C64` |
| 🔵 Dark Navy | `#0F172A` |

Design principles:
- Clear information hierarchy
- Minimal visual clutter
- Easy-to-read statistics
- Fast access to daily limits
- Modern Android UI patterns
- Consistent cards and components
- Accessible, readable typography

---

## 🔒 Third-Party Services

| Service | Purpose |
|---|---|
| **Firebase** | Optional authentication and cloud functionality |
| **Google Mobile Ads / AdMob** | In-app advertisements |
| **Google Play Services** | Required Android/Google service integrations |

> ReelWise is independently developed and is **not affiliated with, sponsored by, endorsed by, or officially connected to** Instagram, Facebook, YouTube, Meta, or Google. All third-party names and trademarks belong to their respective owners.

---

## 📥 Get ReelWise

<div align="center">

<a href="https://play.google.com/store/apps/details?id=com.dvexo.reelguard">
  <img src="https://img.shields.io/badge/Download%20on-Google%20Play-0A6C64?style=for-the-badge&logo=google-play&logoColor=white" alt="Download ReelWise">
</a>

**`https://play.google.com/store/apps/details?id=com.dvexo.reelguard`**

</div>

---

## 🗺️ Product Vision

ReelWise started with a simple question:

> **How many Reels and Shorts do we actually scroll through every day?**

Traditional screen-time metrics tell you how long an app was open — but not what actually happened during that time. ReelWise focuses on the short-form content itself, combining:

**Tracking → Limits → Alerts → Blocking → Statistics → Goals → Streaks → Challenges**

...to help users become more aware of their scrolling and make more intentional decisions about where their attention goes.

---

## 🔮 Future Improvements

- Additional supported short-form platforms
- More detailed analytics
- More customizable goals
- Additional challenge types
- Expanded ranking features
- Improved detection reliability
- Additional digital-wellbeing tools
- More personalization options

> Feature availability may change as the application evolves.

---

## 📄 Privacy Policy

For details on data handling, permissions, third-party services, retention, and deletion, please see the official ReelWise Privacy Policy:

🔗 **[abdullahalnuman-dev.github.io/reel-wise](https://abdullahalnuman-dev.github.io/reel-wise)**

---

## 💬 Contact & Support

Have a question, found a bug, or want to suggest a feature?

| Channel | Contact |
|---|---|
| 💬 WhatsApp | [+880 1754-155296](https://wa.me/+8801754155296) |
| 📧 Email | [abdullahalnumanb@gmail.com](mailto:abdullahalnumanb@gmail.com) |
| 🌐 Google Play | [Download ReelWise](https://play.google.com/store/apps/details?id=com.dvexo.reelguard) |

---

## ⭐ Support ReelWise

If ReelWise helps you become more aware of your scrolling habits, consider:

- ⭐ Starring the project on GitHub
- 📱 Trying the app on Google Play
- 💬 Sharing your feedback
- 🐛 Reporting issues
- 💡 Suggesting new features

<div align="center">

### ReelWise: Reels Counter
**Track. Limit. Take Control.**

*Built with ❤️ for a more intentional digital life.*

© 2026 ReelWise. All rights reserved.

</div>