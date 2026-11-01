# English machine-flavor wordlist (reference, not a checklist)

Use this to avoid patterns naturally while writing — not as a replacement table. Any substitute phrase used repeatedly becomes the new tell. The cure for a cliché is usually deletion, not a synonym.

Data file; updated as patterns are identified. Add words with context notes (see CONTRIBUTING.md).

Note on decay: the vocabulary tier expires. "Delve" collapsed after it was named in 2024; newer models suppress em dashes on their own. The structural patterns (significance inflation, template conclusions, moral-stating) last; the word list does not. Prioritize accordingly.

## Formulaic openers

| Phrase | Handling |
|---|---|
| It is worth noting that / It is important to note | Delete; say the thing |
| In recent years, X has attracted increasing/growing attention | Open on a concrete phenomenon or number instead |
| In the ever-evolving landscape of / In today's fast-paced world | Delete; docs, not prose, start this way |
| With the rapid development of | Same as above |

## Significance inflation

| Phrase | Handling |
|---|---|
| plays a crucial/pivotal role in | Say what it actually does |
| stands as a testament to / serves as | "is", usually |
| represents a significant step towards | Delete; the step is the step |
| sheds light on / paves the way for / opens new avenues | Delete or state the concrete consequence |
| underscores the importance of / highlights the critical role of | Delete the commentary sentence entirely |
| groundbreaking / state-of-the-art / novel | Only when verifiably true; usually cut |

## Dangling -ing verdicts

| Pattern | Handling |
|---|---|
| "..., highlighting the importance of X" | Report the finding; drop the verdict |
| "..., demonstrating the profound impact of X" | Same |
| "..., showcasing the potential of X" | Same |

The construction attaches an appraisal to real data — keep the data, lose the appraisal.

## The overused tier (era-dependent)

delve, pivotal, landscape, testament, crucial, foster, leverage, robust, comprehensive, multifaceted, intricate, paramount, instrumental, holistic, seamless, transformative, harness, embark, navigate (metaphorical), unlock, elevate. — Check each: does the plain word lose anything? "Important" for "crucial", "use" for "leverage", "part" for "landscape".

## Connective padding

| Pattern | Handling |
|---|---|
| Moreover / Furthermore chains | Vary by relation; don't stack additively |
| Additionally | At most once per paragraph |
| In conclusion / To summarize | The conclusion section concludes; drop the signpost |
| Firstly, Secondly, Finally | Only for genuine enumeration; usually cut |

## Wordy frames

| Phrase | Handling |
|---|---|
| in order to | to |
| due to the fact that | because |
| a majority of | most |
| conduct an analysis of | analyze |
| it can be seen that / it is observed that | Delete; state the observation |
| not only ... but also ... | Usually "and" |

## Negative parallelism (the "not X, but Y" template)

| Form | Handling |
|---|---|
| "not X, but Y" / "The key is not X but Y" / "What matters is not X, but Y" | Handle by meaning, three ways: the negated term adds nothing → drop it, state Y alone; it names a misconception worth marking → state Y first ("Y, not X" — plain appositive contrast); X is the default assumption the passage overturns → keep refute-then-state. Cap the literal form at two or three per document |
| "not just X — it's Y" / "isn't X; it's Y" | Same treatment; these variants count toward the same quota |

Test per instance: does the sentence draw a real distinction below the surface? A real one keeps its function in a new form; a fake one ("not just a tool, but a paradigm") is the template impersonating a thought — delete.

## Signposted advances (announcing the move instead of making it)

| Form | Handling |
|---|---|
| "With these two points established, the picture becomes clear" / "Bringing these together, ..." / "It is against this backdrop that ..." | Delete the announcement; the next sentence makes the move directly |
| "Needless to say" / "It goes without saying" | If it needn't be said, don't |

Root cause: over-explicitation — spelling out relations the context already implies. Connectives that carry logic are fine; announcing that you are about to connect things is not.

## Abstract subjects (verbs demoted to nouns)

| Form | Handling |
|---|---|
| "The implementation of the policy drove the improvement of efficiency" | Restore the actor: "After the policy took effect, efficiency improved" |
| "The solution of the problem depends on the allocation of resources" | "Solving this depends on allocating resources" — or better, name who allocates what |

Readers parse agency backwards in these sentences; give the action back to the verb and the actor back to the subject.

## What to keep (do not over-correct)

- Logical connectives: Although, Whereas, Thus, Hence, Therefore, In contrast, Conversely, Based on these results, As expected — dense, natural use of these is what good human academic prose looks like. Stripping them produces choppy text, which is a worse defect than the one being treated.
- "Additionally" once per paragraph; "not only ... but also" once per paragraph when the semantics genuinely escalate.
- Hedges that match real uncertainty (may, suggests, consistent with); superlatives that are true; plain "is" and "has"; plain verbs — wrote, used, measured. AI avoids these; people use them freely. Protect them.
