# S-play 🎬
### Your Cinema, Unlimited — YouTube Video Streaming Interface

A beautiful dark-themed video streaming UI that searches and plays YouTube videos using the YouTube Data API v3 and youtube-nocookie.com embed.



## ✨ Features

- 🔍 Live YouTube search via YouTube Data API v3
- ▶️ In-app video playback via youtube-nocookie.com embed (works on all origins)
- 🎬 Category pills: Action, Comedy, Thriller, Sci-Fi, Horror, Documentary, Music
- 📋 Up Next queue while watching
- 🕐 Watch Later (saved to localStorage)
- ❤️ Liked videos (saved to localStorage)
- 🕘 Watch history (saved to localStorage)
- 🔗 Share video link / copy to clipboard
- ⌨️ Keyboard shortcut: Escape closes the player
- 📱 Fully responsive (mobile + desktop)
- 🌙 Dark cinema theme

---

## 🛠 Tech Stack

- Pure HTML5 + CSS3 + Vanilla JavaScript (zero dependencies)
- YouTube Data API v3 (search + video metadata)
- youtube-nocookie.com IFrame embed (video playback)
- Google Fonts (DM Sans + Playfair Display)
- localStorage (Watch Later, Liked, History)

---

## 📝 Notes

- The YouTube embed uses `youtube-nocookie.com` which works from any origin including `file://`, `localhost`, and deployed HTTPS domains — no "Video configuration error" issues.
- The modal player uses no `overflow:hidden`, `clip-path`, `transform`, or `filter` on the iframe ancestors, which prevents the audio-only / black video rendering bug in Chromium.
- Free YouTube API quota is 10,000 units/day. Each search uses ~100 units, so ~100 searches/day on the free tier.
