# Portfolio foundation references

These values come from the local portfolio `src/styles/tokens.css` at commit `3d7b1d8c108c1d37189c6a7acb1b06b411730351`. Read on 10 November 2026. Use them to understand the existing system or as a starting reference when a brief asks for a related direction. A new product may need different values. Project-specific overrides mean a source token does not establish every pixel in a screenshot.

## Color roles

| Role | Light reference | Dark reference |
|---|---|---|
| Canvas | `#FAFAF8` | `#111110` |
| Alternate canvas | `#F2F1EE` | `#1A1918` |
| Surface | `#FFFFFF` | `#222220` |
| Main ink | `#1A1A1A` | `#EDEDEC` |
| Quiet high accent | `#A8B8D8` | Same source token; inspect the actual surface |

These are neutral surrounding surfaces. V09, V10, V11, V14, and V17 in the [visual references](visual-references.md) show how project content supplies stronger color. The reference supports color with a role, not one favorite accent for all work.

Muted ink tokens in the source use opacity and have historically misleading names. Choose semantic roles such as primary, secondary, disabled, border, and decoration in a new system, then verify the actual foreground/background pairs. Do not copy opacity values or source contrast comments as proof of accessibility in a different context.

## Type roles

| Role | Existing reference | How to interpret it |
|---|---|---|
| Large editorial display | Nikolas, regular | Character and fine detail at sufficient size; V01 and V19 |
| Body and UI | General Sans | Plain support for reading and operation; V03 and V06 |
| Small readable serif fallback | Charter, Iowan Old Style, Georgia | The source distinguishes small reading text from delicate display forms |
| Project typography | Butler's Slice, three supplied weights | A project-specific construction language; V14–V16 |

The token named `--mono` resolves to General Sans first. It is not evidence of a real monospace family. The tested project opening titles use sans type even though the broad display rule uses Nikolas elsewhere.

The source's nominal scale includes 11, 12, 13, 16, 18, 24, 32, and 48px equivalents. The hero token is `clamp(3.5rem, 8vw, 6rem)`. Body line height is 1.65 and relaxed reading is 1.75. These describe the source; the small end of the scale is not a recommendation for essential text. Use legible sizes suited to the display and task.

## Spacing and shape

The source uses a spacing sequence of 4, 8, 12, 16, 24, 32, 48, 64, and 96px equivalents. Its shared gutter is `clamp(1.25rem, 4vw, 3rem)`. Local reading guidance describes a separate 1040px maximum frame for case studies and a readable 65–75-character measure for prose. Different content types need different widths and density.

The core radius tokens are 4, 8, and 12px, with a 10px token named pill. Project media and specialist surfaces have exceptions. Use a consistent shape vocabulary for a new project rather than copying a radius based only on its token name. The mobile captures C01–C03 show why spacing and control layout still need rendered checks.

## Motion and depth

The `--motion-*` family has 180ms fast, 360ms base, 620ms slow, and 70ms stagger values. The principal motion ease is `cubic-bezier(0.16,1,0.3,1)`. A separate `--dur-*` family uses 150, 250, 400, and 700ms. Choose one coherent vocabulary for a new implementation rather than copying both families. Exact timing remains specific to the interaction.

The portfolio includes glass, shadows, 3D form, and atmospheric scenes. Study their purpose in the images: shared floating chrome, visible object construction, or a complete archive setting. A flat operational surface may need none of them. Still images cannot establish animation quality, reduced-motion handling, sound behavior, or idle rendering cost.

## Applying a reference

State which relationship you are borrowing: editorial display with readable support, a quiet frame around strong media, a legible input-to-output mechanism, or a concept carried across an experience. Make the choice using the actual brand and content. Check the rendered type, spacing, controls, responsive behavior, and relevant states before judging the match.
