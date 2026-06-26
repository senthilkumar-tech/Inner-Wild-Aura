<div align="center">

# 🐾 Inner Wild Aura™

### *Discover the Animal Hidden Within Your Soul*

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Visit_Site-ff0080?style=for-the-badge)](https://innerwildaura.com)
[![License](https://img.shields.io/badge/License-MIT-8b00ff?style=for-the-badge)](LICENSE)
[![Made With](https://img.shields.io/badge/Made_With-HTML%2FCSS%2FJS-ff6b00?style=for-the-badge)](#)
[![Spirit Animals](https://img.shields.io/badge/Spirit_Animals-15_Unique-00d4ff?style=for-the-badge)](#spirit-animals)

<br/>

> **2.4M+ souls discovered · 15 spirit animals · 10 personality dimensions**

<br/>

🦁 🐺 🦊 🦉 🦅 🐯 🐬 🐘 🐆 🐋 🐈‍⬛ 🦊 🐼

</div>

---

## ✨ What Is This?

**Inner Wild Aura™** is a viral, mobile-first personality quiz web app that matches users to their spirit animal through a 10-question psychometric quiz. Built as a single HTML file with zero dependencies — pure HTML, CSS, and vanilla JavaScript.

It blends the wonder of Disney storytelling, the depth of National Geographic wildlife, and the shareability of viral social media quizzes into one immersive, visually stunning experience.

---

## 🖼️ Screenshots

| Landing Page | Quiz | Results |
|---|---|---|
| Animated hero with particle system | 10-question trait analysis | Full spirit animal reveal |
| Daily animal wisdom | Glowing progress bar | Animated trait bars |
| Animal carousel | Emoji-driven options | Shareable result card |

---

## 🚀 Features

### 🎯 Core Quiz Engine
- **10 personality questions** measuring 10 soul dimensions
- **Psychometric scoring algorithm** — each answer weights traits across all 15 animals
- **Animated loading reveal** with rotating animal parade
- **Rare spirit animal unlocks** — Snow Leopard, Panther, Orca, Red Panda trigger only on edge-case profiles

### 🐾 Spirit Animals (15 Total)

| Animal | Rarity | Dominant Trait |
|--------|--------|----------------|
| 🦁 Lion | Common | Leadership + Courage |
| 🐺 Wolf | Common | Loyalty + Pack Instinct |
| 🦊 Fox | Common | Intelligence + Creativity |
| 🦉 Owl | Common | Wisdom + Empathy |
| 🦅 Eagle | Common | Independence + Vision |
| 🐯 Tiger | Common | Courage + Strategy |
| 🐬 Dolphin | Common | Empathy + Social Energy |
| 🐘 Elephant | Common | Loyalty + Memory |
| 🐆 Snow Leopard | ⭐ Rare | Creativity + Solitude |
| 🦊 Red Panda | ⭐ Rare | Curiosity + Warmth |
| 🐈‍⬛ Panther | ⭐ Rare | Mystery + Power |
| 🐋 Orca | ⭐ Rare | Intelligence + Leadership |

### 🎨 Visual Design
- **Glassmorphism cards** with backdrop blur
- **Neon glow animations** and gradient text
- **Floating particle system** (25 animated particles)
- **Conic gradient logo ring** with infinite spin
- **Auto-scrolling animal carousel**
- **Pulse glow CTA button**
- Mobile-first, fully responsive

### 📊 Results Page
- Spirit animal emoji with floating animation
- Soul match percentage badge
- **10 animated trait bars** (staggered reveal on load)
- Strengths, Shadow Side, Social Style, Hidden Talent cards
- Fun wildlife fact per animal
- Rare spirit badge for edge-case results
- Animal Compatibility teaser
- Achievement badges (Soul Seeker, Wild Heart, Mystic, Rare Spirit)
- Daily Animal Wisdom quote (rotates by day of week)

### 📲 Social & Sharing
- One-tap share to **WhatsApp**, **X (Twitter)**, **Instagram**, **Facebook**
- **Downloadable SVG result card** — auto-generated with name, emoji, match %
- Pre-written viral copy per result

---

## 🧬 Personality Dimensions

The quiz scores users across 10 dimensions:

```
Leadership     ████████████████████  
Loyalty        ████████████████████  
Courage        ████████████████████  
Intelligence   ████████████████████  
Creativity     ████████████████████  
Adaptability   ████████████████████  
Empathy        ████████████████████  
Curiosity      ████████████████████  
Social Energy  ████████████████████  
Independence   ████████████████████  
```

Each of the 40 answer options (10 questions × 4 choices) carries a unique weight vector across these dimensions. The spirit animal with the highest weighted dot product against the user's cumulative score wins.

---

## 🗂️ Project Structure

```
inner-wild-aura/
│
├── index.html          # Entire app — single file, zero dependencies
├── README.md           # This file
├── LICENSE             # MIT
└── assets/             # Optional: OG image, favicon, preview screenshots
    ├── og-image.png
    └── favicon.png
```

> **Single file architecture.** The entire quiz — all pages, animations, quiz logic, scoring algorithm, 15 animal profiles, and share functionality — lives in one `index.html`. No build step. No npm install. No framework. Just open and run.

---

## ⚡ Getting Started

### Option 1 — Just open it
```bash
git clone https://github.com/yourusername/inner-wild-aura.git
cd inner-wild-aura
open index.html   # or double-click the file
```
That's it. No server needed. Works completely offline.

### Option 2 — Serve locally
```bash
# Python
python -m http.server 8080

# Node
npx serve .

# VS Code
# Install Live Server extension → Right-click index.html → Open with Live Server
```

### Option 3 — Deploy in 60 seconds

**Netlify Drop:**
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag your `index.html` onto the page
3. Get a live URL instantly

**GitHub Pages:**
```bash
# In your repo settings → Pages → Source: Deploy from branch → main → / (root)
# Your site goes live at: https://yourusername.github.io/inner-wild-aura
```

**Vercel:**
```bash
npx vercel --prod
```

---

## 🛠️ Customization Guide

### Add a New Spirit Animal
Find the `ANIMALS` object and add a new entry:

```javascript
const ANIMALS = {
  // ... existing animals ...

  cheetah: {
    name: 'The Cheetah',
    emoji: '🐆',
    rare: false,
    match: 91,
    traits: {
      leadership: 75,
      loyalty: 70,
      courage: 96,
      intelligence: 88,
      creativity: 72,
      adaptability: 97,   // <-- cheetah's superpower
      empathy: 65,
      curiosity: 85,
      social: 60,
      independence: 95
    },
    desc: "You are the Cheetah — built for speed, precision, and explosive action...",
    fact: "🐆 Cheetahs can accelerate from 0 to 100km/h in 3 seconds...",
    strengths: ['Lightning fast', 'Laser focus', 'Decisive', 'Adaptive'],
    weaknesses: ['Burns out quickly', 'Impatient', 'Short bursts only'],
    social: 'Semi-solitary — sprints alone, rests with a small trusted circle.',
    talent: 'Executing at maximum speed when everyone else freezes.'
  }
};
```

### Add a New Question
Find the `QUESTIONS` array and append:

```javascript
{
  emoji: '🌙',
  trait: 'night_mind',
  text: 'What does your mind do at 3am when you cannot sleep?',
  options: [
    { e: '📋', t: 'Plan tomorrow in perfect detail',        score: { leadership: 9, intelligence: 8 } },
    { e: '🎨', t: 'Flood with creative ideas and visions', score: { creativity: 10, curiosity: 9 } },
    { e: '💭', t: 'Replay conversations and feel deeply',   score: { empathy: 10, social: 8 } },
    { e: '🌌', t: 'Drift into pure philosophical wonder',   score: { intelligence: 10, independence: 9 } }
  ]
}
```

### Change the Color Theme
The three main gradient stops control the entire vibe:

```css
/* In the <style> block, find and replace: */
--color-1: #ff6b00;   /* orange */
--color-2: #ff0080;   /* hot pink */
--color-3: #8b00ff;   /* purple */
--color-4: #00d4ff;   /* cyan */
--color-5: #00ff88;   /* green */
```

---

## 📐 Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 (semantic) |
| Styling | CSS3 — Custom Properties, Keyframe Animations, Backdrop Filter, Conic Gradient |
| Logic | Vanilla JavaScript (ES6+) |
| Animations | Pure CSS — no GSAP, no libraries |
| Sharing | Web Share API + platform deep links |
| Download | SVG Blob + anchor download trick |
| Fonts | System font stack |
| Dependencies | **Zero** |
| Bundle size | ~1 single HTML file |

---

## 🧪 How the Scoring Works

```
For each question answered:
  For each spirit animal:
    contribution = Σ (animal.traits[t] / 100) × answer.score[t]
    animal.totalScore += contribution

Winner = animal with highest totalScore after all 10 questions
```

Each answer option carries a `score` object — e.g. `{ courage: 10, leadership: 8 }`. For every trait in that object, the algorithm checks how strongly each animal embodies that trait (0–100), multiplies by the answer weight, and accumulates. After 10 questions, the animal whose trait DNA best matches your answer pattern wins.

---

## 🌍 Browser Support

| Browser | Support |
|---------|---------|
| Chrome 88+ | ✅ Full |
| Firefox 87+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 88+ | ✅ Full |
| Mobile Chrome | ✅ Full |
| Mobile Safari | ✅ Full |

> Backdrop-filter (glassmorphism) requires Chrome 76+, Safari 9+, Firefox 103+.

---

## 🗺️ Roadmap

- [ ] **v2.0** — Animal Compatibility Mode (compare two users' results)
- [ ] **v2.1** — Animated result card generation (Canvas API)
- [ ] **v2.2** — Sound effects — each animal has its real sound on reveal
- [ ] **v2.3** — Extended quiz — 20 questions, 6 rarer animals unlocked
- [ ] **v2.4** — Localization — Tamil, Hindi, Japanese, Spanish
- [ ] **v3.0** — Backend leaderboard — most common spirit animals by region
- [ ] **v3.1** — Friend comparison — send a link, see your wild compatibility score
- [ ] **v3.2** — Daily streak — retake once per day, track how your wild self shifts

---

## 🤝 Contributing

Contributions are very welcome! Especially:

- New spirit animals with full trait profiles
- New quiz questions
- Translations / localization
- Accessibility improvements
- Performance optimizations

```bash
# Fork the repo, make your changes, then:
git checkout -b feature/add-cheetah-spirit
git commit -m "feat: add cheetah spirit animal with adaptability profile"
git push origin feature/add-cheetah-spirit
# Open a Pull Request
```

Please keep the zero-dependency, single-file architecture. This is a feature, not a limitation.

---

## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## 🙏 Credits

Built with pure HTML, CSS, and Vanilla JS.  
Personality dimensions inspired by Big Five (OCEAN) and Jungian archetype research.  
Wildlife facts sourced from WWF, National Geographic, and IUCN Red List data.

---

<div align="center">

**Made with 🐾 and wild curiosity**

*If this project helped you — drop a ⭐ and share your spirit animal!*

🐺 🦁 🦊 🦉 🦅 🐯 🐬 🐘 🐆 🐋 🐈‍⬛ 🐼

</div>
