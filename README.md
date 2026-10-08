# Pocket Pulmo

*For quick lookups or long study sessions.*

A sage-green study site for respiratory therapy students preparing for the NBRC TMC / CSE exams. It's built for quick lookups on a phone or laptop: no logins, no installs, and it follows your device's light/dark setting.

It opens on a **landing page** that explains what's here and helps you pick where to start. After that, every page shares the same simple navigation bar:

- **Look up** menu: ABG values · Medications · O₂ devices · O₂ math & gas cylinders · Mnemonics
- **Practice** menu: O₂ device cases · Med cases · O₂ math quiz · ABG practice · Medication quiz · Med flashcards · Review my mistakes
- **Search:** search the whole site from any page. Press `/` on a keyboard, or tap the magnifying glass.

---

## What's on the site

### Home — `index.html`
The landing page, made so the site isn't overwhelming the first time:
- **Badges under the tagline:** **Works offline** (it changes to "saved on this device ✓" once your phone has saved the site) and **Add to Home Screen** (tap it for iPhone and Android steps, plus a one-tap Install button on Android/Chrome).
- **A big search box.** Type a drug, device, gas, formula, lab value, symptom or mnemonic (e.g. "albuterol", "Venturi", "E cylinder", "thrush", "can't see"), and it jumps you to the right spot. Drug results open the med chart already filtered to that drug. "Try:" buttons show example searches.
- **Two paths:** **Look something up** (the 5 reference pages) and **Practice** (the 7 quizzes, flashcards and your mistakes deck), each with a one-line description. The **Review my mistakes** card shows a red count when you have questions waiting.
- **Quick numbers:** a tabbed card (ABG · O₂ devices · O₂ math · Meds) with the most-looked-up values: ABG normals and ROME, every device's flow and FiO₂, entrainment ratios and cylinder factors, and key med doses (albuterol, ipratropium, DuoNeb, the 20-beat rule, theophylline level, caffeine loading, racemic epi, PFT reversibility). It remembers the last tab you opened, and each tab links to its full chart.
- **Case of the day:** one patient case from the O₂ and med case sets, the same for everyone on a given day. It works through all of them in a shuffled order before any case repeats. Answer it right on the home page to see the explanation. It remembers today's answer, keeps a streak for days in a row, and links to more cases like it.

### 1. ABG Values — `abg-o2.html#abg`
Normal adult arterial blood gas values (room air, sea level), each with what a high or low value means:

| Value | Normal range |
| --- | --- |
| pH | 7.35 – 7.45 |
| PaCO₂ | 35 – 45 mmHg |
| HCO₃⁻ | 22 – 26 mEq/L |
| PaO₂ | 80 – 100 mmHg |
| SaO₂ | 95 – 100% |
| Base excess | −2 to +2 mEq/L |

Plus the **ROME** rule (Respiratory Opposite, Metabolic Equal), and a link to ABG practice.

### 1b. ABG Practice — `abg-practice.html`
Unlimited random blood gases to interpret.

- **Options:** all patterns, respiratory only, or metabolic only; acid–base only or with PaO₂; and 5, 10 or 20 gases.
- **Patterns:** normal; uncompensated, partially compensated and fully compensated respiratory or metabolic acidosis or alkalosis; and combined (mixed) acidosis or alkalosis. Every generated gas follows Henderson–Hasselbalch, so the numbers are realistic.
- **Oxygenation (when PaO₂ is on):** 80–100 normal, 60–79 mild, 40–59 moderate, below 40 severe hypoxemia.
- **Every answer explains itself:**
  - a **tic-tac-toe grid** that puts each value in its Acid / Normal / Base column;
  - numbered steps (pH → PaCO₂ → HCO₃⁻ → primary problem → compensation → oxygenation);
  - common causes.
- **Also on the page:** a "How to read an ABG" refresher and a "Retry the missed" button.

### 1c. Review My Mistakes — `review.html`
Every question you miss anywhere on the site goes into one personal deck. That includes O₂ device cases, med cases, the medication quiz, the O₂ math quiz, ABG practice and the case of the day.

- **Leaving the deck:** answer a question right (here or in its original quiz) and it leaves the deck. Miss it again and it stays, marked "missed 2×" and so on. The most-missed questions come up first.
- **Filters:** review everything or one source at a time, and choose 5, 10, 20 or all.
- **Math questions:** keep their typed-answer box and the calculator.
- **Browse the deck:** see every question and answer in a list, remove single questions, or clear the deck (it asks you to confirm first).
- **Storage:** the deck is saved on your device only (up to 300 questions) and works offline.

### 2. O₂ Devices — `abg-o2.html#o2`
Six oxygen delivery devices, each with liter flow, FiO₂ range, low vs. high flow, humidification, and whether FiO₂ changes with the patient's rate / tidal volume:

| Device | Liter flow | FiO₂ | Flow |
| --- | --- | --- | --- |
| Nasal cannula | 1 – 6 L/min | 24 – 44% | Low |
| Simple face mask | 5 – 10 L/min | 35 – 50% | Low |
| Partial rebreather | 10 – 15 L/min (keep bag inflated) | 35 – 60% | Low |
| Non-rebreather | 10 – 15 L/min | 60 – 80% | Low |
| Venturi mask | 4 – 12 L/min | 24 – 60% | High |
| High-flow nasal cannula (HFNC) | Up to 60 L/min | 21 – 100% | High |

Includes a short explanation of why low-flow FiO₂ varies and high-flow FiO₂ doesn't, and a link to the O₂ Device Cases quiz. On a phone the table becomes one card per device.

### 3. O₂ Device Cases — `o2-cases.html`
A case-study quiz on oxygen devices. Each case gives you a patient (history, SpO₂, vitals, sometimes an ABG) and asks what you'd do. Every answer explains why it's right and why the other choices aren't.

- **40 cases in 4 types:**
  - **Pick the device (12):** e.g., the COPD CO₂ retainer already at target, cluster headache, carbon monoxide poisoning, pneumonia failing a non-rebreather, an infant with bronchiolitis, nasal packing, a claustrophobic patient.
  - **Troubleshoot (15):** e.g., a cannula hooked to the air flowmeter, a whistling humidifier, a Venturi set below its flow, HFNC prong size, a bad pulse-ox signal, a low cylinder before transport, a collapsing reservoir bag, a simple mask below 5 L/min, a dry nose on a cannula, raising a Venturi's FiO₂, blocked entrainment ports, the aerosol mist disappearing, HFNC humidity, mouth breathing, the non-rebreather's safety port.
  - **Next step (8):** HFNC failure, weaning FiO₂ in a preemie, stepping up a Venturi, opioid hypoventilation, hypercapnic failure needing BiPAP, CHF pulmonary edema needing CPAP/BiPAP, weaning off a non-rebreather, O₂-induced hypercapnia.
  - **Concepts (5):** why a cannula above 6 L/min barely helps, estimating cannula FiO₂, how breathing pattern changes low-flow FiO₂, partial rebreather vs. non-rebreather, which devices are high flow.
- **Quiz options:** filter by case type, choose 5, 10, 20 or all, and open the built-in device cheat sheet.
- **Results:** a score broken down by case type, with a review of your misses and a "Retry the missed" button.

### 3b. Med Cases — `med-cases.html`
A clinical-scenario quiz on respiratory medications, in the same format as the O₂ Device Cases. Every answer explains why, and links straight to that drug in the med chart.

- **167 application-based cases in 4 types:**
  - **Pick the drug (32):** add-on tiotropium for asthma, acute asthma, croup and post-extubation stridor, COPD maintenance, choosing a biologic, CF, apnea of prematurity, PCP prophylaxis, cromolyn before an allergen, end-of-life secretions, and more.
  - **Side effects & safety (47):** tobramycin ototoxicity, steroid-induced hyperglycemia, extra montelukast before exercise, tachycardia and tremor during treatment, thrush, theophylline toxicity and interactions, anticholinergic effects (glaucoma, urinary retention), anaphylaxis with biologics, duplicate-drug orders, LABA without an ICS, beta blockers in asthma, MAO inhibitors and epinephrine, colistin and gentamicin hazards, and more.
  - **Dosing & delivery (55):** dose calculations (caffeine loading dose, racemic epi and acetylcysteine mg, continuous albuterol volume), catching wrong orders (doses, units, frequency), inhaler technique (MDI, spacer, Diskus, Ellipta, HandiHaler, Respimat, QVAR), priming, ventilator delivery, the CF treatment order, mixing rules, diluents and storage.
  - **Next step (33):** ICS and pneumonia risk in COPD, single-inhaler triple therapy, judging response (peak flow, FEV₁, the silent chest), rescue-inhaler overuse, steroid tapers, when a treatment is needed early, and more.
- **Where they came from:** application-based questions from the course's respiratory pharmacology study set (de-duplicated, with a few corrected), the textbook's review questions, and cases written to fill in the drugs those didn't cover.
- **Roman-numeral questions** (I, II, III…) show the statements in a list, with the choices kept in their original order.
- **Quiz options:** filter by case type, choose 5, 10, 20 or all, and open the built-in drug-class cheat sheet.
- **Results:** a score by case type, a review of your misses with chart links, and a "Retry the missed" button.

### 4. O₂ Math & Gases — `gas.html`
- **Total flow (air-entrainment devices):** the air : O₂ ratio formula, the total flow formula, a ratio table (24% → 100%), the "total flow ≥ 3 × minute ventilation" rule, fixes for low flow, and the formula for the FiO₂ of a mixed gas.
- **Total flow calculator:** enter FiO₂ and O₂ flow (and optionally minute ventilation) to get the ratio, total flow, and whether it's adequate.
- **Cylinder duration:** the formula, step-by-step method, cylinder factors (D 0.16, E 0.28, M 1.56, G 2.41, H/K 3.14), and full-cylinder volumes.
- **Cylinder duration calculator:** pick a cylinder size, enter gauge pressure, safe residual and flow.
- **Medical gas cylinders:** US color code, what each gas is used for, and its pin index (PISS) for oxygen, medical air, heliox, helium, carbon dioxide, CO₂/O₂, nitrous oxide, nitrogen, cyclopropane and ethylene. Also PISS vs. ASSS vs. DISS and cylinder safety.

### 5. O₂ Math Quiz — `math-quiz.html`
A separate quiz for the calculations. You type your answer (or pick one for yes/no-style questions), check it, and see the worked solution.

- **Topics:** total flow, cylinder duration, or both.
- **Practice set:** the 15 worked problems (8 total flow, 7 cylinder duration), in a random order.
- **Random problems:** new numbers every time, for unlimited practice. Problem types:
  - total flow from the ratio table
  - working out an entrainment ratio
  - whether the total flow is adequate for the patient's minute ventilation
  - the FiO₂ of mixed O₂ and air
  - cylinder duration, with and without a safe residual
  - whether a cylinder will last a transport
  - the minimum gauge pressure needed
- **Choose 5–20 questions.** A **Hint** button shows the formulas, and **Show answer** gives you the solution if you're stuck.
- **Calculator:** tap the **Calculator** button (bottom right) for a pop-up calculator with + − × ÷, parentheses and %. **Use in answer** puts the result straight into your answer box. On a phone it opens as a compact panel and scrolls the question into view above it. The Med Cases page has the same calculator for the dose-calculation cases.
- **Flexible answers:** cylinder answers accept minutes or hours and minutes (“2 hr 48 min”, “2:48”). FiO₂ accepts a percent or a decimal. Small rounding differences are counted as correct.
- **Results:** a score at the end, a review of everything you missed with the worked solutions, and a “Retry the missed” button.

### 6. Medications — `meds.html#table`
The NBRC respiratory pharmacology chart: **46 drugs in 11 classes.** Each drug has brand names, category, strength, dosage, onset / peak / duration, mode of action, clinical effects and indications, adverse effects, contraindications, hazards, delivery device, and exam notes.

- **Classes:** sympathomimetics (β agonists), parasympatholytics (anticholinergics), combinations, xanthines, biologics, mast cell stabilizer, leukotriene modifiers, anti-infectives, mucolytics, corticosteroids, and diluents / bland aerosols.
- **Table view:** the full chart, with search, class filters, and "Hide answers" (tap a cell to reveal) for self-testing.
- **Cards view:** one expandable card per drug.
- **Flashcards:** study one field or everything, shuffle, mark cards known, and skip known cards (progress is saved on your device).
- **Quiz:** 83 hand-written NBRC-style questions (including textbook review questions on SABAs vs. LABAs, DPIs, DuoNeb/Combivent and ipratropium vs. atropine) plus auto-generated drug class and brand-name questions; choose 10, 20, 30 or all, then review your misses.

### 7. Mnemonics — `meds.html#mem`
The **Memory aids** tab of the medication chart:
- **The big picture:** sympathetic vs. parasympathetic, "1 heart, 2 lungs," cAMP vs. cGMP, and rescue vs. controller.
- **Read the ending, know the class:** 8 drug-name endings (-terol, -tropium / -clidinium, -sone / -nide / -olone, -lukast, -phylline, -mab, -mycin, -cillin).
- **50 class-by-class mnemonics and rules of thumb.** These include "can't see, can't pee," "Big Happy Dogs Chase After Squirrels" (the CF treatment order), the STEROIDS side-effect acrostic, Mean GNATS for aminoglycosides, and Anoro = "A-NO-roid."

---

## Files

| File | What it is |
| --- | --- |
| `index.html` | Landing page: site search, Look up / Practice paths, quick numbers, case of the day |
| `abg-o2.html` | ABG values and O₂ devices |
| `abg-practice.html` | ABG practice: unlimited random gases to interpret |
| `review.html` | Review my mistakes: every missed question from every quiz |
| `gas.html` | O₂ math (total flow, cylinder duration) with calculators, and medical gas cylinders |
| `o2-cases.html` | O₂ Device Cases: case-study quiz on choosing and troubleshooting O₂ devices |
| `med-cases.html` | Med Cases: clinical-scenario quiz on respiratory medications |
| `math-quiz.html` | O₂ Math Quiz: graded total flow and cylinder duration problems |
| `meds.html` | Medication chart: table, cards, flashcards, quiz, memory aids |
| `apple-touch-icon.png` | The lung icon people see when they add the site to their phone's home screen |
| `sw.js` | The offline helper (service worker): saves the pages so the site works without internet |
| `manifest.webmanifest` | App info for phones: the name, icon and colors used by "Add to Home Screen" |
| `icon-192.png`, `icon-512.png` | App icons used by the manifest (Android and desktop) |
| `README.md` | This file |

There's no build step and no dependencies. Each page is a single HTML file.

Old links and bookmarks to `index.html#abg` or `index.html#o2` still work: they forward to `abg-o2.html`.

## Put it online with GitHub Pages

1. Create a new repository on GitHub.
2. Click **Add file → Upload files**, drag in all thirteen files, then **Commit changes**. (When updating, upload the new versions to replace the old ones.)
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick `main` and `/ (root)`, then **Save**.
5. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`.

Tip: on your phone, open the site and use **Add to Home Screen**. It saves as **Pocket Pulmo** with the lung icon and opens like an app.

## Offline use

Pocket Pulmo works without internet after it's been opened once online.

- **How:** on the first visit, the browser installs `sw.js` in the background, and it saves a copy of every page. Online, pages always load fresh from GitHub, so updates show up right away, and the saved copy is refreshed. Offline, or if the connection takes more than about 4 seconds, the saved copy is used. Search, quizzes, calculators and flashcards all keep working.
- **Updates:** just upload new files as usual. `sw.js` is rebuilt with every update, so old saved copies are cleared automatically.
- **iPhone tip:** use **Add to Home Screen**. Home-screen apps keep their offline copy most reliably, and Safari may clear saved data for sites that haven't been opened in a while.
- **Fonts:** saved after the first online visit. If they weren't saved yet, the site uses the phone's built-in fonts.
- Offline mode only works on the live (https) site, not when a page is opened as a file on your computer.

## Editing

- **ABG values and O₂ devices:** edit the text directly in `abg-o2.html`.
- **Total flow, cylinder duration and gas cylinders:** edit the text directly in `gas.html`.
- **Device cases:** in `o2-cases.html`, the cases are the `CASES = [ ... ]` array near the bottom. The comment above it explains each field, and you can add your own case by copying one.
- **Med cases:** in `med-cases.html`, the cases are the `CASES = [ ... ]` array near the bottom (same format as the O₂ cases, plus `d`, the drug names to link to in the chart).
- **Math quiz problems:** in `math-quiz.html`, the practice set is the `FIXED = [ ... ]` array (the comment above it explains each field). The random problem generators are in `GEN`.
- **Medications:** in `meds.html`, the drug list is the `D = [ ... ]` array and the quiz questions are the `QUIZ = [ ... ]` array inside the `<script>` near the bottom. Each entry's fields are explained in the comment above it.
- **Mnemonics:** also in `meds.html` — `MEM_BIG` (big-picture cards), `MEM_SUFFIX` (name endings), and `MEM` (cards for each drug class).

- **ABG practice:** the logic is the `window.ABG` script in `abg-practice.html` (normal ranges in `N`, practice patterns in `PATTERNS`).
- **Site search:** each page has its own copy of the search list (`window.RTQ_INDEX`). If you add a drug, case or mnemonic by hand, it shows up on its page right away, but it won't appear in search until that list is rebuilt.

Flashcard progress, your mistakes deck, filters, quiz settings and your last-used tab are saved in your browser, per device.

> For exam study. Ranges, doses and ratios vary slightly between textbooks and facilities. Always follow your program's references, your facility's policies, and the current order / package insert in clinical practice.
