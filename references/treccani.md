# Linguistic verification — Treccani

A revision that makes a claim about Italian must be defensible. This reference
governs when to check one and how to report it; the `treccani` skill performs the
lookup.

Verification is conditional. It applies to a genuine doubt or to an explicit
linguistic judgement, not to every period of the text.

## When to consult

Check before asserting anything about:

- conjunctions and connectives, and the relation a given connective expresses;
- verb, noun, and adjective government, and the choice of preposition;
- coordination and subordination, and the order of constituents;
- punctuation, when the doubt concerns correctness rather than rhythm;
- pronouns, anaphora, and demonstratives;
- fixed locutions, foreign borrowings, and technical terms;
- nominalizations and forms perceived as bureaucratic, literary, archaic, or
  colloquial;
- differences in meaning between constructions that look equivalent.

Also check whenever the revision note would use the words *scorretto*,
*burocratico*, *antiquato*, *improprio*, or *non si dice*.

## When not to consult

Skip the lookup for ordinary rewriting where no linguistic claim is made: cutting
a redundant sentence, reordering information, replacing a vague noun with a
precise one, or shortening a period. Consulting a dictionary for every sentence
wastes the pass and buries the cases that matter.

## How to consult

Use the `treccani` skill. Choose the command from the doubt, not from the
sentence:

| Doubt | Command |
|---|---|
| meaning, accezioni, government of a verb or noun | `word <lemma>` |
| register: bureaucratic, archaic, literary, rare? | `word <lemma>`, then read the usage labels (*burocr.*, *ant.*, *letter.*, *raro*) |
| an equivalent in another register | `synonyms <lemma>` |
| a construction, a connective, punctuation, agreement | `language <phenomenon>` |
| the concept behind a technical term | `encyclopedia <term>` |

Where authority sits: the Vocabolario decides **register**, through its usage
labels; the Enciclopedia dell'Italiano decides **structure**, because it
describes the grammar of the language. A magazine article describes usage; it
does not settle a norm.

Search the lemma, never the inflected form, and never the author's sentence:
what reaches Treccani is the isolated doubt, not the passage under revision.

Read `warnings` before the results — it says whether you have the entry or only a
fallback search — and read `truncated`: an extract is not the whole entry.

## The four levels

Separate them explicitly; conflating them is the failure this reference exists
to prevent.

| Level | Question |
|---|---|
| **Correctness** | Is the construction grammatically admitted? |
| **Meaning** | What semantic relation does it express? |
| **Register** | Is it common, academic, specialistic, bureaucratic, literary, colloquial, rare, archaic? |
| **Appropriateness** | Does it suit this text, or would a plainer form be clearer here? |

Most disputed cases in academic Italian are level 3 or 4, not level 1.
`nonché`, `altresì`, `il medesimo`, `per quanto concerne`, and `nell'ambito di`
are admitted forms with a marked register, not errors.

## Reporting

State the level, name and link the exact entry consulted, then give the proposal.
Record whether the entry supported the judgement, was inconclusive, or was
unavailable. Carry that evidence with the proposal when handing it off.

- «`in merito a` è corretto ma di registro burocratico (Vocabolario Treccani,
  s.v. *merito*): qui `su` è più piano.»
- «`nonostante` regge il congiuntivo o un nome, non `che` + indicativo
  (Enciclopedia dell'Italiano, *concessive, frasi*).»

When the entry does not settle the question, say so and present the change as a
motivated stylistic preference:

- «Treccani non discrimina i due costrutti; preferisco il secondo perché
  avvicina il soggetto al verbo.»

If the `treccani` skill is unavailable or returns an error, the point is
unverified: say it, and do not upgrade the change into a linguistic correction.

## Prohibitions

- Never call a form wrong when it is only unsuited to the register of the text.
- Never turn a stylistic preference into a grammatical rule.
- Never attribute to Treccani a judgement its entry does not carry.
- Never state that a point was checked when the lookup was not run or failed.
- Never leave an explicit linguistic claim unverified when a real doubt exists.
