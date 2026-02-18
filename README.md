# 🛡️ THREAT HUNTER — Cyber Defense Arcade

> **An AI-powered endless cybersecurity shooter that teaches real-world threat intelligence through gameplay.**

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/threat-hunter)
[![License: MIT](https://img.shields.io/badge/License-MIT-cyan.svg)](LICENSE)

---

## 🎮 Play Now

**[▶ Live Demo](https://threat-hunter-gules.vercel.app)/** *(update after deployment)*

---

## What is this?

THREAT HUNTER is an endless wave-based arcade game where every enemy is a **real cyber threat** — phishing lures, trojans, worms, ransomware, rootkits, APT agents, and zero-day exploits. Each kill teaches you real cybersecurity facts, and an AI analyst named **SENTINEL** briefs you between waves using actual CVEs, MITRE ATT&CK techniques, and incident case studies.

It's designed to make cybersecurity education engaging and addictive — learn while you play.

---

## ✨ Features

### 🕹️ Gameplay
- **Endless waves** — difficulty scales infinitely, how far can you go?
- **8 threat types** with unique visuals, behaviors, and attack patterns
- **Boss fights** every 5 waves (APT Agents and Zero-Day Exploits that shoot back)
- **Combo system** (up to ×12 multiplier) and kill streaks (10, 25, 50, 100)
- **Dash** (Shift) with invincibility frames for clutch dodges
- **EMP blast** (E) — area-of-effect damage that costs energy
- **6 powerups**: Heal, Spread Shot, Rapid Fire, Full Shield, Killswitch (nuke), Time Freeze
- **Magnetic data orbs** that fly out of kills and get pulled toward you
- **Screen shake**, slow-motion boss kills, score popups, particle explosions

### 🤖 3 Live API Integrations

| API | Purpose | Auth Required |
|-----|---------|---------------|
| **Anthropic Claude** | AI analyst (SENTINEL) gives tactical briefings between waves, personalized debriefs on game over, and answers questions in the Threat Codex | Via Anthropic proxy |
| **Open Trivia DB** | Computer science trivia bonus rounds every 2 waves — correct answers heal + bonus score | None (free) |
| **NVD/NIST CVE API** | Live vulnerability feed on the start screen showing real high-severity CVEs with CVSS scores | None (free) |

### 📚 Educational Content
- **48 real cybersecurity facts** baked into kill popups
- **Threat Codex** — unlock intel on each threat type with real-world case studies
- Real incidents: WannaCry, Colonial Pipeline, SolarWinds, Log4Shell, Mirai, and more
- Defense strategies and MITRE ATT&CK technique references
- AI-powered deep dives — ask SENTINEL anything about any threat

### 📱 Share Your Score
- Enter your call sign after each run
- Share formatted results to Twitter/LinkedIn/WhatsApp
- Includes score, wave, kills, combo, streak, trivia accuracy, and threats identified

---

## 🚀 Deploy

### One-Click Vercel Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/threat-hunter)

### Manual Deploy

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/threat-hunter.git
cd threat-hunter

# Deploy to Vercel
npx vercel

# Or just open index.html locally
open index.html
```

### Deploy Anywhere
It's a **single HTML file** — no build step, no dependencies, no framework. Works on:
- Vercel
- Netlify (drag and drop)
- GitHub Pages
- Any static hosting
- Or just open `index.html` in a browser

---

## 🎮 Controls

| Key | Action |
|-----|--------|
| `W A S D` / Arrow Keys | Move |
| `Space` | Fire |
| `Shift` | Dash (costs 12 energy, grants i-frames) |
| `E` | EMP Blast (costs 35 energy, AoE damage) |

---

## 🧬 Threat Types

| Threat | Category | HP | Behavior |
|--------|----------|-----|----------|
| 🔷 Phishing | Social Engineering | 1 | Fast, erratic movement |
| 🔶 Trojan | Malware | 1 | Steady approach, disguised |
| 🟠 Worm | Malware | 1 | Fast, sine-wave movement |
| ⚡ DDoS Bot | Network Attack | 1 | Very fast, swarm behavior |
| 👻 Rootkit | Persistence | 2 | Semi-transparent, shoots back |
| 🔴 Ransomware | Malware | 3 | Tanky, shoots projectiles |
| 🎯 APT Agent | Advanced (Boss) | 10 | Spread-shot pattern, tactical |
| 💀 Zero-Day | Advanced (Boss) | 16 | Ring-shot pattern, devastating |

---

## 📁 Project Structure

```
threat-hunter/
├── index.html      # The entire game (single file)
├── vercel.json     # Vercel deployment config
├── LICENSE         # MIT License
└── README.md       # This file
```

---

## 🛠️ Tech Stack

- **Vanilla HTML5 Canvas** — no frameworks, no dependencies
- **Web Audio API** — procedural sound effects
- **Anthropic Claude API** — AI-powered game intelligence
- **Open Trivia DB API** — trivia questions
- **NVD NIST API** — real CVE vulnerability data

---

## 📝 Notes on AI Features

The Anthropic API calls work automatically in Claude.ai artifacts. For production deployment on Vercel, you may need to set up a serverless API proxy function to handle authentication. The Trivia DB and CVE APIs are fully public and work everywhere.

---

## 🤝 Credits

- **Game Design & Development**: Built with Claude
- **Trivia Data**: [Open Trivia Database](https://opentdb.com/) (CC BY-SA 4.0)
- **CVE Data**: [National Vulnerability Database](https://nvd.nist.gov/) (NIST)
- **AI Intelligence**: [Anthropic Claude](https://anthropic.com/)
- **Cybersecurity Knowledge**: MITRE ATT&CK, real-world incident reports

---

## 📄 License

MIT License — free for personal and commercial use.

---

<p align="center">
  <strong>How long can you survive the kill chain? 🛡️</strong>
</p>
