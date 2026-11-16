# ALSKwela JHS ALS A&E Reviewer — LS 1 Filipino

## Contents
- index.html: working mobile-first reviewer, all 120 questions EMBEDDED; no network requests or external libraries.
- manifest.webmanifest: **JHS ALS A&E Reviewer LS 1 - Filipino**; home-screen short name **JHS A&E LS1 Filipino**.
- sw.js: Filipino-specific service worker, safe alongside JHS English on GitHub Pages.
- icon-192.png and icon-512.png: Filipino-specific PWA icons.
- .nojekyll: for reliable GitHub Pages root deployment.

## Deploy to GitHub Pages
1. Create a **separate** repository, suggested: `alskwela-ls1-filipino-reviewer-jhs`.
2. EXTRACT the ZIP and upload the root files (NOT the ZIP itself) to the repository root. Include all five named app files and `.nojekyll`.
3. GitHub repository → Settings → Pages → Deploy from a branch → `main` / (root).
4. Open the HTTPS URL in Chrome **directly**, not solely in the Glide in-app browser. Wait until the offline-ready message appears. Install/Add to Home Screen; test airplane mode.
5. In ALSKwela Glide, add a JHS LS1 Filipino Reviewer card with Open Link action to that new HTTPS URL.

**Important**: Existing LS1 English site is a DIFFERENT reviewer. Keep the two PWAs in separate repositories/paths. Never replace your JHS English index or sw.js with Filipino files. Unique localStorage keys and distinct cache prefixes avoid collisions even on the same GitHub Pages origin.

## Reviewer usage
- Fixed Sets A/B/C: 40 questions each; cover all 22 numbered LCs, with 12 Easy / 20 Moderate / 8 Challenging.
- Balanced Random: 40 from 120, with a competency blueprint and 12/20/8 mix; tracks seen items for later trials.
- Feedback immediately after submission, Filipino explanation after every question.
- Resume progress via local device storage.
- End report: score, question responses and answer explanations; use **Download PDF** or Chrome Print → Save as PDF, including for accented Filipino characters.

## Academic QA limitations
- First-draft simulation of the 2026 revised CG. NOT official BEA test items or a verified 2027 prediction.
- Multiple choice evaluates decisions underlying composition/performance, not the full actual performance competencies.
- Manual SME review and learner pilot/psychometric item analysis are recommended before high-stakes use.
- Offline storage is tied to one browser and device and can be cleared. No cloud sync/teacher dashboard yet.
- Changing data or names later requires updating cache version in sw.js and in index.html OFFLINE_CACHE.
