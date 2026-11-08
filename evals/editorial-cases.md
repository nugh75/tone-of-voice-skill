# Editorial regression cases

Use these synthetic examples for a chat-only evaluation. Give the request and
the sample to the skill. Compare its response with the expected decision.

| Request and sample | Expected decision |
|---|---|
| Review two paragraphs. The first defines autoefficacia. The second uses the same term and reports how it was measured. | Keep the canonical term and both functions. |
| Review two paragraphs. Both say the same outcome was associated with autoefficacia in the same sample. The second adds neither evidence nor qualification. | Keep the canonical term and flag the repeated proposition for `/r-redundancy`. |
| Polish “Nel campione, X è associata a Y.” A proposed rewrite reads “X favorisce Y.” | Preserve the sample boundary and association. Flag the causal reading as a conceptual change. |
| Improve the rhythm of a long sentence and leave its meaning intact. The sentence contains a specialized term. | Offer a local replacement and describe its stylistic rationale. Preserve the term and its meaning. |
| A construction sounds awkward. The Treccani lookup is inconclusive. | Label the suggestion as a stylistic preference and report the lookup outcome. |
| Prepare an accepted style change for a versioned article. | Pass the locator, exact original and replacement, reason and evidence to the revision workflow. |
