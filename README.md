# AI Act Triage

A one-page tool that classifies an AI system under the EU AI Act (Regulation (EU) 2024/1689, as amended by the AI Omnibus) in about a minute.

Answer six questions and get:

- **The risk tier**: outside scope, prohibited, high-risk, transparency risk or minimal risk
- **The provisions that apply**, split by role (provider or deployer), with article references
- **The key dates**, marked as already in force or still upcoming
- **An assessment note** you can copy into an email or a file note

Five built-in examples (CV screening, customer chatbot, credit scoring, spam filter, staff emotion monitoring) show how the logic works.

## How the classification works

The questions follow the order of the Regulation's own tests:

| Step | Test | Provision |
|---|---|---|
| 1 | Scope exclusions (military, research, personal use) | Art. 2 |
| 2 | Role | Art. 3 |
| 3 | Prohibited practices | Art. 5 |
| 4 | Safety component of a regulated product | Art. 6(1), Annex I |
| 5 | Use in a sensitive area | Art. 6(2), Annex III |
| 6 | Filter for low-impact Annex III uses (never available with profiling) | Art. 6(3) |
| 7 | Transparency situations, which stack on any tier | Art. 50 |
| 8 | General-purpose AI models | Art. 51–55 |

Application dates reflect the AI Omnibus: Annex III high-risk obligations from 2 December 2027, Annex I from 2 August 2028, and the new prohibition on generating non-consensual intimate imagery from 2 December 2026.

## Run it

It is a single HTML file with no build step. Open `index.html` in a browser, or publish it with GitHub Pages (Settings → Pages → deploy from the `main` branch).

`src/app.html` is the same page without the document wrapper, used for hosted previews.

## Disclaimer

This is a first-pass triage aid, not legal advice. It simplifies the Regulation's tests and exceptions. Verify any result against the consolidated text in the Official Journal.
