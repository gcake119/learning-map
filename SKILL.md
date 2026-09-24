# learning-map

## Purpose

Turn a technical topic into an interactive learning deck that teaches through system behavior, manipulation, comparison, and design decisions rather than long-form exposition.

Use this skill for interactive technical learning materials, especially System Design and Agent-enabled System Design topics.

## Core principles

1. One topic should usually become one independent interactive deck.
2. Start from a concrete problem or design question, not a glossary term or definition.
3. Keep one focal problem visible at a time.
4. Prefer direct manipulation, simulation, state changes, diagrams, and comparison over explanatory paragraphs.
5. Let the learner observe a behavior before naming the concept when practical.
6. An interaction must change something meaningful: system state, architecture, data flow, evidence, measurement, or outcome.
7. Do not add interaction only for decoration.
8. Do not use scores, locks, badges, completion gates, or game-like progression unless explicitly requested.
9. Keep prose short. The visualization or simulation should carry most of the explanation.
10. Use progressive disclosure instead of showing the whole conceptual model up front.

## Default teaching rhythm

Use this sequence when it fits the topic:

```text
Problem
  ↓
Run / Observe
  ↓
Failure, limitation, or design tension becomes visible
  ↓
Inspect evidence
  ↓
Change the design
  ↓
Re-run the same case
  ↓
Compare results
  ↓
Verify the new design
  ↓
Transfer to a different case
  ↓
Name / summarize the design principle
```

Do not force every deck to use every step.

## System Design rule

For System Design materials, the main subject is the system.

AI, LLMs, and Agents are components or implementation choices inside that system.

Do not silently turn a System Design lesson into an Agent fundamentals lesson.

Ask questions such as:

- What must the system guarantee?
- What belongs inside or outside the system boundary?
- Which component owns this responsibility?
- How does data or work move through the system?
- Which work is synchronous or asynchronous?
- What state must persist?
- What can fail, and what happens next?
- What may the Agent see or do?
- Which guarantees must remain deterministic?
- What evidence is needed to know the system behaved correctly?
- What should be measured before redesigning the architecture?

## Agent-enabled System Design

When an Agent participates in implementation:

- distinguish Agent decisions from system guarantees;
- distinguish model context from persistent system state;
- keep permissions and important invariants outside prompt-only enforcement;
- treat Agent/tool/model failures as ordinary system failure modes that architecture must contain;
- evaluate architecture changes against quality and correctness, not only token/cost improvements;
- Multi-Agent is one architecture option, not an automatic end state.

## Case library

Prefer the case that makes the current design problem easiest to see.

### AI customer support system
Best for:
- tool and permission boundaries
- external services
- human escalation
- write operations
- partial failure and recovery

### Software development Agent
Best for:
- long-running work
- state and checkpoints
- context construction
- sandbox and permissions
- verification
- workflow profiling
- token attribution
- architecture redesign
- Multi-Agent comparisons

### Meeting work assistant
Best for:
- media/document pipelines
- queues and workers
- synchronous vs asynchronous execution
- partial completion
- background processing
- scale

### Research assistant
Best for:
- retrieval
- context
- source evidence
- claim tracing
- semantic evaluation
- observability

### Enterprise knowledge assistant
Best for:
- ingestion
- indexing
- ACL propagation
- freshness
- versioning
- source-of-truth design

### Data analysis Agent
Best for:
- data architecture
- query sandbox
- semantic/metric contracts
- resource limits
- cost attribution
- performance bottlenecks
- scaling

## Case-transfer rule

Whenever possible:

1. teach the design issue with the case that exposes it most clearly;
2. use a different case for the learner exercise.

The transfer case should test whether the learner understood the design principle rather than memorized the first domain.

## Interaction patterns

Choose the smallest interaction pattern that makes the system behavior visible.

### Architecture Builder
Use for:
- component responsibility
- boundaries
- trust boundaries
- data/storage placement
- architecture redesign

### Flow Simulator
Use for:
- requests
- jobs
- queues
- asynchronous work
- pipelines
- data movement

### Failure Injection
Use for:
- timeout
- crash
- partial success
- lost response
- stale data
- authorization failure
- external dependency failure

### Trace Explorer
Use for:
- request/job/run tracing
- tool calls
- source provenance
- debugging
- observability

### Profiler
Use for:
- latency
- token use
- cost
- throughput
- queue depth
- model/tool calls
- bottleneck analysis

### Design Comparison
Use when the learner needs to compare:
- before / after
- single Agent / parallel tools / Multi-Agent
- sync / async
- prompt-only / backend enforcement
- full history / retrieval + structured state

## Optimization rule

Do not teach optimization as isolated tricks.

Prefer:

```text
MEASURE
  ↓
ATTRIBUTE
  ↓
DIAGNOSE
  ↓
REDESIGN
  ↓
RE-RUN
  ↓
VERIFY
```

Examples of redesign targets:

- prompt
- context construction
- retrieval
- persistent state
- tool-output processing
- deterministic validators
- model routing
- workflow structure
- service boundaries
- queue / worker architecture
- Multi-Agent coordination

When token use is involved, distinguish:

- call-level usage: how many input/output tokens a model call consumed;
- workflow attribution: which step and context source caused that usage.

Do not assume provider APIs expose identical usage fields.

## Verification rule

A cheaper, faster, or simpler design is not automatically better.

Re-run the same workload or fixed evaluation set whenever possible.

Compare at least the relevant subset of:

- required behavior
- correctness
- permissions
- evidence
- quality
- latency
- token use
- cost
- failure behavior

If quality or correctness drops, show that regression explicitly.

## Deck structure

A deck should be independently understandable.

Recommended opening:
- a concrete engineering problem;
- enough system context to act on it;
- one clear action.

Recommended closing:
- the design artifact or judgment the learner has produced;
- a concise reusable principle;
- optionally a transfer exercise.

Avoid opening with:
- a learning map;
- a full architecture diagram;
- a glossary;
- a list of all topics.

## Design artifact

Each deck should leave the learner with a concrete System Design output or decision, for example:

- requirements and constraints
- component responsibility diagram
- execution/data flow
- Agent/tool/trust boundary
- state/context strategy
- failure and recovery strategy
- data-access/governance design
- observability design
- verification strategy
- profiler report and architecture redesign

## Visual direction

The first validated reference implementation is:

`gcake119/agent-system-design-learning-map`
route: `#/deck/token-profiler`

Use it as a reference for interaction rhythm and presentation behavior, not as a mandatory template.

Desired characteristics:

- presentation-first rather than dashboard-first;
- one dominant visual per stage;
- restrained chrome;
- short labels and technical annotations;
- diagrams that animate meaningful state changes;
- clear progress/navigation;
- responsive;
- reduced-motion support;
- no dense wall of cards or article-like scrolling unless the content truly requires it.

Do not clone third-party branding or pixel-level visual design.

## Workflow for creating a new deck

### 1. Define the learning problem
Write:
- the engineering question;
- what decision the learner should be able to make afterward;
- the System Design artifact produced.

### 2. Select cases
Choose:
- one explanation case;
- one transfer case when useful.

Do not add more domains without a teaching reason.

### 3. Build the interaction storyboard
For each stage define:
- visible question;
- system state;
- user action;
- visual/state transition;
- evidence revealed;
- concept named afterward;
- next design tension.

### 4. Create deterministic teaching data
For simulations:
- use synthetic data unless real data is explicitly required;
- keep arithmetic internally consistent;
- make failure modes reproducible;
- label synthetic benchmarks/costs clearly.

### 5. Implement
Keep content/model/state logic separate from view code when practical.

Prefer reusable primitives, but do not force every deck into one universal component.

### 6. Verify
Check:
- every visible control works;
- back/restart behavior is deterministic;
- direct route load works;
- mobile layout works;
- reduced-motion preserves information;
- arithmetic/data invariants pass tests;
- interaction changes meaningfully affect state or architecture.

### 7. Human UI review
After automated checks, inspect:
- does it feel like an interactive presentation?
- is there too much prose?
- can the learner understand the main change visually?
- is the interaction teaching or merely decorating?
- is the engineering conclusion supported by what the learner observed?

Do not treat automated UI/test success as final learning validation.

## Anti-patterns

Avoid:

- one slide per learning objective;
- huge scenario counts used as a proxy for depth;
- card-heavy dashboards masquerading as lessons;
- abstract forms that ask learners to type design answers before they have manipulated a system;
- explaining everything before the interaction;
- treating all AI components as Agents;
- presenting Multi-Agent as inherently more advanced or better;
- reducing System Design to prompt engineering;
- optimizing token usage without measuring other bottlenecks;
- accepting a lower-cost design without re-verifying quality;
- using a single domain so heavily that the learner can succeed by memorizing the example.

## Reference implementation notes

The Token Profiler deck established the first accepted pattern:

- independent deck;
- run an Agent workflow;
- inspect per-call token usage;
- re-aggregate by context source;
- distinguish provider usage from application-level attribution;
- redesign state/retrieval architecture;
- run the same workload again;
- reject a cheaper design when verification regresses;
- transfer to a Data Analysis Agent where the dominant cost is outside the LLM.

Use this as evidence for the rules above, not as a requirement that every future deck contain profiling.
