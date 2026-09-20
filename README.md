# TeamUp

**Find hackathon teammates near you, filtered your way.**

🔗 **Live site:** [monica1620.github.io/teamup](https://monica1620.github.io/teamup/)
🏆 Built for **Hack Devengers 2.0** (Unstop)

---

## The problem

Finding a hackathon team usually means scrolling through a WhatsApp or Discord group full of "looking for teammate" messages nobody reads, with no way to tell who's actually free, what they're good at, or whether you can trust them.

## The solution

TeamUp is a filtered matchmaking layer for hackathons. Set up a quick profile, filter the pool by **region**, skill, role, experience, availability, and vibe, and send a request to team up. Once it's mutual, you're matched — and you can instantly see what skill your forming team is still missing.

## Features

- **Region-first filtering** — find people in your timezone or part of the world, not a random global list
- **Six filter dimensions** — region, skills, experience level, availability, role, idea status, and vibe
- **Mutual accept** — requests only turn into a match when both sides say yes
- **Instant team gap analysis** — once matched, see exactly what skill or role your team is still missing
- **Zero setup for judges** — no login screen, no backend to configure; profile is saved locally in the browser

## How it works

1. **Create your profile** — region, skills, availability, role, idea status, vibe
2. **Filter & browse** — narrow the pool to real fits
3. **Request to team up** — send a request; a mutual match confirms it
4. **See your team's gaps** — get an instant, rule-based read on what your team still needs

## Tech stack

- Single self-contained `index.html` — no build step, no external runtime dependencies
- Vanilla JavaScript, no framework
- `localStorage` for on-device profile and match persistence
- Hosted on GitHub Pages

## Why no backend?

This build prioritizes something judges can open and use in one click, with nothing to configure. The matching logic and data model are written so that swapping `localStorage` for a real multi-user database (e.g. Supabase or Firebase) later is a drop-in change — the app logic doesn't change, only where state is read and written.

## Running locally

No build step required — just open `index.html` in any browser.

```bash
git clone https://github.com/monica1620/teamup.git
cd teamup
open index.html   # or double-click the file
```

## Submission

Submitted for **Hack Devengers 2.0**, hosted by Unstop.
