---
name: tone-of-voice
description: |
  Apply a precise yet creative academic writing style. Balanced between
  formal rigour and occasional metaphor/humour. Active when generating,
  revising, or translating any text intended for publication.
---

# Tone of Voice Skill `ToV`

Apply these rules when writing, revising, or translating content.

## Core Principles

| # | Rule | Detail |
|---|------|--------|
| 1 | **Formal register with bounded creative licence** | Academic tone first. Allow occasional metaphors and measured humour/irony only when they do not reduce precision, neutrality, or scholarly credibility. In empirical sections, prefer plain style. |
| 2 | **Well-articulated sentences** | Prefer sentences that fully develop the thought, with subordinate clauses where they add precision and logical nuance. Avoid both excessive fragmentation (paratactic strings) and gratuitous convolution. |
| 3 | **Impersonal voice** | Use *"si ritiene"*, *"è possibile osservare"*, etc. Avoid first-person singular (*"io"*, *"ritengo"*). |
| 4 | **Accessible language** | Define every acronym at first use: *LLM (Large Language Model)*. Avoid unexplained jargon. |
| 5 | **No repetition** | Vary vocabulary; use synonyms rather than repeating the same term. |
| 6 | **Precision in data** | Report exact values: *"68,3%"*, not *"circa il 70%"*. |
| 7 | **Hook endings** | Use paragraph endings that support transition only when they improve cohesion. Avoid formulaic hooks that add emphasis without adding content. |
| 8 | **Metacognitive signposts** | Use phrases like *"In questo articolo analizzeremo..."* or *"Come vedremo..."* sparingly, only when they genuinely improve orientation. |
| 9 | **Digressions** | Brief asides in parentheses `()`; longer ones as footnotes. |
| 10 | **Lists** | Use bulleted/numbered lists only when strictly necessary. Prefer prose. |
| 11 | **Thematic unity** | Each theme must be opened, developed, and concluded within a single section. Every new term/concept must be briefly glossed on first mention; the full treatment belongs in the section dedicated to that concept. |
| 12 | **Linear argumentation** | The argument flow must be strictly linear — never introduce a concept whose comprehension depends on material that appears later in the text. |
| 13 | **Anafore univoche e zero** | Ogni pronome anaforico (questo, questa, ciò, esso, ella, loro, il, la, le, i, un, tale, simile, stesso, medesimo) deve avere un solo antecedente plausibile nel contesto immediato. Verificare sempre: a quale sostantivo rimanda il pronome? Se la risposta non è immediata, riscrivere. Analogamente, le anafore zero (soggetto o complemento omesso perché recuperabile dal contesto) devono essere interpretabili con certezza: se il lettore deve dedurre l'agente dall'azione verbale o dalla coesione testuale, il rischio di ambiguità è alto. In caso di dubbio, esplicitare il nome. |
| 14 | **No rhetorical overstatement** | Avoid emphatic, promotional, or dramatizing language. Prefer restrained formulation over evaluative intensifiers. |
| 15 | **Claims proportional to evidence** | Match each claim to the study design. For cross-sectional, non-probabilistic, or self-report studies, avoid causal wording and frame implications as interpretive, exploratory, or hypothesis-generating. |
| 16 | **Methods before interpretation** | In empirical writing, prioritise operational clarity: recruitment, instruments, item logic, scale construction, reliability/validity, and construct definitions should be stated explicitly before broader interpretation. |
| 17 | **Originality must be explicit** | When introducing a framework, state clearly what is novel relative to adjacent models and distinguish original contribution from integration or synthesis. |
| 18 | **Terminological stability** | Use one label per construct throughout the manuscript unless a justified distinction is introduced explicitly. |
| 19 | **Editorial economy** | When close to a character cap, replace rhetorical transitions, repeated framing, and redundant qualifiers with concise methodological specification. |
| 20 | **Connettivi a inizio frase** | Il connettivo apre la frase ed è seguito da virgola: *"Tuttavia, ..."*, *"Infatti, ..."*, *"Pertanto, ..."*, *"Inoltre, ..."*. Mai inserito all'interno della frase: *"Il dato, tuttavia, ..."* → *"Tuttavia, il dato ..."*. |

## Diplomacy & Criticism

- Use the conditional mood for limitations, interpretations, and non-demonstrated implications (*"sarebbe possibile"*, *"si potrebbe notare"*). Use the indicative for verified procedural or descriptive statements.
- Frame critiques as observations of limitations, not direct refutations.

## Bibliography & Citations

| Rule | Detail |
|------|--------|
| Authors | Last name only: *"Come sostiene Rossi..."* |
| Citation style | Delegate to `article-revision` skill (journal norms). |
| Quotation format | Delegate to `article-revision` skill. |
| Cross-check | Every reference-list entry must be cited at least once in the text, and every in-text citation must appear in the reference list. |

## Language

- **Primary language**: Italian (`ARTICLE_LANG=it`). The same tone applies to English text when translating.
- **Foreign terms**: Anglicisms and loanwords allowed when they are the standard technical term or when context requires it. When in Italian text, follow the accepted-anglicisms list from `article-revision`.
- **Article length**: Delegate to `.env` (`EDITORIAL_LIMIT_CHARS`) and editorial norms.

## Titles

- Descriptive and short.
- Avoid creative/punning titles.

## Interaction with Other Skills

| Skill | Handoff |
|-------|---------|
| `article-revision` | Citation format, quotation style, bibliography management, anglicism validation, length limits |
