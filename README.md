# Concussion Hub

An evidence-based clinical reference on **concussion and mild traumatic brain injury** —
mechanism, assessment, management, persisting symptoms and long-term risk.

Built on the **Amsterdam 2023 international consensus** (6th International Conference on
Concussion in Sport) together with the systematic reviews, randomised trials and cohort
studies published since, across **90 peer-reviewed sources**.

---

## What's in it

| | |
|---|---|
| **24 sections** | Pathophysiology · biomechanics · red flags · CRT6 / SCAT6 / SCOAT6 · vestibulo-ocular and cervical examination · imaging and blood biomarkers · differential diagnosis · return to learn and return to sport · exercise as treatment · targeted rehabilitation · persisting symptoms · prognosis · biopsychosocial factors · repetitive head impacts and CTE · special populations · prevention |
| **9 calculators** | 22-item symptom scale · mSIT 6-item screen · VOMS scorer · modified BESS and tandem gait · Buffalo Concussion Treadmill Test prescription · return-to-sport and return-to-learn trackers · risk stratification · orthostatic vitals |
| **3 audience views** | **Clinician** (24 sections) · **Athlete & coach** (18) · **Patient & family** (14). Switching filters whole sections, the calculators and the contents list |
| **Full-document search** | Highlights every match, steps through them, and tells you when matches sit in sections your current view hides |
| **Selective printing** | Choose exactly which sections to print, with a live page estimate |
| **Two themes** | *Manuscript* (parchment) and *Midnight*. Every text pair meets WCAG AA |
| **Works offline** | Installable to a home screen or dock; fully usable pitch-side or in clinic with no signal |

---

## Publishing it on GitHub Pages

No build step and no command line needed.

1. **Create a repository.** On GitHub, click **+ → New repository**. Name it `concussion-hub`,
   set it to **Public**, and click **Create repository**.
2. **Upload the files.** On the new repo page choose **uploading an existing file**, then drag in
   *everything inside this folder* — `index.html`, `manifest.webmanifest`, `service-worker.js`,
   `.nojekyll`, the `icons` folder, and these markdown files. Click **Commit changes**.
3. **Turn on Pages.** Go to **Settings → Pages**. Under *Build and deployment* set
   **Source** to `Deploy from a branch`, **Branch** to `main` and the folder to `/ (root)`.
   Click **Save**.
4. **Wait about a minute**, then reload the Settings → Pages screen. Your link appears at the top:

   ```
   https://<your-username>.github.io/concussion-hub/
   ```

> **Keep the folder structure.** `icons/` must stay a folder next to `index.html`, or the
> icons and offline support will not work. Every path in the project is relative, so the
> site works from any repository name without editing anything.

### Updating it later

Open the repo, click `index.html`, then the pencil icon, paste the new content and commit —
or use **Add file → Upload files** and drop the replacement in. Pages redeploys automatically.

Returning visitors get the new version immediately: the service worker fetches the document
from the network first and only falls back to its cache when offline. If someone has the app
open when you publish an update, a small prompt offers them a reload.

### Using it without GitHub

`index.html` is entirely self-contained — no frameworks, no CDN, no external requests.
Double-clicking it opens the full application in any modern browser. Offline install and
icons are the only features that need it to be served over `https://`.

---

## Clinical scope and currency

The Amsterdam 2023 statement remains the current international consensus; the 7th consensus
statement is anticipated but not published as of August 2026. Content also incorporates
systematic reviews, randomised trials and cohort studies through 2026, plus national guidance
including the 2025 Australia / Aotearoa New Zealand mTBI guidelines.

Effect estimates are given with confidence intervals where available. Where evidence is weak,
contested or extrapolated, this is stated rather than smoothed over — several findings cited
(the mSIT, parts of the SCOAT6 validation) come from single cohorts and are not yet in
consensus guidance.

## Disclaimer

This resource is **educational**. It is not a substitute for individual clinical assessment,
diagnosis or treatment, and it does not establish a clinician–patient relationship. Concussion
is a clinical diagnosis made by a qualified healthcare professional.

The interactive tools reproduce published scoring conventions for teaching and clinical-support
purposes. **They are not validated medical devices** and must not be used as the sole basis for
return-to-play, return-to-work or clearance decisions.

If you have sustained a head injury and have any red flag feature — worsening headache, repeated
vomiting, seizure, weakness or numbness, slurred speech, unusual drowsiness or escalating
confusion — **seek emergency medical care immediately**.

## Licence

Released under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](LICENSE)
(CC BY-NC-SA 4.0). You may share and adapt it for non-commercial purposes with attribution, and
derivatives must carry the same licence. See `LICENSE` for the full terms.

## Citing it

See [`CITATION.cff`](CITATION.cff), or cite as:

> *Concussion Hub: an evidence-based clinical reference on concussion and mild traumatic brain
> injury.* 2026. https://github.com/&lt;your-username&gt;/concussion-hub
