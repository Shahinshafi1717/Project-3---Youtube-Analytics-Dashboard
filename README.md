# 📊 YouTube Analytics Dashboard

A real-time YouTube channel analytics dashboard built with **pure HTML, CSS, and JavaScript** — no frameworks, no build tools, no dependencies. Just open and run.

Built as part of the **Hex Softwares Internship Project** by **Shain Shafi**.

---

## 🖥️ Live Preview

> Glassmorphism UI with dark/light theme, animated SVG charts, and live YouTube data.

---

## ✨ Features

- 📺 **12 YouTube Channels** across Entertainment, Music, Gaming, Tech, and News
- 📈 **Live Stats** — real-time subscribers, views, and video counts via YouTube API
- 🏆 **Best Performing Channel** banner with growth badge
- 📊 **5 Custom SVG Charts** — bar, vertical bar, area/trend, donut, radar (no chart library)
- ⚖️ **Channel Comparison Table** — ranked with avg views per video and growth %
- 🎬 **Per-Channel Deep Dive** — top videos, engagement rate, progress bars
- 🔍 **Search & Filter** — live filter by channel name or category
- 🌙 ☀️ **Dark / Light Theme** — toggle persisted across sessions via `localStorage`
- ⚡ **6-Hour Smart Cache** — avoids redundant API calls, loads instantly on revisit
- 📱 **Responsive** — mobile sidebar collapses into tab navigation

---

## 🚀 Getting Started

### 1. Get a YouTube Data API v3 Key
1. Go to [Google Cloud Console](https://console.cloud.google.com)
2. Create a project → Enable **YouTube Data API v3**
3. Go to **Credentials** → **Create API Key**
4. *(Recommended)* Restrict the key to YouTube Data API v3 only

### 2. Add Your Key
Open `index.html` and find this line:

```js
const API_KEY = "YOUR_YOUTUBE_API_KEY_HERE";
```

Replace with your actual key.

### 3. Open in Browser
No install, no build step needed:

```
Double-click index.html
```

Or use **VS Code Live Server** for the best experience:
```
Right-click index.html → Open with Live Server
```

---

## 🗂️ Channels Tracked

| Channel | Category |
|---|---|
| MrBeast | Entertainment |
| T-Series | Music |
| PewDiePie | Gaming |
| Markiplier | Gaming |
| Fireship | Tech |
| TechWithTim | Tech |
| freeCodeCamp | Tech |
| Traversy Media | Tech |
| Ed Sheeran | Music |
| Eminem | Music |
| CNN | News |
| BBC News | News |

---

## 📌 Dashboard Tabs

| Tab | What It Shows |
|---|---|
| **Overview** | KPI cards, all channel grid, category filter pills |
| **Compare** | Ranked table, subscriber bar chart, radar analysis |
| **Videos** | Top videos with view progress bars |
| **Engagement** | Donut chart, engagement rate per video, trend line |

---

## 🛠️ Tech Stack

| | |
|---|---|
| **Structure** | HTML5 |
| **Styling** | CSS3 — custom properties, glassmorphism, animations |
| **Logic** | Vanilla JavaScript ES6+ |
| **Charts** | Custom SVG — zero libraries |
| **Data** | YouTube Data API v3 |
| **Storage** | localStorage — theme + 6h data cache |

---

## ⚡ API Quota Info

YouTube Data API free tier gives **10,000 units/day**.

| Action | Units |
|---|---|
| Per channel info | ~1 unit |
| Per channel videos | ~100 units |
| Full refresh (12 channels) | ~1,200 units |
| Cache hit | 0 units |

Well within the free limit even with multiple refreshes per day.

---

## 📁 Project Structure

```
yt-analytics-dashboard/
├── index.html    ← Entire app (single file)
└── README.md
```

---

## ⚠️ Security Note

Never commit your real API key to GitHub.  
This repo uses a placeholder — add your own key **locally only**.

---

## 🙏 Credits

**Built by Shain Shafi**  
Hex Softwares Internship — 2026
