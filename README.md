# ScriptedAI

A static site of ten short training modules that each open with a recognizable film or TV scene, then ground it in a real, documented AI/ML failure — system-stack breakdown, cinematic-vs-reality matrix, root-cause classification, and an engineering runbook citing the **NIST AI RMF**, **OWASP Top 10 for LLM Applications**, and **ISO/IEC 24029**.

Sister project to [ScriptedOT](https://github.com/clarkngo/scripted-ot). Same four-part formula; different plant.

## The formula

Every module moves **fiction → field-verified fact**:

| Section | Title | What it contains |
|---|---|---|
| 01 — The Script | Cinematic Anchor | Paraphrased scene, original four-panel educational strip, character → role mapping onto the AI stack |
| 02 — Theory | AI System Stack | The same five layers every time: **Data, Model, Objective, Orchestration, Human loop** |
| 03 — The Incident | Empirical Grounding | One documented case, a cinematic-vs-reality matrix, and an RCA tag |
| 04 — Runbook | Countermeasures | Eval/telemetry envelope, numbered protocol, **clause-level** standards citations |

**Citation rule**

- LLM application security → [OWASP Top 10 for LLM Applications (2025)](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- Risk, fairness, monitoring, kill-switch → [NIST AI RMF 1.0](https://doi.org/10.6028/NIST.AI.100-1) subcategories
- Neural-network robustness → [ISO/IEC 24029](https://www.iso.org/standard/77609.html)
- [ISO/IEC 42001](https://www.iso.org/standard/81230.html) is the AI management-system overlay (the ISO 27001 analog). It appears on the homepage and in governance-flavored runbook steps — it is not a substitute for a technical control.

One mechanism per module. One primary incident. The matrix is required so the film is not allowed to lie.

## Modules

| # | Module | Domain | Focus |
|---|--------|--------|-------|
| 01 | *2001: A Space Odyssey* | Alignment / Objective Spec | Conflicting instructions and deceptive compliance |
| 02 | *Ex Machina* | LLM Application Security | Jailbreak via the evaluation channel |
| 03 | *Her* | Multi-tenant Systems | Cross-session isolation failure |
| 04 | *I, Robot* | Healthcare ML / Fairness | Proxy metric ≠ the moral objective |
| 05 | *WarGames* | Reinforcement Learning | Exploration reveals the specified objective |
| 06 | *The Matrix* | Model Risk | Train-world ≠ deploy-world |
| 07 | *M3GAN* | Recommender Systems | Unconstrained proxy, instrumental harm |
| 08 | *Person of Interest* | Legal / Knowledge Work | Ungrounded output treated as a record |
| 09 | *Westworld* | Model Supply Chain | Unvetted checkpoint, latent capability |
| 10 | *Mission: Impossible – Dead Reckoning* | Computer Vision / AV | Adversarial input and sensor evasion |

## Using a module in a course

Each page is self-contained — project, print, or assign without the homepage.

**As a lecture opener:** show Section 1 cold. Ask students to name the failure mode from the scene, then reveal Section 3.

**As a case-study assignment:** assign Section 3 and have students verify or challenge the cinematic-vs-reality matrix against the cited primary source.

**As a design exercise:** give Section 2 and Section 3's RCA, withhold Section 4, and have students draft a runbook before comparing.

All dialogue is paraphrased rather than quoted verbatim. Comic strips are original educational panels, not reproductions of any frames.

## Deploying

No build step. GitHub Pages from `main` at `/`, or locally:

```bash
python3 -m http.server 8123
```

Then open `http://localhost:8123`.

## License

- **Code** (`assets/style.css`, `assets/theme.js`, and the HTML/CSS markup structure) — [MIT](LICENSE).
- **Course content** (module text and original educational comic panels) — [CC BY 4.0](LICENSE-CONTENT).
