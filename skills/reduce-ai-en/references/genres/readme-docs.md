# Genre: README / Release notes / Usage docs

Machine flavor in docs is different from in papers: papers inflate significance, docs do marketing decoration. Both come from templates, but the symptoms differ — treat what's in front of you.

## Layout

- No emoji in headings. None. "🚀 Quick Start" and "✨ Features" are the generated-doc signature.
- Badges: hosting platform, license, maybe CI if it's real. A wall of badges is decoration wearing a suit.
- Don't bold terms reflexively; when everything is emphasized, nothing is.
- Sections follow the document's actual need, not the full template stack (Intro / Features / Install / Usage / Roadmap / Contributing / License). Installation appears exactly once.

## Voice

State facts; skip marketing.

> Before: A powerful and elegant tool that lets you achieve stunning efficiency gains with ease!
> After: This script cuts X's build from ~4 min to 40 s (measured; if unmeasured, write "faster" — no invented numbers).

- "Powerful", "blazing fast", "elegant", "effortless", "seamless", "just three steps": deleting these costs no information. Delete them.
- Performance, coverage, and scale numbers need a source. If you haven't run the benchmark, there is no benchmark number.
- No "Why choose X?" self-Q&A headings. The facts answer it or they don't.

## Content discipline

- Install steps, config options, commands: write them once, write them correctly. Command blocks are copy-pasteable as-is — no dropped required flags, no triple repetition for thoroughness.
- Known issues are known issues; "under active development" is not an issues section.
- Roadmap: one or two concrete items, or none. A fifteen-item checklist that stops updating after v1.0 is just a lie with checkboxes.
- Version numbers, bundle sizes, compatibility ranges: verify before writing; keep them consistent across the document.

## Register for technical docs

Direct and executable, few adjectives. One command per line, one intent per paragraph. The reader came to do something; every word between them and the command needs a reason to exist.
