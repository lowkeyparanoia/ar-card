# AR Business Card — AI Engineer

Paper-free digital + AR business card. Show QR on your phone → they scan → see holographic card in browser. Tap "View in AR" → card floats in real space.

## Files

```
index.html   — 3D flip card, skills, contact links, particle background
ar.html      — AR camera view (point at Hiro marker)
```

## Customise (5 min)

In `index.html`, change:
- `Your Name` → your real name
- `AI / ML Engineer · LLMs · Agents · MLOps` → your title
- All `yourusername` → your handles
- `you@email.com` → your email
- `yourportfolio.dev` → your URL
- Skills badges in the grid section

Same changes in `ar.html` (the `<a-text>` elements).

## Deploy to GitHub Pages

```bash
cd /Users/Jre/ar-card
git init
git add .
git commit -m "Initial AR business card"

# Create repo on github.com first, then:
git remote add origin https://github.com/YOURUSERNAME/ar-card.git
git push -u origin main

# Enable GitHub Pages:
# GitHub repo → Settings → Pages → Source: main branch → / (root)
# Live at: https://YOURUSERNAME.github.io/ar-card
```

## AR Usage

1. Open `ar.html` on phone — grants camera
2. Show the **Hiro marker** (print or display on second screen)
   - Get marker: https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png
3. Point camera → card floats above marker

## Share your card

- Save your GitHub Pages URL as a QR code (use qr-code-generator.com)
- Screenshot the QR → save to phone home screen photo
- Show QR → person scans → instant holographic card
- No app install, no physical card needed

## Browser support

| Browser | Digital card | AR view |
|---------|-------------|---------|
| iOS Safari | ✅ | ✅ (camera) |
| Android Chrome | ✅ | ✅ (camera) |
| Desktop Chrome | ✅ | ✅ (webcam) |
| Desktop Safari | ✅ | ✅ (webcam) |
