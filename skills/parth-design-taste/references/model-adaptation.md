# Adapting to the working model and tools

Use this reference when model capabilities, provider behavior, context limits, or available tools affect how the design work can be performed. Keep the company being designed for separate from the model provider. A provider's brand is not the client's design direction.

The business or service model belongs in [company context](company-context.md). This reference concerns the assistant doing the work.

## Establish what is actually available

Use the active environment and tool descriptions to establish capabilities. Record the exact model and provider only if the environment exposes them or the user supplies them; otherwise leave them unknown. Do not infer abilities from a name, price tier, or provider stereotype.

| Available capability or constraint | Adaptation |
|---|---|
| Image understanding and a usable image viewer | Open the existing company's relevant screen and a small set of taste images. Compare specific traits in the pixels. |
| Text-only input or images that cannot be opened | Use the captions, evidence, and foundations as partial context. State that image fidelity is unverified. Do not claim to have seen the references. |
| Code and a local runtime | Use the existing framework and components. Build the representative behavior and inspect the result when a preview tool is available. |
| Browser or application inspection | Check relevant sizes, states, focus, and behavior in the actual rendered surface. |
| Code access without a rendered preview | Perform the applicable code and structural checks, then distinguish those from visual verification. |
| Design-tool access | Follow that tool's applicable skill and native component/token system. Do not claim a design-file update when only code or instructions were produced. |
| A constrained context or handoff | Carry the current project brief, selected reference IDs, decisions, and next check. Read other references only when they become relevant. |
| Limited tool access or a short task | Reduce the scope of the working slice and the amount of explanation. Keep the agreed design quality and report what remains unverified. |

Use only supported capabilities. Do not switch models, change provider settings, purchase access, or install the skill into another assistant merely to apply this guidance. Follow a user's explicit request if they ask for one of those changes.

## Tailor the working instructions

Start with the audience, task, company constraints, and observable result. Select only the references that affect the next decision. Keep the underlying taste consistent while adapting how the work is expressed:

- For a task that benefits from a short working brief, provide constraints, one representative example, and the next observable check.
- For a complex design question, compare concrete alternatives against the same audience, workflow, and brand requirements. Do not add alternatives simply to fill a quota.
- If the output misses a requirement, correct the specific mismatch with evidence and a bounded next step. Do not keep appending broad style adjectives.
- If a capability is missing, choose an available route and state the practical limit. Do not substitute an invented screenshot, benchmark, or visual inspection.

When the task actually depends on model-specific prompting, API parameters, or tool behavior, consult current official documentation for that exact model and provider. Preserve a user-specified model. Record the source and date for any persistent model-specific rule; do not maintain unsupported brand-name presets here.

## Combine useful decisions across model outputs

When comparing alternatives from the same brief, inspect them at the same viewport and exercise the same task and recovery paths. Borrow individual decisions that improve the project. The Mentra comparison paired one output's compact device row with the other's more legible primary button. The Designwhich comparison paired simple navigation with a compact introduction and a project preview sheet. Recheck the combined result, including asset paths and state copy. Attribute findings to the observed outputs from that run.

## Portable working packet

When a handoff is requested or context needs to be reduced, use a compact packet such as:

```text
Design task and current state:
Company / product / audience / business model:
Brand and existing system to preserve:
Relevant taste principles and selected image IDs or paths:
Chosen direction and important tradeoffs:
Runtime capabilities and verification limits:
Requested artifact or implementation slice:
Acceptance checks and next action:
```

Include only the needed material. For an assistant that cannot access this skill's files, supply the selected reference images or their honest text descriptions through an available, authorized route. An ID such as V12 has no visual meaning without its image or annotation. Do not imply that Codex's automatic skill rule also configures another application or provider.

The small entrypoint and selective reference loading follow the progressive-disclosure approach described in [official OpenAI documentation](https://learn.chatgpt.com/docs/customization/overview#skills), checked 10 November 2026. The capability-based workflow above is a design-process choice, not a benchmark or a claim that a particular model is better at design.
