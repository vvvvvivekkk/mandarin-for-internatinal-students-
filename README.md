# Mando · Taiwan Mandarin for International Students

> 台灣中文學習應用程式 · A free, zero-install Taiwan Mandarin learning app built for international exchange students at **National Chung Cheng University (CCU)** and anywhere else in Taiwan.

🔊 **Audio on every phrase** · 🇹🇼 **Traditional characters** · 📱 **Mobile-first** · ⚡ **Single HTML file, zero backend**

## 🌐 Live demo

Open [`index.html`](./index.html) in any modern browser. Works offline once loaded. No build step, no install.

For a hosted version, enable **GitHub Pages** in repo Settings → Pages → Deploy from branch `main` → `/root`. The app will be live at `https://vvvvvivekkk.github.io/mandarin-for-internatinal-students-/`

## ✨ What it does

Everything a new exchange student needs for daily life in Taiwan:

- **🏠 Home** — Daily phrase, voice selector, speed control, quick-access tiles
- **📖 Learn** — 160+ phrases across 15 categories, with live search
- **🎓 Lessons** — Interactive versions of Prof. 陳欣徽's course material (Lessons 3–6)
- **🎯 Practice** — Listen-and-identify quiz across 5 categories, with score tracking
- **📚 Reference** — Interactive 4-tone wheel, full pinyin chart, 6 tongue twisters

### Content categories

| Category | 中文 | What's inside |
|---|---|---|
| Greetings | 問候 | Hi, bye, good morning, Taiwan-casual "have you eaten?" |
| Basics | 基本 | Thanks, sorry, please, yes/no |
| Introduce | 自我介紹 | Self-intro pre-built for CCU exchange students |
| Numbers | 數字 | 0–10,000 + counters |
| Time & Days | 時間 | Days of the week, time expressions |
| Food & Drink | 飲食 | Full bubble tea customization (半糖, 去冰, 無糖) |
| Shopping | 購物 | Prices, sizes, card vs cash |
| 7-Eleven | 便利商店 | EasyCard, receipt lottery, heating food |
| Night Market | 夜市 | 老闆, portions, tasting |
| Transit | 交通 | MRT, HSR, scooter, taxi |
| Directions | 方向 | Left/right, Google Maps vocab |
| Dorm & Campus | 宿舍與校園 | Wifi, laundry, 冷氣, classroom basics |
| Weather | 天氣 | Hot, cold, 颱風 |
| Emergency | 緊急 | 119, 110, hospital, pharmacy |
| Taiwan Slang | 台灣俚語 | 加油, 超讚, 蝦米, 拍謝 |

Each phrase shows:
- **Traditional Chinese** (繁體字 — what you'll see on Taiwan signs)
- **Pinyin with tone marks**
- **English meaning**
- **Audio playback** via Web Speech API (prefers 🇹🇼 zh-TW voices)
- Tags for **Taiwan-specific** (TW) and **must-learn** (★) phrases

## 🧰 Tech

- **One HTML file.** No build step, no dependencies, no backend.
- **Web Speech API** for text-to-speech (works offline on most devices once the voice is cached).
- **CSS Grid + Flexbox** responsive layout — bottom tab navigation on mobile, horizontal nav on desktop.
- **Dark mode by default** with a one-tap light-mode toggle.
- **~85 KB** uncompressed. Loads instantly on dorm wifi.

## 🎓 Course lessons

Interactive versions of the real course material from **Prof. 陳欣徽 (Chen Hsin-Hui)**:

- **Lesson 3** — j · q · x initials + i/ü finals + spelling rules (y/w substitutions)
- **Lesson 4** — z · c · s dentals + dividing apostrophe (`Xī'ān`)
- **Lesson 5** — zh · ch · sh · r retroflex + the 不 (bù → bú) tone sandhi + full bubble-tea dialogue
- **Lesson 6** — Word stress tips + 一 (yī) tone changes + Shantian's self-introduction model

## 📱 How to use

1. Open `index.html` in Chrome, Edge, or Safari (any OS).
2. At the top, pick a Chinese voice from the dropdown — prefer any marked **🇹🇼 zh-TW** for the most natural Taiwan accent.
3. Adjust the speed slider down (0.6–0.7) if you need slower pronunciation while learning.
4. Tap any phrase card or 🔊 button to hear it.
5. Use the **bottom navigation** to switch between Home / Learn / Lessons / Practice / Reference.

### Install a Chinese voice (if dropdown is empty)

- **macOS**: System Settings → Accessibility → Spoken Content → System Voice → Manage Voices → add "Mei-Jia" or "Sin-Ji" (both zh-TW).
- **Windows**: Settings → Time & Language → Speech → Add voices → Chinese (Traditional, Taiwan).
- **iOS**: Settings → Accessibility → Spoken Content → Voices → Chinese → download Mei-Jia or Sin-Ji.
- **Android**: Settings → System → Languages → Google Text-to-speech engine → Install voice data → Chinese (Taiwan).

## 🎯 Who this is for

Primary: International exchange students landing in Taiwan with zero Mandarin, especially those at CCU in Chiayi.

Also useful for:
- Anyone taking a beginner Taiwan Mandarin class (Traditional characters, not Simplified)
- Travelers to Taiwan who want more than Google Translate
- Students pivoting from mainland Mandarin resources to Taiwan-specific vocabulary

## 🛣️ Roadmap

Open to contributions. Planned next:

- [ ] More course lessons as they are covered (L7+)
- [ ] Spaced-repetition flashcard mode (SRS)
- [ ] Photo-to-translation (camera → Gemini Vision API for signs, menus)
- [ ] AI conversation partner (Groq / Gemini free tier) for role-play scenarios
- [ ] Progress tracking with localStorage
- [ ] PWA installable version with offline voice caching

## 🤝 Contributing

Add a new phrase: edit the `PHRASES` array in `index.html` with `{ zh, pinyin, en, cat, tw?, hot? }`.

Add a new category: extend `CATEGORIES` array with `{ id, icon, name, cn, py }`.

Add a lesson: duplicate one of the `<div class="lesson">` blocks in the Lessons section.

Pull requests welcome — especially from other CCU exchange students who notice missing vocab.

## 📄 License

MIT — use it, fork it, ship it in your own class materials. No attribution required (but appreciated).

---

Built with help from Claude. For international students at [CCU](https://www.ccu.edu.tw/) · 2026.

加油! 🇹🇼
