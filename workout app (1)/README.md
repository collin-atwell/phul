# PHUL — Lift & Fuel

A private workout + diet tracker built around your **PHUL** program (Power Hypertrophy Upper Lower).
Runs on your iPhone as a home-screen app. **No App Store, no Xcode, no Apple Developer account, no $99 fee.**
All your data stays on your phone — nothing is uploaded anywhere.

## What's inside

- **Calendar** — your 4-day PHUL split laid out (Mon Upper Power · Tue Lower Power · Thu Upper Hyper · Fri Lower Hyper). Tap any day to log it, or swap a leg day for a 🥾 hike.
- **Workout** — log sets, reps, and weight (lbs). Shows your last session's numbers on each lift so you can chase progressive overload. Check off sets as you go.
- **Diet** — log meals with calories + protein/carbs/fat, track water cups, and tick off supplements (creatine, fish oil). Daily calorie ring and macro bars.
- **Stats** — workout streak, weekly volume chart, personal bests on the big lifts, diet adherence. Edit your targets and weekly split in Settings, and export a backup anytime.

---

## How to put it on your iPhone (≈2 minutes)

The app is a **PWA** (Progressive Web App). You just need to get it onto the web once, then "Add to Home Screen." It works fully offline after that.

### Easiest path — Netlify Drop (no coding)
1. On your computer, go to **https://app.netlify.com/drop**
2. Drag this whole `workout app (1)` folder onto the page.
3. It gives you a URL like `https://your-name.netlify.app`.
4. Open that URL **in Safari on your iPhone**.
5. Tap the **Share** button (the square with the up-arrow) → scroll down → **Add to Home Screen** → **Add**.
6. Done. Tap the green dumbbell icon on your home screen — it opens full-screen like a real app and works with no internet.

### Alternative — GitHub Pages (free, also no fees)
1. Create a free GitHub account, make a new repository.
2. Upload all the files in this folder (`index.html`, `manifest.webmanifest`, `sw.js`, and the three `icon-*.png` files).
3. Repo **Settings → Pages → Deploy from branch → main / root → Save**.
4. Open the resulting `https://...github.io/...` URL in Safari and **Add to Home Screen** (same as step 5 above).

> Quick test without any hosting: email yourself `index.html` and open it in Safari — the app runs and saves data. (Offline caching and the home-screen icon work best from a hosted URL, which is why the steps above are recommended.)

---

## Notes
- **Your data lives on the device.** Use **Stats → Export my data** to save a JSON backup before clearing Safari data or switching phones.
- **Change the program** anytime in **Stats → Edit targets & schedule** — assign any PHUL day (or Hike/Rest) to any weekday.
- Everything is in a single `index.html` plus the PWA support files — easy to tweak later.
