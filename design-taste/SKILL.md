---
name: design-taste
description: Use when making visual/UI design decisions or judging whether a design is any good - choosing color, type, spacing, motion, hierarchy; building an app screen, landing page, or component; or reacting to "make it look good/premium/modern/less cheap". Encodes durable design judgment (not just current fads) so output reads as crafted rather than AI-default. Triggers - "design a UI", "make it premium", "it looks cheap/generic", "pick colors", "landing page", "improve the visual design", "does this look good".
---

# Design Taste

## Overview

**Every trend is a costume over five timeless moves.** Encode the moves as law; treat the costumes (specific palettes, gradients, typefaces) as swappable and dated.

**The thesis that matters most in 2026:** AI can generate competent UI for free, so *default output is the new cheap.* Anything a template ships is depreciating. Distinctiveness and craft are the moat — and both come from judgment, not from copying what's trending.

Use this to make design decisions, or as a checklist when reviewing a screen and asking "why does this feel cheap / generic?"

## When to Use
- Choosing color, type, spacing, motion, or layout for any UI.
- Building an app screen, landing page, dashboard, or component.
- Reacting to "make it premium," "it looks generic," "improve the visuals."

**When NOT to use:** information architecture, copywriting, or product logic — those come *first* (see Guardrails), this is the visible 10% on top.

## The Five Moves (timeless — obey these)

1. **One hero per screen.** Ruthless hierarchy: answer the user's #1 question loudly, demote everything else to support. Cheap screens answer six questions at the same volume.
2. **One accent; earn every second color.** Restraint is confidence. The accent means *interaction or status*, never decoration. Each extra color is a confession of indecision.
3. **Space over chrome.** When padding looks done, add ~50% more. Get depth from surface-elevation steps (luminance), not borders. Borders are the last resort. Density panic is the strongest cheapness tell.
4. **Type as structure.** Big scale jumps (hero ≈ 3–4× body), 1–2 typefaces, 2 weights. If you're bolding everything to fake hierarchy, your scale is too flat.
5. **Motion as explanation.** 150–350ms, ease-out or spring, never linear, never on everything. If nothing changed state, nothing moves. Premium motion is *felt*, not watched.

Plus a sixth, quieter one: **care at the edges** — design empty, loading, error, and success states with happy-path effort. That's where trust is won.

## Taste Rules (encodable)

| # | Rule |
|---|------|
| 1 | One hero element per screen; everything else demotes itself. |
| 2 | Pick ONE accent. Accent = interaction/status, never fill or decoration. |
| 3 | Never pure #000 or #FFF. Build 3 surface elevations from near-black/off-white; separate with them, not borders. |
| 4 | One global radius scale; nested elements use concentric radii (inner = outer − padding). |
| 5 | Type scale must jump. Two weights, large ratios. Bolding-for-hierarchy = scale too flat. |
| 6 | Motion explains causality/state or it doesn't exist. |
| 7 | Numbers are content: tabular figures, real locale formatting, meaningful precision. A giant "1,024.00" earns its size; a giant "3" is noise. |
| 8 | Personality only in low-stakes moments. Money, errors, deletion get calm, plain language. |
| 9 | Show the real product early and crisply. Screenshot > illustration > abstraction. |
| 10 | If a style ships in a template, it's already generic. Take the principle, replace the styling. |

## Durable vs Fad — separate principle from costume

| Principle (keep) | Costume (will date) |
|---|---|
| One accent on a neutral base | Hot-pink / lime / acid-yellow palette (reads "2025–26") |
| Typography as the layout | Serif-display revival (cyclical, ~2–3 yrs) |
| Giant hero number = hierarchy | Ring/donut charts (screenshot well, communicate poorly past 1 value) |
| Motion that explains state | "Motion everywhere" / aurora-mesh gradients (already the AI-default wallpaper) |
| Show the real product (light SaaS) | Dark dev-tool + monospace aesthetic (audience-gated; cosplay off a dev product) |

**Judgment > trend:** when you catch yourself reaching for a costume, ask "which move is this serving?" If none, drop it.

## Current register (July 2026 — reference, not gospel)

What's trending right now, useful as *examples* of the moves in action: Apple-style liquid-glass translucency and frosted depth layers; AI-copilot side panels and inline assistant chips docked beside content rather than replacing it; sci-fi/spaceship-dashboard neon grids on dark UI; atmospheric soft-glow, smoky-gradient hero art (replacing flat aurora-mesh); bold sculptural 3D objects — liquid-metal blobs, warped ribbons — as hero art; oversized fintech balance numbers; cream/pastel friendly onboarding; scattered/modular grid layouts breaking the rigid 12-column template; cinematic hero video backgrounds; spring-physics micro-interactions. Treat all of it as dated-by-default styling layered over the five moves.

## How It Goes Wrong (the tells)

- **Glowing-text tell:** saturated accent used for body text/large fills on dark — vibrating edges, failed contrast. Pros use neon at small area (a dot, a line, one number).
- **AI-template tell:** aurora gradient + Inter + three feature cards + "Ship faster." The gradient was doing the work the content couldn't.
- **Motion-tax tell:** staggered fade-ins on every list, scroll-jacking — the user waits for the UI to finish performing.
- **Mismatched-radius tell:** pill buttons + 8px inputs + 20px cards + sharp modals in one screen. Fastest amateur identifier.
- **Fake-hierarchy tell:** oversized numbers on data nobody asked about; six competing "hero" stats. Scale without editorial judgment is just shouting.
- **Inverted-dark-mode tell:** light design with colors flipped and pure-black background. Dark mode is a re-lighting job, not an inversion.

## Guardrails (non-negotiable — the trend feed ignores these)

1. **Contrast math.** Accent may carry text only if it passes WCAG 4.5:1; otherwise accent is non-text only. Lime/yellow on white almost always fail; hot-pink on near-black often fails. Not a style choice.
2. **Motion has a cost.** Honor `prefers-reduced-motion`; budget motion like bundle size; watch LCP on video heroes and jank on mid-range Android. Trend clips are recorded on top-end hardware.
3. **Content first.** IA, naming, and copy decide quality; the aesthetic is the visible 10%. Linear and top fintechs won on model clarity first.
4. **Ethics check.** Fintech aesthetic + celebration + haptics on money/consequential actions = casino mechanics. Confetti on a trade is a mistake. Delight belongs in low-stakes moments.
5. **Density by audience.** Whitespace = premium for consumer apps; *intentional density* = premium for pro tools. Don't max out padding by reflex.
6. **Correct for sample bias.** X surfaces what screenshots well (dark, neon, big type, motion) and under-samples what retains (clarity, fast loads, good defaults). The corpus is "what demos well," not "what's good."

## How this skill was built

Learned by studying ~40 currently-trending UI/design posts on X (July 2026), synthesized by Opus 4.8 with Fable 5 as a taste advisor. The costumes will age; the five moves and the guardrails are the durable part — refresh the "current register" section periodically, leave the rest.
