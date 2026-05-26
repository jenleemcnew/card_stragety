# 💳 Card Strategy — Which Card Do I Swipe?

**A lightweight, mobile-first web app that tells you exactly which credit card to use for every purchase — instantly.**

🔗 **Live demo:** [jenleemcnew.github.io/card_stragety](https://jenleemcnew.github.io/card_stragety)

---

## The Problem

You have multiple rewards credit cards. Each one earns more points or cash back in different categories. But standing at the register — or ordering online — you can never remember which card is best for *this* purchase.

So you guess. Or you just use the same card for everything and leave rewards on the table.

**Card Strategy fixes that.**

---

## What It Does

- **Instant lookup** — type what you're buying and it tells you which card to use, the earn rate, and why
- **Tap-to-expand card sections** — browse all categories by card at a glance
- **Smart fallback** — if a category doesn't match any bonus, it defaults to your flat-rate catch-all card automatically
- **Works on any phone** — add it to your home screen and it opens like a native app, no app store required
- **No login. No data collected. No internet required after first load.**

---

## Who It's For

| User | Use Case |
|------|----------|
| 👫 Couples | Share one URL so both partners always swipe the right card |
| 🃏 Rewards maximizers | Stop leaving points on the table across 3–5 cards |
| 💼 Financial coaches | White-label and customize for each client's specific card stack |
| 🏦 Anyone new to credit card rewards | Removes the learning curve entirely |

---

## How to Add It to Your Phone Home Screen

No app store needed. It installs as a Progressive Web App (PWA).

**iPhone (Safari):**
1. Open the live link in Safari
2. Tap the **Share button** (box with arrow)
3. Tap **"Add to Home Screen"**
4. Tap **Add** — done

**Android (Chrome):**
1. Open the live link in Chrome
2. Tap the three-dot menu
3. Tap **"Add to Home Screen"**

It will appear on your home screen and open full screen like a native app.

---

## How to Customize It for Your Own Cards

This is a single `index.html` file — no build tools, no frameworks, no dependencies.

To personalize it:

1. Fork this repo
2. Open `index.html`
3. Edit the **card sections** in the HTML to match your cards and their category rates
4. Edit the **`rules` array** in the JavaScript to update the quick lookup logic
5. Commit and push — your personalized version goes live automatically via GitHub Pages

Each rule in the lookup array looks like this:

```javascript
{
  keys: ['gas', 'fuel', 'shell', 'chevron'],  // search terms that trigger this rule
  card: 'Your Card Name',                      // card to recommend
  rate: '3% cash back',                        // earn rate to display
  why: 'Explanation of why this card wins.'    // shown below the rate
}
```

No coding experience required beyond basic find-and-replace.

---

## How to Deploy Your Own Version Free

1. Fork this repo
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your personalized app is live at `yourusername.github.io/card_stragety`

Total cost: **$0.** Hosted free on GitHub Pages forever.

---

## Tech Stack

| Layer | Choice | Why |
|-------|--------|-----|
| Framework | None — vanilla HTML/CSS/JS | Zero dependencies, loads instantly, works offline |
| Hosting | GitHub Pages | Free, reliable, deploys on every commit |
| Fonts | Google Fonts (DM Sans + DM Serif Display) | Loaded once, cached forever |
| Install | PWA via browser | No app store friction |

---

## Roadmap Ideas

- [ ] User-customizable cards via a settings screen (no code required)
- [ ] Annual spend cap tracker (e.g. Credit One X5 $5k/yr cap)
- [ ] Points value calculator — see estimated dollar value of rewards earned
- [ ] Shareable card profiles — generate a custom URL for your exact card stack
- [ ] Dark/light mode toggle

---

## Contributing

Pull requests welcome! If you've customized this for a popular card combination (Chase Trifecta, Amex ecosystem, Capital One duo, etc.) and want to share it as a preset, open a PR.

---

## License

MIT — free to use, fork, customize, and share. A credit back to this repo is appreciated but not required.

---

*Built for real people trying to get the most out of their wallet — without a finance degree.*
