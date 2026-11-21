# Corpus Codebook (Draft)

Definitions for sentence-level tags used in `corpus_template.csv`:

• Syntactic Agency:
  - `active_human`: Named person or role acts ("Our engineer checks the system").
  - `passive_agentless`: Passive voice with no actor named ("System checks will be performed").
  - `nominalized`: Smothered verb turned into an abstract noun ("facilitation of deliverables", "escalation").
  - `inanimate_actor`: Framework, policy, or system acts as subject ("The methodology ensures...").

• Modality & Modal Drift:
  - `firm`: Hard commitment (`will`, `shall`, `must`, `executes`—noting any drift from strict FAR Part 2 definitions).
  - `hedged`: Built-in wiggle room (`aims to`, `supports`, `designed to`, `strives to`, `may`).

• Specificity & Density:
  - `concrete`: Includes named tools, numbers, SLAs, or step-by-step workflow.
  - `echo`: Repeats prompt phrasing without new operational detail.
  - `noun_stack`: Heavy multi-word modifier chains with low concrete meaning ("enterprise-wide mission-critical support services").

• Pragmatic Uptake (`uptake_tag`):
  - `quotes_concrete_detail`: Reviewer cites specific numbers, tools, or workflows as a Strength.
  - `penalizes_vagueness`: Reviewer cites missing detail, hedging, or echo phrasing as a Weakness/Deficiency.
  - `echoes_vendor_fog`: Reviewer accepts or repeats abstract vendor phrasing without requiring concrete proof.
