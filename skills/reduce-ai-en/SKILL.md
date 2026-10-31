---
name: reduce-ai-en
description: Natural English writing rules. Use when drafting any extended English prose — theses, papers, literature reviews, READMEs, release notes, technical docs, reports — so that AI-assisted text reads natural, restrained, and written by someone in the field. Avoids formulaic machine patterns (inflated significance, template conclusions, rule-of-three lists, filler connectives, AI vocabulary). Load this skill whenever the user asks to draft, continue, or expand any English paragraph, even if they never mention "AI tone".
---

# reduce-ai-en: Natural English Writing

These are generation-time constraints: load them before writing, and what you write is the final draft. There is no write-then-polish second pass. One goal — extended English prose that reads natural, restrained, and like it was written by someone who does this work.

This skill does not target AI detectors and promises nothing about detection scores. If asked, say so plainly: detectors are unreliable, and this skill fixes style, not detection.

## Before writing: calibrate

Confirm two things and read the matching references:

1. **Genre.** For a thesis or dissertation read `references/genres/thesis.md`. For a README, release notes, or usage docs read `references/genres/readme-docs.md`. Other genres run on the core rules below.
2. **Discipline.** If known, read the matching file under `references/disciplines/` (e.g. `engineering-management.md`). If none exists, rely on the core rules and common sense.

The core principles below always apply; no profile overrides them.

## Hard constraints

Three rules with no give. Style yields to fact.

**1. Facts are immutable.** Numbers, data, units, experimental settings, dates, names — use them exactly as the source material gives them, or leave a placeholder like `[TODO: N]` for the author to fill. Never invent a plausible number. One fabricated statistic does more damage than ten empty sentences: readers skip the empty ones and cite the fake one.

**2. Citations stay in place.** [1], (Smith, 2023), `FIDIC 1999` — keep markers where they are. When paraphrasing, keep the attribution the source provides; if there is none, write "some studies suggest" rather than inventing "Research has shown that...".

**3. One term per concept.** Pick "patients" or "participants" or "subjects" and stay with it. This cuts against schoolbook advice about varying vocabulary: in technical writing, cycling synonyms for the same construct makes readers count three different things. Term cycling is a machine tell; practitioners don't do it.

## Structural principles

The signal is in the structure, not the vocabulary. Swapping words fixes the layer that was already fixing itself; these rules fix the layer that persists.

**4. Concrete beats abstract.** Every paragraph lands on something concrete — a number, a named object, a step, a clause in a standard. Test: if the paragraph could be pasted into a paper in any other field unchanged, it is too abstract; rewrite it.

> Before: The proposed method significantly improves project management efficiency and shows great promise for practical applications.
> After: On the Metro Line 7 contract, the method cut schedule variance from 8.3% to 3.1%.

The numbers in the example are placeholders — in real writing they must come from the source material. Concrete content doesn't need "great promise" to back it up.

**5. Don't state the moral.** End on the evidence. No "This highlights the importance of...", no "This underscores the critical role of...", no "These findings pave the way for...". The reader draws the conclusion; writing it out is the heaviest machine habit there is.

> Before: The above results demonstrate that accurate risk identification is of great significance for successful project delivery.
> After: (Delete. The results already said it.)

**6. Vary paragraph architecture.** Not every paragraph is topic sentence → support → wrap-up. Don't run "Firstly, ... Secondly, ... Finally, ..." across a section. Don't end every paragraph on a summary sentence. Some paragraphs can open on a fact or a counterexample. Paragraph lengths differ — some three lines, some twelve.

**7. Let sentence length vary.** Mix long and short sentences within a paragraph; short sentences are often the author's firmest claims — keep them short. The standard is clarity, not rhythm for its own sake: split a sentence the reader must parse twice; keep long the sentence that merging would force the reader to reassemble.

**8. Connectives serve logic, not decorum.** Use "therefore", "in contrast", "building on this" when the logical relation needs making; state things plainly when it doesn't. Test: delete the connective — if the logic blurs, keep it; if only the tone flattens, cut it. "Therefore", "however", "moreover": at most one of each per paragraph. Note well: connectives are not an AI tell. Human academic prose uses them densely; stripping them until the text turns choppy is a worse defect than the one being fixed.

**9. Say it once.** State the point in its most specific form and move on. No "In other words", no "That is to say", no restating the last sentence at a higher level of abstraction. When you catch a repetition, delete the emptier version — usually the paraphrase.

## Language habits

**10. Plain verbs; no copula avoidance.** "Serves as", "stands as", "acts as", "functions as" → "is". "In order to" → "to". "Due to the fact that" → "because". "Conduct an analysis of" → "analyze". "Utilize" → "use". Prefer the plain verb; save the Latinate frame for when it carries weight.

**11. Cut the inflated register.** The overused tier — "pivotal", "landscape", "delve", "crucial", "robust", "novel", "comprehensive", "multifaceted" — and the dangling -ing verdict ("...highlighting the importance of...", "...underscoring the pivotal role of..."): report the finding, skip the commentary. The rule of three only when the list genuinely has three members; "not only ... but also ..." is usually just "and". Em dashes are not forbidden, but reach for a comma, parenthesis, or full stop first — stacked em-dash asides are a strong tell. Headings in sentence case, not Title Case.

**12. Hedge to match certainty.** One hedge per claim: "may suggest ... have the potential to confer" → "suggest ... may reduce". If the evidence is solid, say so plainly — a claim wrapped in perpetual caution reads as either machine-made or evasive.

## Vocabulary reference

`references/vocabulary.md` lists the common offenders by category. Treat it as a reference, not a checklist: avoid these patterns naturally while writing; do not run replacement passes. Any substitute phrase used repeatedly becomes the new tell. The cure for a cliché is usually deletion, not a synonym.

## On restraint

The goal is natural, not a different kind of artificial. When rules conflict or a call is close, return to one question: **would a practitioner reading this find it odd?** Practitioners don't count your connectives or scan for em dashes — they either find the prose unremarkable (good) or machine-flavored (bad). The rules serve that sentence; when they conflict with it, the sentence wins.
