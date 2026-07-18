# 🎓 CollegeMate AI — TNEA College Predictor

> **Find the right engineering college for your TNEA cutoff — instantly.**

CollegeMate AI is a single-page, fully client-side web app that helps Tamil Nadu Engineering Admission (TNEA) aspirants predict which colleges they can realistically get into, explore 55+ colleges by district / strength / type, compare shortlists side-by-side, and chat with a built-in assistant for quick answers — all in one bilingual (English + Tamil) interface.

No backend. No database. No API keys. Just one HTML file.

---

## ✨ Features

| Module | What it does |
|---|---|
| 🎯 **Cutoff Predictor** | Enter your cutoff mark, community, branch and (optional) district → get a ranked list of colleges tagged **Safe**, **Moderate**, or **Dream**, each with a plain-English explanation and an admission-chance percentage. |
| 🏫 **Explore Colleges** | Browse all 55 colleges with filters for **District**, **Strength/Focus** (Placement, Skill Development, Academic Excellence, Research, Affordable), and **Type** (Government / Autonomous / Private / Deemed). |
| ❤️ **Favourites** | Save colleges you're interested in from anywhere in the app and revisit them in one tab. |
| ⚖️ **Compare** | Pick up to 3 colleges and see a side-by-side table — fees, placement %, average package, NAAC grade, hostel availability, and strength tags. |
| 🤖 **AI Assistant** | A floating chat bubble (bottom-right) that answers natural questions like *"safe colleges for 178 BC ECE"*, *"hostel colleges in Coimbatore"*, or *"best placement colleges"* — powered entirely by client-side logic, no API required. |
| 🌐 **Bilingual UI** | Toggle the entire interface between **English** and **Tamil** with one click. |

---

## 🧠 How the prediction works

Each college has a **base closing cutoff** (illustrative sample data). The predictor adjusts that baseline using:

- **Branch adjustment** — CSE/IT/AI&DS close higher than ECE/EEE/MECH/CIVIL
- **Community adjustment** — reflects standard TNEA reservation cutoff gaps (OC / BC / BCM / MBC / SC / SCA / ST)

Your cutoff is compared against this adjusted threshold:

- **≥ +3 marks above threshold** → 🟢 Safe
- **Within ±3 marks** → 🟠 Moderate
- **3–14 marks below** → 🔴 Dream
- **More than 14 marks below** → not shown

> ⚠️ **Disclaimer:** All cutoffs, fees, placement %, and package figures in this app are **illustrative sample data** for demo purposes only — not official TNEA statistics. Always verify on [tnea.ac.in](https://www.tnea.ac.in) and the official college website before making admission decisions.

---

## 🛠️ Tech Stack

- **Pure HTML, CSS & vanilla JavaScript** — zero build step, zero dependencies
- **Google Fonts** — Fraunces (headings) + Inter (body) + IBM Plex Mono (data/numbers)
- Fully static — works by simply opening the `.html` file, or hosting it anywhere (GitHub Pages, Netlify, Vercel, etc.)

---

## 🚀 Getting Started

### Run it locally
1. Download `collegemate.html`
2. Double-click it — it opens directly in your browser. That's it.

### Host it for free with GitHub Pages
1. Push this repo to GitHub (see commands below)
2. Go to **Settings → Pages**
3. Set Source to your `main` branch and Save
4. Your live link: `https://<your-username>.github.io/<repo-name>/collegemate.html`

```bash
git init
git add collegemate.html README.md
git commit -m "Initial commit - CollegeMate AI"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

---

## 📂 Project Structure

```
collegemate-ai/
├── collegemate.html   # the entire app (HTML + CSS + JS in one file)
└── README.md           # you are here
```

---

## 🗺️ Roadmap / Ideas for later

- [ ] Swap the sample dataset for real, verifiable TNEA cutoff data
- [ ] Add more branches (Biomedical, Chemical, Automobile, etc.)
- [ ] Persist favourites/compare list across sessions (localStorage or a small backend)
- [ ] Connect the assistant to a real LLM backend for open-ended Q&A
- [ ] Add year-over-year cutoff trend charts per college

---

## 📄 License

This project is for educational/demo purposes. Feel free to fork, modify, and build on it.

---

<p align="center">Made with ❤️ for TNEA aspirants — good luck with your counselling! 🎓</p>
