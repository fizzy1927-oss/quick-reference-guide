# RT Quick Reference

A sage-green study site for respiratory therapy students preparing for the NBRC TMC / CSE exams. It's built for quick lookups on a phone or laptop: no logins, no installs, and it follows your device's light/dark setting.

Every page shares one navigation bar: **ABG Values · O₂ Devices · O₂ Device Cases · O₂ Math & Gases · O₂ Math Quiz · Medications · Mnemonics**.

---

## What's on the site

### 1. ABG Values — `index.html#abg`
Normal adult arterial blood gas values (room air, sea level), each with what a high or low value means:

| Value | Normal range |
| --- | --- |
| pH | 7.35 – 7.45 |
| PaCO₂ | 35 – 45 mmHg |
| HCO₃⁻ | 22 – 26 mEq/L |
| PaO₂ | 80 – 100 mmHg |
| SaO₂ | 95 – 100% |
| Base excess | −2 to +2 mEq/L |

Plus the **ROME** rule (Respiratory Opposite, Metabolic Equal).

### 2. O₂ Devices — `index.html#o2`
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

- **28 cases in 4 types:**
  - **Pick the device (10):** e.g., the COPD CO₂ retainer, carbon monoxide poisoning, pneumonia failing a non-rebreather, an infant with bronchiolitis, nasal packing, a claustrophobic patient.
  - **Troubleshoot (9):** e.g., a collapsing reservoir bag, a simple mask below 5 L/min, a dry nose on a cannula, raising a Venturi's FiO₂, blocked entrainment ports, the aerosol mist disappearing, HFNC humidity, mouth breathing, the non-rebreather's safety port.
  - **Next step (5):** opioid hypoventilation, hypercapnic failure needing BiPAP, CHF pulmonary edema needing CPAP/BiPAP, weaning off a non-rebreather, O₂-induced hypercapnia.
  - **Concepts (4):** estimating cannula FiO₂, how breathing pattern changes low-flow FiO₂, partial rebreather vs. non-rebreather, which devices are high flow.
- **Quiz options:** filter by case type, choose 5, 10, 20 or all, and open the built-in device cheat sheet.
- **Results:** a score broken down by case type, with a review of your misses and a "Retry the missed" button.

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
- **Flexible answers:** cylinder answers accept minutes or hours and minutes (“2 hr 48 min”, “2:48”). FiO₂ accepts a percent or a decimal. Small rounding differences are counted as correct.
- **Results:** a score at the end, a review of everything you missed with the worked solutions, and a “Retry the missed” button.

### 6. Medications — `meds.html#table`
The NBRC respiratory pharmacology chart: **46 drugs in 11 classes.** Each drug has brand names, category, strength, dosage, onset / peak / duration, mode of action, clinical effects and indications, adverse effects, contraindications, hazards, delivery device, and exam notes.

- **Classes:** sympathomimetics (β agonists), parasympatholytics (anticholinergics), combinations, xanthines, biologics, mast cell stabilizer, leukotriene modifiers, anti-infectives, mucolytics, corticosteroids, and diluents / bland aerosols.
- **Table view:** the full chart, with search, class filters, and "Hide answers" (tap a cell to reveal) for self-testing.
- **Cards view:** one expandable card per drug.
- **Flashcards:** study one field or everything, shuffle, mark cards known, and skip known cards (progress is saved on your device).
- **Quiz:** 78 hand-written NBRC-style questions plus auto-generated drug class and brand-name questions; choose 10, 20, 30 or all, then review your misses.

### 7. Mnemonics — `meds.html#mem`
The **Memory aids** tab of the medication chart:
- **The big picture:** sympathetic vs. parasympathetic, "1 heart, 2 lungs," cAMP vs. cGMP, and rescue vs. controller.
- **Read the ending, know the class:** 8 drug-name endings (-terol, -tropium / -clidinium, -sone / -nide / -olone, -lukast, -phylline, -mab, -mycin, -cillin).
- **50 class-by-class mnemonics and rules of thumb.** These include "can't see, can't pee," "Big Happy Dogs Chase After Squirrels" (the CF treatment order), the STEROIDS side-effect acrostic, Mean GNATS for aminoglycosides, and Anoro = "A-NO-roid."

---

## Files

| File | What it is |
| --- | --- |
| `index.html` | Home page: ABG values and O₂ devices |
| `gas.html` | O₂ math (total flow, cylinder duration) with calculators, and medical gas cylinders |
| `o2-cases.html` | O₂ Device Cases: case-study quiz on choosing and troubleshooting O₂ devices |
| `math-quiz.html` | O₂ Math Quiz: graded total flow and cylinder duration problems |
| `meds.html` | Medication chart: table, cards, flashcards, quiz, memory aids |
| `README.md` | This file |

There's no build step and no dependencies. Each page is a single HTML file.

## Put it online with GitHub Pages

1. Create a new repository on GitHub.
2. Click **Add file → Upload files**, drag in all six files, then **Commit changes**. (When updating, upload the new versions to replace the old ones.)
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick `main` and `/ (root)`, then **Save**.
5. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`.

Tip: on your phone, open the site and use **Add to Home Screen** so it opens like an app.

## Editing

- **ABG values and O₂ devices:** edit the text directly in `index.html`.
- **Total flow, cylinder duration and gas cylinders:** edit the text directly in `gas.html`.
- **Device cases:** in `o2-cases.html`, the cases are the `CASES = [ ... ]` array near the bottom. The comment above it explains each field, and you can add your own case by copying one.
- **Math quiz problems:** in `math-quiz.html`, the practice set is the `FIXED = [ ... ]` array (the comment above it explains each field). The random problem generators are in `GEN`.
- **Medications:** in `meds.html`, the drug list is the `D = [ ... ]` array and the quiz questions are the `QUIZ = [ ... ]` array inside the `<script>` near the bottom. Each entry's fields are explained in the comment above it.
- **Mnemonics:** also in `meds.html` — `MEM_BIG` (big-picture cards), `MEM_SUFFIX` (name endings), and `MEM` (cards for each drug class).

Flashcard progress, filters, quiz settings and your last-used tab are saved in your browser, per device.

> For exam study. Ranges, doses and ratios vary slightly between textbooks and facilities. Always follow your program's references, your facility's policies, and the current order / package insert in clinical practice.
