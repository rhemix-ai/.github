# rhemix

**Stateful synthetic dialogue for conversational AI evaluation and research.**

Rhemix is a Python ecosystem for building synthetic dialogue datasets from domain-specific ingredients. A `domain pack` defines the world: participant roles, prompts, tools, constraints, and quality checks. Profile generation creates concrete participants for that world. The engine then runs multi-party conversations through explicit discourse-state operations, producing transcripts, state snapshots, tool traces, and generation metadata.

## What Rhemix Is For

Rhemix is built for evaluation engineers, data scientists, and researchers who need controlled dialogue data rather than scraped, hand-authored, or single-pass conversations.

It is designed for work such as conversational AI evaluation, redaction and compliance testing, dialogue-system regression tests, and research workflows that need structured conversational state alongside plain text.

## How The Ecosystem Fits Together

The framework separates conversation generation from domain content.

| Package | Role |
| --- | --- |
| `rhemix-engine` | Domain-agnostic runtime for discourse state, orchestration, dashboard workflows, and batch generation. |
| `rhemix-profiles` | Infrastructure for generating and managing participant profiles. |
| Domain packs | Vertical-specific roles, schemas, prompts, tools, constraints, routing policies, and quality checks. |

Domain packs can vary the participants, world state, scenario parameters, channel, language configuration, output style, tool surface, and evaluation rules without changing the core runtime.

## What Gets Produced

Rhemix conversations are generated as inspectable artifacts, not just text transcripts.

- Conversation transcripts
- Discourse-state snapshots
- Tool traces
- Participant/profile metadata
- Generation metadata
- Domain-specific quality signals

## The Name

The name is a portmanteau of **rheme** and **remix**. A *rheme* is the new-information contribution an utterance makes to a discourse. *Remix* points to the system's method: participant profiles, scenarios, domain constraints, and discourse operations are recombined to generate new conversations with inspectable structure.

## Status

Public repositories and documentation are being prepared. The public website is available at [rhemix.ai](https://rhemix.ai/).

For early access or questions, reach out at [jake@rhemix.ai](mailto:jake@rhemix.ai).
