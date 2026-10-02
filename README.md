# RT Quick Reference

A sage-green study site for respiratory therapy students, built for quick lookups on a phone or laptop.

| Page | What's on it |
| --- | --- |
| `index.html` | **ABG values** (pH, PaCO₂, HCO₃⁻, PaO₂, SaO₂, base excess, ROME) and **O₂ delivery devices** (nasal cannula, simple mask, partial rebreather, non-rebreather, Venturi): liter flow, FiO₂, low vs. high flow, humidification, and whether FiO₂ changes with the patient's RR/VT |
| `meds.html` | **NBRC respiratory medication chart**: table, cards, flashcards, and an NBRC-style practice quiz, with search and drug-class filters |

Both pages share one navigation bar (ABG Values · O₂ Devices · Medications), follow your phone's light/dark setting, and need no build step or installs.

## Put it online with GitHub Pages

1. Create a new repository on GitHub (it can be public or private with Pages enabled on your plan).
2. Click **Add file → Upload files** and drag in `index.html`, `meds.html`, and `README.md`, then **Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick `main` and `/ (root)`, then **Save**.
5. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`.

Tip: on your phone, open the site and use **Add to Home Screen** so it opens like an app.

## Editing

- **ABG / O₂ values:** edit the text directly in `index.html`.
- **Medications:** in `meds.html`, the drug list is the `D = [ ... ]` array and the practice questions are the `QUIZ = [ ... ]` array inside the `<script>` near the bottom. Each entry's fields are explained in the comment above it.

Flashcard progress and filters are saved in your browser (per device).

> For exam study. Ranges and doses vary slightly between textbooks and facilities — always follow your program's references and the current order / package insert in clinical practice.
