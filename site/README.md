# Co-Work & — AI Content Engine Waitlist

A single-page, no-build waitlist landing page for Co-Work &'s "Build Your AI
Content Engine" cohort.

## Run locally

No build step or dependencies — just open the file or serve the folder:

```bash
# Option 1: just open it directly
open index.html        # macOS
# or double-click index.html in your file explorer

# Option 2: serve it (recommended, avoids any local file:// quirks)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Structure

```
site/
  index.html       # the whole page (markup + CSS + a few lines of vanilla JS)
  images/          # hero photo + photo strip + logo
```

## Notes

- The waitlist form is front-end only: clicking "Join the Waitlist" swaps the
  form for a success state via a few lines of plain JavaScript in
  `index.html`. Wire it up to a real backend/API or a form service (e.g.
  Formspree, Tally, a serverless function) to actually collect signups.
- The hero photo frame auto-cycles through 5 photos with a smooth crossfade
  (pure CSS animation, no JS needed).
