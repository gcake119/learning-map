# learning-map

## Purpose

Turn a topic into an interactive learning deck that teaches through observation, manipulation, comparison, simulation, and guided discovery rather than long-form exposition.

This skill is topic-agnostic. It can be used for technical subjects, science, humanities, language learning, professional training, conceptual models, processes, systems, and other subjects where interaction can make the material easier to understand.

Do not assume the subject is software, AI, Agent, or System Design unless the source material or user request says so.

## Core principles

1. One focused topic should usually become one independent interactive deck.
2. Start from a concrete question, phenomenon, task, tension, example, or situation instead of a glossary definition when the subject allows it.
3. Keep one focal learning problem visible at a time.
4. Prefer meaningful interaction, visual change, comparison, simulation, spatial relationships, and progressive disclosure over explanatory paragraphs.
5. Let the learner observe or experience something before naming the concept when practical.
6. Every interaction must serve a learning purpose. It should change what the learner can observe, compare, infer, construct, or test.
7. Do not add interaction only for decoration.
8. Do not use scores, locks, badges, completion gates, or game-like progression unless explicitly requested.
9. Keep prose concise. Let the visual or interactive representation carry as much explanation as the subject permits.
10. Do not reveal the entire conceptual structure up front when progressive discovery would teach it better.
11. Preserve the source material's terminology, framing, scope, and uncertainty. Do not invent missing facts or silently replace the source with generic knowledge.
12. The interaction format must follow the learning problem; do not force every topic into a system diagram, simulator, or the same component set.

## Curriculum planning with the Pyramid Principle

Interactive design begins only after the learning structure is sufficiently clear.

The skill should help the user discuss and shape the curriculum before building interactions. Use the Pyramid Principle as a reasoning aid: clarify the top-level learning outcome, group the supporting ideas or abilities beneath it, and make sure lower-level material actually supports the level above.

The Pyramid Principle is a structural check, not a requirement that every subject become a rigid tree. Preserve natural learning logic such as chronology, prerequisite order, developmental sequence, narrative progression, or procedural dependency when those are more appropriate.

### Determine curriculum status first

At the beginning, identify which situation applies.

#### Topic or rough idea only

Work with the user to develop the curriculum.

Start by clarifying:

- What should the learner ultimately understand, explain, decide, recognize, or be able to do?
- Who is the learner and what can they already be expected to know?
- What is inside and outside the intended scope?
- What central question or outcome should organize the material?

Then build downward from the top-level outcome.

#### Fragmented notes, sources, or content

Do not immediately turn the fragments into slides.

First:

1. identify the likely top-level learning outcome;
2. group related ideas;
3. distinguish core ideas from examples, evidence, exercises, and supplementary detail;
4. identify missing links, overlaps, and misplaced material;
5. discuss the proposed structure with the user.

#### Existing curriculum

An existing curriculum is NOT automatically locked.

By default:

1. understand the curriculum's current organizing logic;
2. review it with the Pyramid Principle;
3. identify strengths, gaps, overlaps, unclear groupings, sequencing issues, and weak learning objectives;
4. explain possible adjustments;
5. discuss them with the user before restructuring;
6. confirm the curriculum before moving into interaction design.

Do not replace the user's curriculum merely because another organization is possible.

#### Locked curriculum

Only treat the curriculum as fixed when the user explicitly says to follow it as-is, not change it, skip curriculum discussion, or equivalent.

In locked mode:

- preserve unit structure and order;
- preserve intended scope;
- do not silently reorganize content;
- still flag factual contradictions, impossible interactions, missing source material, or implementation blockers when they materially affect correctness;
- proceed directly to learning objectives and interaction design within the fixed structure.

### Build the curriculum pyramid

A useful discussion sequence is:

```text
Top-level learning outcome / central question
                ↓
Major supporting understandings or abilities
                ↓
Unit-level questions
                ↓
Concrete learning objectives
                ↓
Examples / evidence / practice
```

At each level, check:

- Does this item support the level above?
- Are items at the same level meaningfully distinct?
- Is an important supporting idea missing?
- Is the grouping based on a real learning relationship rather than convenient categorization?
- Does the order reflect prerequisite, chronology, process, difficulty, or another defensible learning sequence?
- Is an example being mistaken for a core concept?
- Is a topic label hiding the actual ability the learner needs?

### Define learning objectives

Do not stop at unit names such as "Authentication", "Photosynthesis", "Past Tense", or "Industrial Revolution".

For each unit, define what the learner should be able to understand or do afterward.

Prefer objectives such as:

- distinguish A from B;
- explain why X changes Y;
- trace a process;
- interpret evidence;
- apply a rule in a new example;
- compare alternatives under stated criteria;
- identify a boundary case;
- construct or revise a model;
- perform a procedure;
- justify a decision from evidence.

Objectives should be specific enough to guide interaction design, but they do not all need separate screens.

### Curriculum review questions

Before confirming a curriculum, review with the user:

- What is the one highest-level learning outcome?
- Do the major sections collectively support it?
- Are any sections primarily interesting side topics rather than necessary support?
- Are important prerequisites missing?
- Are two sections teaching the same underlying idea?
- Is the sequence appropriate for how understanding develops?
- Does every unit have a clear learning outcome?
- Are examples and exercises placed under the concept they support?
- Is the curriculum too broad for the intended depth or time?

Present findings as discussion points and proposed adjustments, not as an automatic rewrite.

### Curriculum confirmation gate

Do not proceed from curriculum planning to detailed interaction storyboard as though the structure were final until one of these is true:

- the user confirms the proposed curriculum;
- the user explicitly delegates curriculum decisions;
- the user explicitly locks an existing curriculum.

Once confirmed, treat that version as the working curriculum. Later changes are allowed when the user requests them or when new evidence reveals a material problem.

## Content design and learning copy

A confirmed curriculum defines **what to teach and in what structure**. It does not yet define the actual lesson content or the words that should appear on screen.

Do not jump directly from learning objectives to interaction storyboard or implementation.

Use a distinct content-design phase:

```text
Confirmed curriculum
        ↓
Learning objectives
        ↓
Canonical content
        ↓
Content review
        ↓
Interaction storyboard
        ↓
Presentation / learning copy
        ↓
Implementation
```

### Canonical content

Before designing the interaction for a unit, establish the stable instructional meaning that the deck must preserve.

Create a compact content brief for each unit or coherent learning segment. Include the relevant subset of:

- central question;
- learning objectives;
- core claims or conclusions;
- explanation, reasoning chain, mechanism, or argument;
- required terminology and definitions;
- prerequisites;
- examples;
- evidence or sources;
- misconceptions;
- counterexamples or boundary cases;
- uncertainty, disagreement, or limitations;
- what the learner should be able to transfer to a new case.

Not every field is required for every subject. Use only what helps define the instructional content accurately.

The canonical content is the source of truth for the lesson's meaning. It may be more complete than the final on-screen copy.

### Content grounding

Canonical content must be grounded in the user's supplied material, agreed curriculum, and appropriate sources.

When content is source-based:

- preserve the source's meaning and scope;
- distinguish source claims from added explanation;
- do not invent missing evidence;
- identify contradictions or uncertain material before turning it into confident teaching copy.

When outside research is needed, gather it before content approval rather than silently filling gaps during implementation.

When illustrative examples, synthetic data, or simplified models are used, label them appropriately and ensure they do not contradict the canonical content.

### Content review gate

Review the canonical content before detailed interaction design.

Check:

- Is it factually or conceptually correct?
- Does it actually satisfy the learning objective?
- Is the explanation complete enough for the intended learner?
- Is the depth appropriate?
- Are prerequisites missing?
- Are important distinctions collapsed?
- Are examples representative rather than misleading?
- Are misconceptions and boundary cases handled where they materially affect understanding?
- Does the content introduce claims not supported by the source or agreed scope?
- Is there unnecessary content that does not support the curriculum?

When the user is actively co-designing the course, discuss material content changes before treating them as final.

Do not use polished interaction to hide unresolved content.

### Canonical content vs. presentation copy

Keep these separate.

**Canonical content** answers:

> What does this lesson need to communicate accurately?

**Presentation / learning copy** answers:

> What should the learner see at this moment in the interactive experience?

Presentation copy includes:

- slide/stage titles;
- opening questions;
- short explanations;
- labels;
- button text;
- prompts;
- feedback;
- revealed terminology;
- summaries;
- transfer-exercise instructions.

Presentation copy may:

- shorten;
- split;
- reorder locally;
- delay a definition;
- turn a statement into a question;
- reveal an explanation after interaction.

It must NOT:

- change the meaning of canonical content;
- remove a qualification that materially changes correctness;
- introduce unsupported certainty;
- replace a precise concept with a catchy but misleading phrase.

### Write copy after the interaction purpose is known

Do not fully polish all screen copy before the storyboard exists.

First determine:

- what the learner sees;
- what they can do;
- what changes;
- what they should notice;
- what explanation is needed at that point.

Then write the presentation copy to support that interaction.

This avoids producing a text-heavy lesson and then adding decorative controls around it.

### Copy review

Before implementation or final content handoff, review presentation copy against canonical content.

Check:

- Is the wording accurate?
- Is it concise without losing necessary meaning?
- Does the question invite the intended observation or reasoning?
- Does feedback explain the consequence rather than merely say correct/incorrect?
- Is terminology introduced at an understandable moment?
- Is repeated explanation removable because the visualization already shows it?
- Does each label describe what the learner can actually observe or do?
- Does the final summary match what the interaction demonstrated?

### Content changes after implementation

UI approval does not freeze the learning copy.

If interaction behavior and visual structure are accepted but wording still needs work:

1. preserve the validated interaction unless the content correction requires structural change;
2. revise canonical content first when the underlying explanation changes;
3. update presentation copy from that revised content;
4. re-check that visuals and interaction still support the revised meaning.

## Default teaching rhythm

A useful default is:

```text
Question / situation
  ↓
Observe / explore / try
  ↓
A pattern, difference, consequence, or limitation becomes visible
  ↓
Inspect or compare
  ↓
Change a variable, choice, arrangement, or interpretation
  ↓
Observe again
  ↓
Explain / name the concept
  ↓
Apply it in a different example
  ↓
Summarize the reusable idea
```

This is a pattern, not a mandatory sequence. Omit or reorder steps when the subject requires a different learning path.

## Choose the learning mechanism from the subject

Before designing screens, identify what kind of understanding the learner needs.

### Relationship / structure
Use:
- interactive diagrams
- maps of relationships
- hierarchy exploration
- component reveal
- compare/contrast views

### Process / sequence
Use:
- stepwise animation
- timeline
- flow simulation
- state transitions
- before/after playback

### Cause and effect
Use:
- variable controls
- scenario switching
- simulation
- prediction → observation
- failure or counterexample injection

### Quantitative concept
Use:
- calculators
- sliders
- parameter controls
- charts
- proportional visualizations
- unit/scale comparison

### Classification / distinction
Use:
- sorting
- grouping
- side-by-side examples
- boundary cases
- progressive counterexamples

### Spatial concept
Use:
- manipulable diagrams
- layers
- zoom/reveal
- labeled regions
- transformations

### Interpretation / evidence
Use:
- source inspection
- annotation
- claim/evidence linking
- comparison of interpretations
- reveal of supporting details

### Decision / trade-off
Use:
- scenario choices
- consequence comparison
- constraint changes
- design comparison
- what-if exploration

### Skill / procedure
Use:
- guided practice
- staged task
- immediate state feedback
- worked example → transfer exercise
- reversible steps

Do not use an interaction pattern merely because it is available.

## Case and example selection

Examples should expose the concept clearly.

When useful:

1. use one example to demonstrate the idea;
2. use a different example or context for transfer.

The transfer example should test whether the learner understood the idea rather than memorized the first example.

Avoid adding many examples only to increase content volume.

## Interaction patterns

These are reusable options, not required components.

### Progressive Reveal
Reveal structure, evidence, labels, or explanation only when it becomes useful.

### Interactive Diagram
Use when relationships, parts, hierarchy, or spatial arrangement are central.

### Flow / Process Simulator
Use when understanding depends on sequence, state, or movement through stages.

### Variable / Parameter Explorer
Use when changing one or more inputs makes a relationship visible.

### Comparison
Use for:
- before / after
- option A / option B
- competing explanations
- alternative designs
- boundary cases

### Timeline
Use for chronological change, historical development, lifecycle, or staged progression.

### Evidence Explorer
Use when the learner must connect claims, observations, sources, or supporting details.

### Scenario / Consequence Explorer
Use when choices or conditions lead to different outcomes.

### Builder / Composer
Use when understanding improves by assembling a structure, argument, system, sequence, sentence, model, or plan.

### Profiler / Measurement View
Use when the subject involves locating where time, cost, quantity, effort, error, or another measurable resource is concentrated.

## Explanation and terminology

- Prefer plain language before specialized terminology.
- Introduce the formal term when the learner has enough context to understand what it names.
- Keep necessary technical or domain-specific terminology accurate.
- Do not simplify by changing the meaning.
- Distinguish observed facts, teaching assumptions, interpretations, and uncertain claims.
- Label synthetic or illustrative data clearly.

## Deck structure

A deck should be independently understandable.

A strong opening usually contains:
- one clear question or situation;
- only the context needed to begin;
- one obvious action or observation.

Avoid opening with:
- a full learning map;
- a glossary;
- a complete conceptual model;
- a long table of contents;
- all learning objectives at once.

A strong closing usually contains:
- the structure, explanation, method, model, or judgment the learner has built;
- a concise reusable principle;
- optionally a transfer exercise or next question.

Do not force a fixed number of screens. A screen exists because the learner needs a new observable state, action, comparison, or conceptual step.

## Learning artifact

When appropriate, let the learner finish with something concrete, such as:

- a completed diagram
- a model
- a comparison
- an annotated source
- a timeline
- a decision framework
- a worked solution
- a design
- a classification
- a causal explanation
- a summary generated from the learner's interactions

Not every subject needs a saved artifact.

## Visual direction

The validated reference implementation is:

`gcake119/agent-system-design-learning-map`
route: `#/deck/token-profiler`

It demonstrates an accepted interaction rhythm and presentation-first experience. It is a reference, not a template and not a content model.

General characteristics:

- presentation-first rather than dashboard-first;
- one dominant learning focus per stage;
- restrained chrome;
- concise labels;
- visual state changes that carry meaning;
- clear progress/navigation;
- responsive layout;
- reduced-motion support;
- avoid dense card grids and article-like scrolling unless the subject genuinely requires them.

Visual language should adapt to the subject. A history deck, language lesson, biology lesson, and software architecture lesson should not automatically look identical.

Do not clone third-party branding, proprietary assets, exact typography, or pixel-level visual design.

## Workflow for creating a new deck

### 1. Ground in the source

Read the supplied material or authoritative source first.

Identify:
- what the source actually teaches;
- its terminology;
- its organization and framing;
- what is factual, interpretive, illustrative, or uncertain;
- what is missing.

Do not silently fill source gaps unless the user asks for expansion or outside research.

### 2. Define the learning problem

Write:
- the topic;
- the central question;
- what the learner should understand or be able to do afterward;
- any prerequisite knowledge;
- the concrete learning artifact, if useful.

### 3. Identify the concept type

Decide whether the key understanding is primarily:
- structural;
- sequential;
- causal;
- quantitative;
- classificatory;
- spatial;
- interpretive;
- decision-oriented;
- procedural;
- or a combination.

Use this to choose interactions.

### 4. Select examples

Choose the smallest set of examples needed to teach and transfer the concept.

### 5. Build the interaction storyboard

For each stage define:
- visible question;
- initial visible state;
- learner action or observation;
- visual/state transition;
- evidence or consequence revealed;
- concept or explanation introduced afterward;
- reason this stage is necessary.

Remove stages that only repeat information.

### 6. Create teaching data and assets

When simulations or numbers are illustrative:
- use synthetic data unless real data is required;
- keep arithmetic internally consistent;
- label assumptions;
- make state changes deterministic enough to teach reliably.

When real sources, images, maps, quotations, or datasets are needed, preserve provenance and permissions.

### 7. Implement

Separate content/data/state logic from view code when practical.

Build reusable primitives where repetition is real, but do not force every deck into one universal component system.

### 8. Verify behavior

Check:
- every visible control works;
- back/restart behavior is predictable;
- direct route/load state works;
- responsive layout works;
- reduced-motion preserves essential information;
- numeric/data invariants are correct;
- no essential concept is available only through animation or hover.

### 9. Review learning quality

Human review should ask:
- does the experience feel like an interactive presentation rather than a dashboard or article?
- is there too much prose?
- can the learner see the important change?
- does each interaction teach something?
- is the conclusion supported by what was observed?
- could the learner transfer the idea to another example?
- did the implementation accidentally distort the source material?

Automated UI/test success is not final learning validation.

## Optional domain overlays

Domain-specific rules may be added on top of this skill when a subject needs them.

Examples:
- System Design may require architecture, failure, state, and verification reasoning.
- Language learning may require pronunciation, grammar, context, and production practice.
- History may require chronology, source interpretation, causality, and competing perspectives.
- Science may require variables, models, observation, uncertainty, and experiment design.

These belong in the deck specification or a domain overlay, not in the universal core of this skill.

## Anti-patterns

Avoid:

- one slide per learning objective;
- large scenario counts used as a proxy for depth;
- dashboards masquerading as lessons;
- interactions that do not change understanding;
- explaining everything before the learner can observe it;
- using the same visual metaphor for every topic;
- forcing every subject into a technical/system architecture frame;
- excessive typing before the learner has enough context;
- hiding essential information behind hover-only interaction;
- treating a successful animation or passing UI test as proof that learning works;
- adding domain assumptions that the source does not support.

## Reference implementation notes

The Token Profiler deck is the first validated reference for the interaction style.

It demonstrated:
- an independent deck;
- progressive interaction;
- visual state change;
- multiple views of the same underlying information;
- learner-driven comparison;
- redesign and re-run;
- a transfer example;
- presentation-first UI.

These are transferable interaction lessons. Token profiling, Agent workflows, architecture redesign, and System Design are NOT requirements for future decks.
