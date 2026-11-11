# Designwhich evidence record

Reviewed 7 November 2026. This record distinguishes direct user choices, published values, observed patterns, and defects. It supports design decisions, not independent verification of Parth’s biography or project outcomes.

## Authority

**U1, direct user choices.** Parth requested a personal design system derived from Designwhich, chose adaptable principles and an audit plus reusable skill, and described the current site as a starting point to refine. The live website is not a blanket requirement to repeat every treatment.

**Published values.** The [Playbook](https://designwhich.works/playbook/) states the following. Treat them as values published on the site; do not invent additional first-person beliefs.

| ID | Value in practical terms |
|---|---|
| P1 | Understand the person’s situation before choosing features. |
| P2 | Consider the complete journey and related touchpoints. |
| P3 | Prototype input, timing, motion, and response when behavior matters. |
| P4 | Share decision reasoning with collaborators and work close to implementation. |
| P5 | Adapt to changing constraints while retaining coherence. |
| P6 | Make consequential choices clear and exercise restraint around money, identity, and ambient AI. |
| P7 | Use experiments, fabrication, and creative practice to learn. |
| P8 | Give people enough context to act, change course, and recover. |

## Observed patterns

| ID | Evidence | Supported interpretation and boundary |
|---|---|---|
| O1 | [Home](https://designwhich.works/), [Work](https://designwhich.works/work/), [About](https://designwhich.works/about/) | Display typography, neutral surrounding surfaces, compact controls, and large artifacts recur. Home uses Nikolas; tested project openings use General Sans. This supports deliberate type roles and content-led composition, not mandatory fonts or a universal dark theme. |
| O2 | [Mentra](https://designwhich.works/mentra/), full story | App access, runtime identity, listening/working/uncertainty, and specific recovery actions receive explicit design attention. Original screens have decision and reading captions. Public results include missing study-context qualifications. This supports understandable behavior; it does not independently prove outcome claims. |
| O3 | [Jugalbandi](https://designwhich.works/jugalbandi/), [Enigma](https://designwhich.works/enigma/) | Acoustic mechanisms and a light sculpture turn technical processes into physical experiences. The pages distinguish original evidence from explanatory browser adaptations. This supports tangible explanation and operable exploration when useful, not a requirement for 3D in every interface. |
| O4 | [Raahi](https://designwhich.works/raahi-project/), [TransFi public preview](https://designwhich.works/transfi-project/) | Service touchpoints and a financial system have distinct visual identities. Later prototypes are identified separately from earlier work. Private prototypes were not entered. This supports domain-specific design and accurate presentation, not a shared product palette. |
| O5 | [Butler’s Slice](https://designwhich.works/typeface/) | Diagonal cuts connect the font to a material gesture; a live specimen exposes text and weight controls. The compact specimen responded to edited text and Bold selection. This supports typographic authorship and usable demonstrations, not using this font for body text everywhere. |
| O6 | [Graveyard](https://designwhich.works/graveyard/), [About](https://designwhich.works/about/) | An illustrated day/night archive, tombstone metaphor, dry humor, and personal creative-practice material allow expressive variation. This supports play with a coherent purpose. The archive’s historical descriptions were not independently verified. |

## Local implementation reference

**D1.** Local checkout the inspected portfolio checkout, HEAD `3d7b1d8c108c1d37189c6a7acb1b06b411730351`. Relevant sources are `docs/portfolio-design-system.md`, `DESIGN.md`, `src/styles/tokens.css`, `src/styles/display-type.css`, and `src/data/playbook.ts`.

The documentation describes an editorial technical portfolio, stable media, accessible controls, readable prose, lazy heavy features, and reduced motion. The source contains Nikolas and General Sans, warm light and dark tokens, spacing and motion scales, glass surfaces, and project-specific exceptions. The live Mentra and other case studies include newer presentation structures than this checkout. Never assume checkout and deployment match.

## Findings that must not become taste rules

- **F1, confirmed route-history dependency.** At 1440px, direct Playbook entry had a computed 16px h1 and 0px main top padding. Following UX Design and then Playbook in the same tab changed those to 89.6px and 152px. The local `.pb-*` rules live in `landing.css`, imported by `CategoryPage.tsx`, while `PlaybookPage.tsx` does not import it. This supports a stylesheet dependency diagnosis; the deployment build itself was not changed or rebuilt.
- **F2, mobile hierarchy.** At 390 × 844, Home placed the scene above a large empty interval and the introduction near the lower part of the viewport. This is an observed composition with a recommended improvement, not measured evidence of user abandonment.
- **F3, competing chrome.** Assistant and optional tool UI can sit over content in reviewed views. The mobile specimen’s lower navigation overlapped the specimen area in the captured view. This supports checking actual positioning and focus, not banning all persistent controls.
- **F4, small display text.** Graveyard’s inscription details and the mobile full specimen’s split weight labels are difficult to scan in the screenshots. Contrast ratios were not measured. Preserve the concept while improving legibility.
- **F5, source naming drift.** The local `--mono` stack begins with General Sans despite documentation calling for mono labels; `--ink-40` and `--ink-30` no longer describe their opacity values. Motion has two token families. These are maintainability findings, not new visual requirements.
- **F6, attribution limits.** Site presence does not establish that every choice expresses a permanent preference. Metrics, job titles, dates, and original technical claims require their own verification before reuse. Published values and inferred visual taste remain distinct.

The actionable audit evidence and selected screenshots are bundled in this skill.

## Bundled visual evidence

On 10 November 2026, Parth asked to add images and references to make the skill's application more faithful. The [visual guide](visual-references.md) now annotates 24 unmodified local images. Eighteen are screenshots from the 7 November audit, and six are images from the local project archive. The [manifest](visual-manifest.json) records their source paths, page links, dimensions, classifications, and hashes. The copies live under this reference directory, so the skill can inspect them without access to the original workspace.

V01–V21 cover editorial direction, project framing, decision evidence, different identities, physical construction, typography, and purposeful play. C01–C03 are explicitly labeled counterexamples. Some other references carry narrower boundaries, such as atmosphere only or before-state comparison. Apply their annotations rather than treating every visible detail as an endorsed preference. These are historical captures; the bundle does not establish the current website's rendering.
