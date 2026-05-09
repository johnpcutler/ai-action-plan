← [README](README.md) | [Combined Report](combined-com-b-report.md) | [Action Plan](ai-maturity-action-plan.md)

---

# COM-B Behavioral Diagnosis: AI as a Thought Partner (Level 1)

**Maturity Level:** 1 — AI as a Thought Partner
**Subtitle:** Help people explore ideas and improve decisions
**Date:** 2026-05-09
**Framework:** COM-B → BCW → BCT Taxonomy v1

---

## Step 1: Behavior Canvas

Two behaviors are framed for this level: an **adoption behavior** (getting individuals to use AI as a thought partner) and a **progression blocker** (why organizations stall at Level 1 and can't advance to Level 2).

---

### Behavior A — Adoption Behavior

| Field | Definition |
|-------|-----------|
| **Behavior** | Employees regularly use AI tools as thought partners for research, brainstorming, and first drafts |
| **Who** | Knowledge workers across the organization — individual contributors, managers, strategists, creatives, analysts. Multiple roles with varying technical comfort levels. |
| **Will do what** | Open an AI tool (ChatGPT, Claude, Gemini, or similar), formulate a prompt that describes their thinking challenge, iterate on the AI's response to sharpen ideas, and incorporate the output into their work product (email, document, presentation, analysis, decision). |
| **To what extent** | Multiple times per week as a default part of the thinking process — not just for novelty or emergencies. Prompts should go beyond simple factual queries to include brainstorming, drafting, critique, and synthesis. Quality bar: the person can distinguish useful AI output from hallucinated or shallow output and knows when to stop iterating. |
| **In what context** | During normal work hours, using personally or organizationally provisioned AI tools, on work devices. No formal process or integration required — this is ad-hoc, individual-level usage. Constraints include data sensitivity concerns, inconsistent tool access, and competing time pressures. |
| **For what outcome** | Faster answers and better first drafts. Reduced time spent on research and brainstorming. Improved quality of strategic and creative thinking. Lower activation energy for writing-heavy tasks. |
| **Current state** | **Partially Realized / Inconsistent** — Usage exists in pockets. Early adopters use AI daily; many employees have tried it once or twice and dropped off; some haven't tried at all. No shared understanding of what "good use" looks like. |
| **Prior attempts** | Organizations have tried: (1) sending company-wide emails encouraging AI use — low follow-through; (2) purchasing enterprise AI licenses — low adoption beyond early adopters; (3) one-off "lunch and learn" sessions — attendance was optional and skewed toward the already-converted; (4) sharing prompt libraries — downloaded but rarely used because context doesn't transfer. These attempts over-index on awareness (ED) and tool provision (EN) while ignoring capability, social permission, and habit formation. |

---

### Behavior B — Progression Blocker

| Field | Definition |
|-------|-----------|
| **Behavior** | Organizations get stuck at ad-hoc individual AI usage and can't formalize or scale to Level 2 (AI-enhanced workflows embedded in processes) |
| **Who** | Organizational leaders, team leads, and the informal network of early adopters. Also includes IT/security teams who control tool access and policy. |
| **Will do what** | Transition from individual, ad-hoc AI usage to documented, team-level AI-enhanced workflows — identifying high-value use cases, creating shared prompting practices, establishing guidelines for responsible use, and embedding AI steps into existing processes. |
| **To what extent** | At least 2-3 team-level workflows should incorporate AI as a standard step, with shared templates, quality criteria, and documented practices. Usage should be tracked (even informally) and discussed in team retrospectives. |
| **In what context** | Cross-functional organizational setting. Requires coordination between practitioners (who know what works), managers (who allocate time and signal priority), and governance functions (legal, IT, compliance) who set boundaries. |
| **For what outcome** | Move from scattered individual value to repeatable organizational value. Create the foundation for AI to become a tool of the team, not just the individual. Enable measurement, learning, and scaling. |
| **Current state** | **Aspirational Only** — Many leaders say they want to "be an AI-first organization" but have not defined what that means in practice. No shared specification of what Level 2 looks like. Early adopters are frustrated; late adopters are disengaged. Governance is either absent or overly restrictive. |
| **Prior attempts** | (1) Top-down mandates to "use AI more" without defining what that means — creates compliance theater. (2) Appointing an "AI champion" without authority or time allocation — champion burns out. (3) Waiting for a vendor to provide an enterprise-ready solution — delays action indefinitely. (4) Treating AI adoption as an IT project rather than a behavior-change effort — misses the human dynamics entirely. |

---

## Step 2: Dimensional Lens Analysis

### Capability (PC)

#### PC-1.1-Knowledge: Declarative and Procedural Knowledge

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PC.1.1.1 Declarative knowledge | **High** | Low-to-mid | Most employees know AI chatbots exist and have a surface understanding of what they do, but lack knowledge of prompt engineering principles, model limitations, and when different tools are appropriate. |
| PC.1.1.2 Procedural fluency | **High** | Low | Few people have a repeatable procedure for AI interaction. They open ChatGPT, type something vague, get a mediocre response, and conclude "AI isn't that useful." The multi-turn prompting skill — where you refine, redirect, and build on responses — is largely absent. |
| PC.1.1.3 Sequence clarity | **Medium** | Low | There is no widely understood sequence for "how to use AI as a thought partner." People don't know whether to start broad or narrow, when to push back on AI output, or how to structure a multi-prompt session. |
| PC.1.1.4 Skill stage | **High** | Novice for most, practiced for early adopters | The vast majority of employees are at the novice stage. They can perform the basic action (type a prompt, read a response) but lack the fluency to get consistent value. |
| PC.1.1.6 Exception handling | **Medium** | Low | When AI produces a hallucination, a confidently wrong answer, or an unhelpful response, most people don't know how to recover. They either accept the bad output or abandon the tool entirely. |

#### PC-1.2-Models: Mental Models

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PC.1.2.1 Model accuracy | **High** | Low | Dominant mental models are polarized: either "AI is magic and can do anything" (leading to disappointment) or "AI is just a search engine" (leading to underuse). Neither model supports effective thought-partnership. People don't understand that AI is a probabilistic text generator that excels at certain patterns and fails at others. |
| PC.1.2.2 Causal understanding | **High** | Low | People don't understand *why* prompts produce different quality outputs. They don't grasp that specificity, context, and role-framing change results because the underlying model responds to statistical patterns in training data. |
| PC.1.2.5 Model completeness | **Medium** | Low | Important factors are omitted from people's mental models: data privacy implications, the non-deterministic nature of outputs, the difference between reasoning and pattern-matching, and the fact that AI doesn't "know" things the way humans do. |
| PC.1.2.7 Updateability | **Medium** | Mid | Most people are willing to update their model of AI — this is a new domain and mental models are not yet rigid. This is a window of opportunity: models are forming now and can be shaped. |

#### PC-1.3-Judgment: Judgment and Decision Competence

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PC.1.3.2 Uncertainty tolerance | **High** | Low | People are uncomfortable with AI's probabilistic nature. They want definitive answers and are unsettled when AI hedges, contradicts itself, or produces different answers to the same question. |
| PC.1.3.4 Recognition competence | **High** | Low | Most people cannot quickly distinguish high-quality AI output from plausible-sounding but inaccurate output. They lack the pattern recognition that experienced AI users develop — knowing when output "feels off" even before fact-checking. |
| PC.1.3.7 Tradeoff handling | **Medium** | Low | People struggle with the tradeoff between AI speed and AI accuracy. They don't have good heuristics for when to trust AI output directly vs. when to verify independently. |

#### PC-1.5-Meta: Metacognition and Calibration

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PC.1.5.1 Calibration | **High** | Poorly calibrated in both directions | Some people are overconfident ("I asked ChatGPT, so it must be right") while others are underconfident ("I can't use AI effectively, I'm not technical enough"). Neither group accurately assesses their own AI literacy. |
| PC.1.5.3 Error detection | **High** | Low | People frequently miss AI errors — fabricated citations, subtly wrong reasoning, confident assertions of false facts. Without domain expertise being actively engaged, errors pass through. |
| PC.1.5.5 Uncertainty awareness | **Medium** | Low | People don't recognize when they're getting poor results from AI. They lack the internal signal that says "this response doesn't seem right, I should try a different approach." |

#### PC-1.6-Shared: Shared Representations and Conceptual Alignment

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PC.1.6.1 Shared language | **High** | Low | There is no common vocabulary for AI usage within organizations. Terms like "prompt engineering," "hallucination," "context window," and even "AI" itself mean different things to different people. |
| PC.1.6.4 Common ground | **High** | Low | Teams don't have a shared understanding of how AI can help *their specific work*. An engineer's mental model of AI differs from a marketer's, and neither has been reconciled. |
| PC.1.6.8 Behavior specification | **High** | Undefined | "What good looks like" for AI-as-thought-partner is not defined. No one has specified: what constitutes effective AI use? How do you know you're doing it well? What does a good AI-assisted brainstorm look like compared to a poor one? |

---

### Opportunity — Physical (PO)

#### PO-2-Resource: Resource and Capacity Conditions

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PO.2.1 Time availability | **High** | Mid-to-low | Most knowledge workers are in time-scarce environments. Learning to use AI effectively requires an upfront time investment that competes with immediate deliverables. The irony: AI saves time once mastered, but people can't find the time to master it. |
| PO.2.4 Competing urgency | **High** | High | Day-to-day work urgency constantly displaces AI exploration. "I'll try using AI for that next time" becomes "I just need to get this done the way I know how." |
| PO.2.7 Activation overhead | **High** | Mid | Opening a new tool, context-switching from the current workflow, formulating a prompt, and evaluating the response is a non-trivial activation cost — especially when the person isn't confident they'll get value. |

#### PO-5-Tooling: Tooling and Interface Affordances

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PO.5.1 Affordance clarity | **Medium** | Mid | Modern AI chatbots (ChatGPT, Claude) have reasonably clear interfaces — a text box, a send button, a conversation thread. But the *cognitive* affordances are unclear: what should I type? What can I ask? How do I get better results? |
| PO.5.3 Core-path efficiency | **Medium** | Mid | The basic interaction is efficient (type → get response), but the high-value interaction (multi-turn refinement, uploading context, using system prompts) has higher friction. |
| PO.5.6 Learnability in context | **High** | Mid-to-high burden | AI tools are easy to *use* but hard to *use well*. The gap between basic usage and effective usage is large and not well-bridged by the tools themselves. There's no progressive disclosure of advanced techniques within the workflow. |

#### PO-4-Visibility: Information and State Visibility

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| PO.4.1 Signal surfacing | **High** | Low | The benefits of AI use are largely invisible to non-users. When someone uses AI to draft a memo faster, their colleagues see the memo — not the process. There are few visible signals of AI-assisted success to imitate. |
| PO.4.3 Feedback latency | **Medium** | Low-to-mid | The feedback on whether AI use actually improved outcomes (better document, faster turnaround, sharper strategy) is delayed and ambiguous. People can't easily tell if using AI made a difference. |

---

### Opportunity — Social (SO)

#### SO-1-Norms: Norms and Normative Climate

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| SO.1.1 Descriptive norm signal | **High** | Low-to-mid | In most organizations, AI use appears uncommon. Early adopters use it privately. There's limited visibility into who is using AI and how — so the descriptive norm signal says "most people don't do this." |
| SO.1.2 Injunctive norm signal | **Medium** | Mixed | Leaders often say they support AI use (positive injunctive norm) but haven't demonstrated it in their own work (inconsistent). Some leaders are privately skeptical or threatened. |
| SO.1.3 Norm clarity | **High** | Low | Normative cues are mixed: Is it OK to use AI for client-facing work? For strategic memos? For performance reviews? For code? The absence of guidelines means every use case carries ambiguity. |
| SO.1.4 Norm consistency | **High** | Low | Leaders say "embrace AI" while simultaneously asking "did you write this yourself?" The gap between stated and revealed norms is wide. Some managers celebrate AI use; others see it as a shortcut or cheating. |

#### SO-5-Legitimacy: Legitimacy, Meaning, and Identity Safety

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| SO.5.1 Legitimacy signal | **High** | Low-to-mid | Using AI is not yet fully legitimate in many professional contexts. There's an unspoken question: "If I use AI for this, will people think I'm lazy or incapable?" Legitimacy varies by task — using AI for research feels more legitimate than using it for a strategy recommendation. |
| SO.5.3 Identity safety | **High** | Low | For many professionals, using AI feels like admitting inadequacy. "I'm supposed to be the expert — why do I need a machine to help me think?" This is particularly acute for senior people whose identity is built on their expertise. |
| SO.5.5 Professional congruence | **High** | Low-to-mid | For some roles (engineers, analysts), AI use fits the professional identity. For others (creative directors, senior consultants, seasoned executives), it feels incongruent with the craft-based identity they've built over decades. |
| SO.5.6 Narrative support | **Medium** | Low | There is no compelling shared narrative within most organizations about *why* AI thought-partnership matters. The narrative is usually vendor-driven hype ("AI will transform everything") rather than grounded in the team's actual work. |

#### SO-6-Power: Power, Politics, and Psychological Safety

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| SO.6.1 Voice safety | **Medium** | Mid | In most organizations, it's reasonably safe to talk about AI — but it's less safe to *admit* you used AI for something important. The distinction matters: people can discuss AI abstractly but feel exposed when they reveal specific usage. |
| SO.6.5 Permission to experiment | **High** | Low-to-mid | Few organizations have created explicit safe-to-experiment zones for AI. People aren't sure what happens if they make a mistake using AI — share a hallucinated fact in a meeting, submit an AI-drafted document with an error, or accidentally feed sensitive data into a public AI tool. |
| SO.6.7 Transparency of rules | **High** | Low | Rules about AI use are either absent or implicit. Which data can go into AI tools? Which outputs need human review? What disclosure is expected? The absence of clear rules creates anxiety that suppresses experimentation. |

#### SO-4-Incentives: Incentives, Accountability, and Reinforcement Architecture

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| SO.4.1 Reward alignment | **High** | Misaligned | Most reward systems don't recognize AI-assisted work. Performance reviews don't ask about AI fluency. Promotions don't consider AI adoption. The reward system is neutral at best — and sometimes negative, when using AI is perceived as "not doing the work yourself." |
| SO.4.5 Recognition visibility | **High** | Low | When someone uses AI to produce great work, the AI contribution is invisible. The person gets credit for the output, but the practice of using AI as a tool isn't recognized or celebrated as a skill worth developing. |
| SO.4.6 Informal reinforcement | **Medium** | Mixed | In some teams, peer conversations celebrate AI discoveries ("Look what I got Claude to do!"). In others, AI mentions are met with eye-rolls or skepticism. The informal reinforcement landscape is highly inconsistent. |

---

### Motivation — Reflective (RM)

#### RM-1.2-Efficacy: Self-Efficacy

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| RM.1.2.1 Efficacy belief | **High** | Low for majority, high for early adopters | Most people have low AI self-efficacy. They've tried AI once or twice, gotten mediocre results, and concluded "I'm not good at this" or "AI isn't useful for my work." This is a self-reinforcing cycle: low efficacy → low effort → poor results → lower efficacy. |
| RM.1.2.3 Recovery after setbacks | **Medium** | Fragile | A single bad AI experience ("It made up a fake citation that I put in my report") creates lasting avoidance. People don't have the resilience framework to treat AI failures as learning opportunities. |
| RM.1.2.4 Task specificity | **Medium** | Broad uncertainty | People have diffuse, unspecified doubt about AI. They don't know *specifically* what they can and can't do with it, so everything feels uncertain. |
| RM.1.2.6 Source of efficacy | **High** | Weak | Very few people have had strong mastery experiences with AI. Vicarious experience is also limited (they haven't watched someone use AI effectively in their domain). The primary efficacy source has been media hype, which creates inflated expectations followed by disappointment. |

#### RM-1.3-EVC: Expectancy-Value-Cost

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| RM.1.3.1 Expectancy of success | **High** | Low for non-adopters | People who haven't developed AI fluency don't expect to get value from trying. The "expected value" of an AI interaction is low because their past experiences have been mixed. |
| RM.1.3.4 Utility value | **Medium** | Mid — recognized but abstract | Most people intellectually agree that AI could be useful. But "useful in theory" doesn't drive behavior — they need to experience the utility in their specific context. |
| RM.1.3.5 Effort cost | **High** | High | Learning to use AI well feels like a significant effort investment on top of an already full workload. The cost is front-loaded (learn now) while the benefit is back-loaded (save time later). |
| RM.1.3.8 Present-vs-future weighting | **High** | Present cost dominates | The temporal mismatch is stark: the cost of learning AI is felt today, but the productivity gains accrue over weeks and months. For time-pressed knowledge workers, present costs consistently win. |

#### RM-1.4-Identity: Identity-Based Motivation

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| RM.1.4.1 Identity congruence | **High** | Variable — strongly role-dependent | For some people, using AI fits their identity as an innovative, efficient professional. For others — particularly those whose identity is built on deep expertise, craftsmanship, or "doing the hard work" — AI threatens who they are. A senior strategist who prides themselves on original thinking may see AI assistance as diminishing. |
| RM.1.4.2 Prototypicality | **Medium** | Low for many roles | "Using AI tools" is not yet a prototypical behavior of most professional identities. A great marketer, consultant, or product manager is not yet *defined* by their AI fluency. |
| RM.1.4.4 Interpretation of difficulty | **Medium** | Difficulty signals mismatch | When AI interactions are frustrating, people interpret it as "AI isn't for me" rather than "I'm learning a new skill that takes practice." The difficulty-as-mismatch interpretation accelerates dropout. |

#### RM-1.5-Intentions: Goal Intentions and Implementation Intentions

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| RM.1.5.1 Intention strength | **Medium** | Weak-to-mid | Many people have a vague intention to "use AI more." But intention without specificity is inert. |
| RM.1.5.3 Plan specificity | **High** | Very low | Almost nobody has a specific plan: "When I start drafting a strategy document, I will first open Claude and brainstorm the key arguments." The if-then linkage between work context and AI action is absent. |
| RM.1.5.4 Cue linkage | **High** | No clear trigger | There is no environmental or habitual cue that triggers AI use. The work environment doesn't prompt "Have you considered using AI for this?" at the point of action. |
| RM.1.5.6 Initiation readiness | **Medium** | Low | Starting an AI interaction requires active decision-making every time. There's no smooth on-ramp from current workflow to AI-assisted workflow. |

---

### Motivation — Automatic (AM)

#### AM-2.1-Habit: Habit Formation

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| AM.2.1.1 Automaticity | **High** | Very low for target behavior | AI use is not automatic for most people. Every instance requires deliberate decision-making: "Should I use AI for this? Which tool? What do I type?" |
| AM.2.1.4 Context stability | **Medium** | Mid | Knowledge work contexts are moderately stable (same desk, same tools, similar task types), which is favorable for habit formation — but the habit-formation process hasn't started. |
| AM.2.1.7 Competing habit strength | **High** | High | Existing habits are deeply entrenched: Google search for research, blank document for drafting, solo brainstorming or team meetings for ideation. These are high-automaticity, well-practiced routines that AI must displace. |

#### AM-2.3-Affect: Affect and Emotion

| Dimension | Relevance | Position | Evidence |
|-----------|-----------|----------|----------|
| AM.2.3.1 Valence | **Medium** | Mixed | Emotional responses to AI are bifurcated. Some people feel excitement and curiosity (positive valence). Others feel anxiety, threat, or inadequacy (negative valence). The split often correlates with efficacy and identity. |
| AM.2.3.3 Anticipatory affect | **Medium** | Mixed | For some, anticipatory excitement ("What can AI do with this?") drives exploration. For others, anticipatory dread ("What if it gives me bad information?" "What if my boss finds out I used AI?") drives avoidance. |
| AM.2.3.5 Social-emotional intensity | **High** | Moderate-to-high | The fear of job replacement is a persistent background emotion. Even when not consciously articulated, the thought "Am I training my replacement?" creates a low-level anxiety that suppresses engagement. For some roles, this is acute. |

---

## Step 3: Practitioner Worksheet

### 1. COM-B Priority Ranking

| Rank | Branch | Rationale |
|------|--------|-----------|
| 1 | **Opportunity (O)** | Social opportunity is the primary gate. Mixed norms (SO.1.4), unclear legitimacy (SO.5.1), absent rules (SO.6.7), and misaligned incentives (SO.4.1) create an environment where even capable, motivated people hesitate. Physical opportunity reinforces this: low visibility of AI success (PO.4.1), competing urgency (PO.2.4), and activation overhead (PO.2.7) make it easy to default to existing behaviors. Opportunity must be addressed first because capability and motivation interventions fail in a hostile or ambiguous opportunity environment. |
| 2 | **Capability (C)** | Capability is a close second. Low procedural fluency (PC.1.1.2), inaccurate mental models (PC.1.2.1), weak judgment of AI output quality (PC.1.3.4), and poor metacognition (PC.1.5.1) mean that even when people try AI, they get mediocre results — which reinforces the belief that AI isn't useful. The absence of shared representations (PC.1.6) prevents organizational learning. Capability and Opportunity interact strongly: building capability without opportunity produces frustrated early adopters; creating opportunity without capability produces disappointing experiences. |
| 3 | **Motivation (M)** | Motivation is important but largely downstream of Opportunity and Capability. Low efficacy (RM.1.2.1), high perceived effort cost (RM.1.3.5), identity threats (RM.1.4.1), and absent implementation intentions (RM.1.5.3) all matter — but many of these will partially resolve when the opportunity environment improves and capability grows through positive experiences. The exception is the identity dimension (RM.1.4), which requires direct attention alongside Opportunity work, especially for senior professionals. |

---

### 2. Per-Lens Synthesis

### Capability (PC / PHC)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PC-1.1-Knowledge | PC.1.1.2 (procedural fluency): Low. PC.1.1.4 (skill stage): Novice. PC.1.1.6 (exception handling): Low. | Procedural fluency is the critical gap, not declarative knowledge. People have heard about AI; they can't *use* it effectively. TR is needed, not more ED about what AI is. Because AM.2.1.7 (competing habit strength) is high, TR must be paired with habit disruption (BCT.8.2, BCT.8.4). Because skill stage is novice, scaffolded TR with graded tasks is appropriate. | BCT.4.1 (instruction on how to perform), BCT.8.1 (behavioral practice/rehearsal), BCT.8.7 (graded tasks), BCT.6.1 (demonstration), BCT.8.2 (behavior substitution) |
| PC-1.2-Models | PC.1.2.1 (model accuracy): Low. PC.1.2.2 (causal understanding): Low. PC.1.2.7 (updateability): Mid. | Mental models are forming, not yet rigid — this is the window. BCT.4.4 (behavioral experiments) to surface model errors is more effective than lectures. The polarized "magic vs. useless" framing needs BCT.4.3 (re-attribution) to build a calibrated middle-ground model. | BCT.4.3 (re-attribution), BCT.4.4 (behavioral experiments), BCT.2.7 (feedback on outcomes), BCT.13.2 (framing/reframing) |
| PC-1.3-Judgment | PC.1.3.4 (recognition competence): Low. PC.1.3.2 (uncertainty tolerance): Low. | Judgment must be built through practice with feedback, not through rules. BCT.8.1 (practice) in realistic scenarios with BCT.2.2 (feedback) builds the pattern recognition that distinguishes expert AI users from novices. | BCT.8.1 (behavioral practice/rehearsal), BCT.2.2 (feedback on behaviour), BCT.6.1 (demonstration) |
| PC-1.5-Meta | PC.1.5.1 (calibration): Poorly calibrated. PC.1.5.3 (error detection): Low. | The overconfident segment (accepts AI output uncritically) needs BCT.2.2 (feedback on behaviour) to surface the gap. The underconfident segment needs BCT.15.1 (verbal persuasion about capability). Metacognition gates other capability interventions — if someone thinks they already know how to use AI, they won't engage with TR. | BCT.2.2 (feedback on behaviour), BCT.4.4 (behavioral experiments), BCT.15.1 (verbal persuasion about capability) |
| PC-1.6-Shared | PC.1.6.1 (shared language): Low. PC.1.6.4 (common ground): Low. PC.1.6.8 (behavior specification): Undefined. | This is critical for progression to Level 2. Without shared language and behavior specification, teams can't coordinate around AI use. BCT.4.1 (instruction) to establish common definitions. BCT.6.1 (demonstration) across roles. BCT.12.5 (adding objects) for shared glossaries and prompt libraries that actually work. | BCT.4.1 (instruction), BCT.6.1 (demonstration), BCT.12.5 (adding objects to environment), BCT.1.1 (goal setting, behavior) |

**Narrative synthesis:** The capability picture is dominated by a *procedural fluency gap*, not a *knowledge gap*. People know AI exists; they don't know how to use it well. This is compounded by inaccurate mental models that set up false expectations, poor metacognition that prevents people from recognizing when they're doing it wrong, and an absence of shared representations that prevents organizational learning from emerging. The most important insight is that the fluency gap is self-reinforcing: low fluency → poor results → lower perceived value → less practice → lower fluency. Breaking this cycle requires scaffolded practice (BCT.8.7) with immediate feedback (BCT.2.2), not more information delivery. What to avoid: lectures, webinars, and documentation dumps. These address the wrong kind of capability gap. What to try: hands-on workshops where people bring their own work tasks, guided prompting sessions with real-time feedback, and buddy systems that pair early adopters with curious novices.

### Opportunity (PO / SO)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PO-2-Resource | PO.2.1 (time availability): Mid-to-low. PO.2.4 (competing urgency): High. PO.2.7 (activation overhead): Mid. | Time scarcity is real but not absolute. The key lever is reducing activation overhead (PO.2.7) and embedding AI into existing routines rather than adding it as separate work. Don't create separate "AI time" — make AI the first step in work people are already doing. | BCT.12.1 (restructuring physical environment), BCT.1.4 (action planning), BCT.7.1 (prompts/cues) |
| PO-4-Visibility | PO.4.1 (signal surfacing): Low. PO.4.3 (feedback latency): Low-to-mid. | AI success is invisible. The person who used AI to draft a great memo gets credit for the memo, not for the AI skill. Making the practice visible — not just the output — is critical for norm formation (SO.1.1). | BCT.12.5 (adding objects), BCT.2.7 (feedback on outcomes), BCT.6.2 (social comparison) |
| PO-5-Tooling | PO.5.6 (learnability in context): High burden. PO.5.1 (affordance clarity): Mid. | Tools are usable but not learnable in context. The gap between "I can type in a box" and "I can have a productive AI conversation" is not bridged by the tools themselves. EN via BCT.12.5 (adding objects) like prompt templates and guided workflows at the point of action. | BCT.12.5 (adding objects), BCT.7.1 (prompts/cues), BCT.4.1 (instruction) |
| SO-1-Norms | SO.1.1 (descriptive norm): Low. SO.1.3 (norm clarity): Low. SO.1.4 (norm consistency): Low. | The descriptive norm says "most people don't use AI regularly." The injunctive norm is inconsistent: some leaders endorse it, others are skeptical. Norm consistency is the critical leverage point. Making AI use visible (MO via BCT.6.1) is necessary but insufficient if leader behavior contradicts the message. Leaders must model AI use, not just endorse it. | BCT.6.1 (demonstration), BCT.6.3 (information about others' approval), BCT.12.2 (restructuring social environment) |
| SO-5-Legitimacy | SO.5.1 (legitimacy signal): Low-to-mid. SO.5.3 (identity safety): Low. SO.5.5 (professional congruence): Variable. | Legitimacy is the social permission layer that gates adoption. People need to see that using AI is not "cheating" or "lazy" — it's a professional skill. BCT.9.1 (credible source) from respected figures in the organization. BCT.13.2 (framing/reframing) to position AI use as augmentation rather than replacement. | BCT.9.1 (credible source), BCT.13.2 (framing/reframing), BCT.6.1 (demonstration), BCT.3.1 (social support) |
| SO-6-Power | SO.6.5 (permission to experiment): Low-to-mid. SO.6.7 (transparency of rules): Low. | Absent rules create anxiety. People don't know what they're allowed to do with AI, so they either don't use it or use it secretly. Establishing clear, permissive guidelines (BCT.4.1 on what's allowed, BCT.12.2 to create safe-to-experiment zones) is a prerequisite for broader adoption. | BCT.12.2 (restructuring social environment), BCT.4.1 (instruction), BCT.1.1 (goal setting) |
| SO-4-Incentives | SO.4.1 (reward alignment): Misaligned. SO.4.5 (recognition visibility): Low. | The reward system doesn't recognize or incentivize AI use. Until AI fluency is valued in performance conversations, promotions, and team recognition, it will remain an optional extra that competes with recognized activities. | BCT.10.4 (social reward), BCT.10.5 (social incentive), BCT.12.2 (restructuring social environment) |

**Narrative synthesis:** The opportunity landscape has two dominant features: *social ambiguity* and *invisible success*. On the social side, the absence of clear norms, rules, and legitimacy signals creates a permission vacuum where people default to caution. The inconsistency between leader messaging and leader behavior (SO.1.4) is particularly damaging — it signals that AI endorsement is performative, not genuine. On the physical side, the invisibility of AI-assisted success (PO.4.1) prevents natural norm formation: people can't imitate what they can't see. What to try: leader modeling (leaders publicly sharing their own AI use, including failures), clear usage guidelines that are permissive rather than restrictive, and making AI-assisted workflows visible through demos, showcases, and shared examples. What to avoid: top-down mandates without leader behavior change (deepens the consistency gap), restrictive policies that make experimentation feel dangerous, and reward systems that implicitly penalize AI use.

### Motivation (RM / AM)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| RM-1.2-Efficacy | RM.1.2.1 (efficacy belief): Low for majority. RM.1.2.3 (recovery after setbacks): Fragile. RM.1.2.6 (source of efficacy): Weak. | Low efficacy is the primary motivation barrier. It must be addressed through mastery experiences (BCT.8.7 graded tasks), not through persuasion alone. The efficacy-capability cycle is key: build small wins first, let efficacy follow mastery. BCT.6.1 (demonstration) from relatable peers (not AI experts) provides vicarious experience. | BCT.8.7 (graded tasks), BCT.15.1 (verbal persuasion about capability), BCT.6.1 (demonstration), BCT.15.3 (focus on past success) |
| RM-1.3-EVC | RM.1.3.5 (effort cost): High. RM.1.3.8 (present-vs-future weighting): Present cost dominates. | The effort cost is partially real (learning takes time) and partially inflated by low efficacy. Reduce the real cost via EN (simpler on-ramps, template prompts) and address the perceived cost via PE (BCT.5.2 salience of consequences, BCT.9.3 comparative imagining). | BCT.5.2 (salience of consequences), BCT.9.3 (comparative imagining of future outcomes), BCT.13.2 (framing/reframing) |
| RM-1.4-Identity | RM.1.4.1 (identity congruence): Variable by role. RM.1.4.4 (difficulty → mismatch interpretation): Active. | For senior professionals and craft-oriented roles, identity is a significant barrier. Don't try to change people's identity — reframe the behavior as congruent with their existing identity. "Great strategists use every tool available" is more effective than "You need to adopt AI." BCT.13.2 (framing/reframing) and BCT.13.5 (identity associated with changed behavior). | BCT.13.2 (framing/reframing), BCT.13.5 (identity associated with changed behavior), BCT.6.1 (demonstration from identity-congruent models) |
| RM-1.5-Intentions | RM.1.5.3 (plan specificity): Very low. RM.1.5.4 (cue linkage): Absent. | The intention-action gap is wide because intentions are vague. People need specific if-then plans: "When I start writing a client brief, I will first open Claude and brainstorm the key messages." BCT.1.4 (action planning) bridges to BCT.8.3 (habit formation). | BCT.1.4 (action planning), BCT.7.1 (prompts/cues), BCT.8.3 (habit formation) |
| AM-2.1-Habit | AM.2.1.7 (competing habit strength): High. AM.2.1.1 (automaticity): Very low for AI use. | Existing workflows run on autopilot. AI must be inserted into the existing habit chain, not bolted on as a separate activity. BCT.8.2 (behavior substitution) is the key technique: identify the moment in the existing routine where AI replaces the old step. Context stability (AM.2.1.4) is favorable — people do similar work in similar settings, which supports habit formation if the cue linkage can be established. | BCT.8.2 (behavior substitution), BCT.8.3 (habit formation), BCT.7.1 (prompts/cues), BCT.12.1 (restructuring physical environment) |
| AM-2.3-Affect | AM.2.3.5 (social-emotional intensity): Moderate-to-high (job replacement fear). AM.2.3.1 (valence): Mixed. | The background anxiety about job replacement is real and can't be dismissed with reassurance. Address it directly via BCT.13.2 (framing/reframing) — position AI use as a career *advantage* rather than a career *threat*. BCT.3.3 (social support, emotional) through peer groups where anxieties can be named and normalized. | BCT.13.2 (framing/reframing), BCT.3.3 (social support, emotional), BCT.11.2 (reduce negative emotions) |

**Narrative synthesis:** Motivation is a picture of *stalled initiation*. People have weak, vague intentions that haven't been translated into specific plans. Low self-efficacy creates a learned-avoidance pattern: "AI isn't for me." The identity dimension adds a layer of resistance for experienced professionals. The key motivational lever is mastery experience — nothing changes motivation faster than a successful first use that clearly saves time on real work. What to try: facilitated "first win" sessions where someone brings a real work task and is coached through using AI to complete it faster and better; implementation intention prompts built into workflow tools; reframing campaigns that position AI fluency as a professional competitive advantage. What to avoid: motivational speeches and hype videos (they inflate expectations and deepen the disappointment cycle), mandatory AI usage targets (creates controlled rather than autonomous motivation, per RM-1.1-SDT), and dismissing job replacement fears as irrational.

---

### 3. Cross-Lens Interactions

**Tensions:**

- **Capability vs. Social Opportunity (PC.1.1 vs. SO.1.4):** Building skill through TR requires practice, but the social environment's norm inconsistency makes visible practice feel risky. People can't build procedural fluency if they're hiding their AI usage.
- **Efficacy vs. Identity (RM.1.2 vs. RM.1.4):** Building self-efficacy normally requires acknowledging you're a beginner and being willing to learn. But for senior professionals, being a beginner threatens the expert identity. The efficacy-building process itself is identity-threatening.
- **Visibility vs. Legitimacy (PO.4.1 vs. SO.5.1):** Making AI use visible (necessary for norm formation) requires people to be willing to be seen using AI (which requires legitimacy). This is a chicken-and-egg problem.

**Reinforcements:**

- **Low fluency → low efficacy → low usage → lower fluency.** PC.1.1.2, RM.1.2.1, and AM.2.1.1 form a self-reinforcing downward spiral. Breaking in at any point helps all three.
- **Invisible success → weak descriptive norm → continued hesitation.** PO.4.1 and SO.1.1 reinforce each other. Making success visible strengthens both simultaneously.
- **Absent rules → anxiety → avoidance.** SO.6.7, AM.2.3.5, and AM.2.1.1 form a chain: unclear rules create anxiety, which prevents the repetitions needed for habit formation.

**Prerequisites:**

- **SO.6.7 (transparent rules) before SO.1.1 (norm building):** People need to know what's allowed before they'll adopt publicly. Guidelines are a prerequisite for visible adoption.
- **PC.1.2.1 (mental model accuracy) before PC.1.3.4 (judgment):** People need a workable model of what AI can and can't do before they can develop judgment about output quality.
- **SO.5.1 (legitimacy) before RM.1.5.3 (implementation intentions):** People won't form specific plans to use AI until they believe it's legitimate to do so.

**Highest leverage (top 3):**

1. **Clear, permissive usage guidelines (SO.6.7 → SO.1.3 → AM.2.3 reduction):** Establishing transparent rules immediately reduces anxiety, clarifies norms, and unblocks experimentation. This is the single highest-leverage intervention because it's a prerequisite for almost everything else.
2. **Leader modeling + visible success stories (SO.1.4 → SO.1.1 → SO.5.1):** When leaders visibly use AI in their own work (not just endorse it) and AI-assisted successes are publicly shared, it simultaneously fixes norm consistency, raises the descriptive norm, and builds legitimacy. One credible senior leader sharing "Here's how I used AI to prepare for the board meeting" does more than a hundred awareness campaigns.
3. **Facilitated first-win experiences (PC.1.1.2 → RM.1.2.1 → AM.2.1.1):** Guided sessions where employees bring their own work tasks and are coached through a successful AI interaction break the fluency-efficacy-habit spiral at all three points simultaneously.

---

### 4. BCW Function Ranking

| Rank | Function | Rationale | Top 3 BCTs |
|------|----------|-----------|------------|
| 1 | **MO — Modelling** | Modelling addresses the highest-leverage cross-lens interaction: the visibility-norm-legitimacy nexus. With SO.1.1 low, SO.1.4 inconsistent, SO.5.1 shaky, and PO.4.1 buried, showing real people using AI effectively in real work is the most efficient way to move multiple barriers at once. Modelling from high-status, identity-congruent figures also addresses RM.1.4.1 (identity congruence). | BCT.6.1 (demonstration of the behavior) — leaders and respected peers demonstrate AI use on real tasks. BCT.6.3 (information about others' approval) — signal that admired colleagues and leaders endorse AI use. BCT.16.3 (vicarious consequences) — make the positive outcomes of AI use observable to non-users. |
| 2 | **EN — Enablement** | Enablement addresses the capability-opportunity bottleneck. PC.1.1.2 (procedural fluency) is low, PO.2.7 (activation overhead) is present, and RM.1.5.3 (plan specificity) is absent. EN removes barriers and creates the conditions for the behavior to start and sustain: scaffolded tools, simplified workflows, specific plans, and social support. | BCT.8.7 (graded tasks) — design progressive AI challenges from simple to complex. BCT.12.5 (adding objects to environment) — prompt templates, quick-start guides, and curated AI bookmarks at point of work. BCT.3.1 (social support) — peer learning groups and AI buddy systems. |
| 3 | **ER — Environmental Restructuring** | ER addresses the structural barriers that suppress behavior. SO.6.7 (absent rules) creates anxiety; PO.4.1 (invisible success) prevents norm formation; SO.4.1 (misaligned incentives) removes reinforcement. ER changes the environment so the behavior is easier, safer, and more visible. | BCT.12.2 (restructuring social environment) — establish clear AI usage guidelines, create "show and tell" forums, integrate AI fluency into performance conversations. BCT.12.1 (restructuring physical environment) — embed AI tools into existing workflow tools (IDE plugins, browser extensions, document editor integrations). BCT.7.1 (prompts/cues) — "Have you tried AI for this?" nudges in project kickoffs and document templates. |
| 4 | **ED — Education** | ED addresses the mental model gap (PC.1.2.1) and the shared representation gap (PC.1.6). People need a workable conceptual model of what AI can and can't do, how to prompt effectively, and what "good use" looks like. ED is ranked 4th (not higher) because information alone doesn't drive the behavior — but without accurate mental models, practice is unproductive. | BCT.4.1 (instruction on how to perform) — practical prompting guides, not abstract AI literacy content. BCT.4.3 (re-attribution) — correct the "magic vs. useless" mental model to a calibrated "powerful tool with specific strengths and limitations" model. BCT.5.3 (information about social and environmental consequences) — make the organizational value of AI fluency concrete and specific. |
| 5 | **PE — Persuasion** | PE addresses the identity barrier (RM.1.4.1), the efficacy gap (RM.1.2.1), and the emotional dimension (AM.2.3.5). It shifts beliefs and emotional associations. PE is essential for the senior-professional segment where identity resistance is strongest, and for the broader population where job-replacement anxiety suppresses engagement. | BCT.13.2 (framing/reframing) — reframe AI use from "replacement threat" to "augmentation advantage" and from "shortcut/cheating" to "professional skill." BCT.15.1 (verbal persuasion about capability) — build confidence that effective AI use is learnable. BCT.9.1 (credible source) — respected industry figures endorsing AI thought-partnership. |

**Contraindicated:**

- **COE — Coercion:** Mandating AI use would create controlled motivation (RM.1.1.1), trigger identity resistance (RM.1.4), and generate compliance theater rather than genuine adoption. People would use AI to check a box without developing real fluency. In an already anxious environment (AM.2.3.5), coercion deepens fear rather than building capability.
- **RE — Restriction:** Restricting non-AI workflows (e.g., "You must use AI before submitting any document") would backfire. People don't yet have the capability to use AI effectively, so forced reliance would produce worse outputs and confirm skeptics' belief that AI isn't useful.

---

### 5. Intervention Implications

**MO (Modelling):** The intervention looks like a curated program of visible AI use by influential people. Identify 3-5 senior leaders and 5-10 respected individual contributors across different functions. Ask each to publicly share one specific instance per week where they used AI — including what worked, what didn't, and what they learned. Format: short Slack posts, 5-minute team meeting slots, or brief video walkthroughs. The key is authenticity and specificity — not polished demos but real work with real imperfections.

**EN (Enablement):** The intervention looks like a structured "first 30 days" program. Week 1: bring one real work task to a facilitated AI session and complete it with coaching (BCT.8.7 graded tasks). Week 2: try a slightly harder task independently with a prompt template (BCT.12.5 adding objects). Weeks 3-4: partner with an AI buddy for accountability and troubleshooting (BCT.3.1 social support). Ongoing: specific if-then implementation plans — "When I start [specific work task], I will first [specific AI action]" (bridges to AM-2.1-Habit via BCT.1.4 and BCT.8.3).

**ER (Environmental Restructuring):** The intervention looks like three structural changes. (1) Publish a clear, permissive AI usage policy: what data can and can't go into AI tools, which tools are approved, what disclosure is expected, and an explicit statement that using AI is encouraged and supported (SO.6.7 → BCT.12.2). (2) Integrate "AI assist" prompts into existing workflows — a checklist item in project kickoffs, a template section in document outlines, a question in sprint planning (BCT.7.1 prompts/cues). (3) Create a regular "AI show and tell" forum where people share what they've tried — modeled after a demo day, low-stakes, curiosity-driven (BCT.12.2 social restructuring + BCT.6.1 demonstration synergy).

**ED (Education):** The intervention looks like a concise, role-specific "AI mental model" primer — not a course, but a 20-minute orientation that corrects the top 3 mental model errors (AI is magic, AI is just search, AI always hallucinates) and provides a practical framework for when and how to use AI. Followed by role-specific prompt collections that demonstrate effective prompting patterns for that function's actual work. Delivered at the point of action, not in a separate learning system.

**PE (Persuasion):** The intervention looks like a reframing campaign with two tracks. Track 1 (broad): Reframe AI use from "replacement threat" to "augmentation multiplier" through credible testimonials, data on time saved, and case studies of AI-augmented success. Track 2 (targeted at senior professionals): one-on-one or small-group conversations with respected peers who have integrated AI into their expert practice. The message: "The best strategists, writers, and analysts are now AI-fluent — this is the new professional standard."

---

## Step 4: BCW and BCT Reasoning

### Dimensional findings → BCW functions mapping

| COM-B Branch | Key Dimensional Finding | Primary BCW Functions |
|-------------|------------------------|----------------------|
| PC (Capability) | PC.1.1.2 low fluency, PC.1.2.1 inaccurate models | ED, TR, EN |
| PO (Physical Opportunity) | PO.2.7 activation overhead, PO.4.1 invisible success | ER, EN |
| SO (Social Opportunity) | SO.1.4 norm inconsistency, SO.5.1 low legitimacy, SO.6.7 absent rules | MO, ER, EN |
| RM (Reflective Motivation) | RM.1.2.1 low efficacy, RM.1.4.1 identity threat, RM.1.5.3 absent plans | PE, EN |
| AM (Automatic Motivation) | AM.2.1.7 strong competing habits, AM.2.3.5 job replacement anxiety | ER, PE, EN |

### Consolidated BCT selection by function

**MO:** BCT.6.1 (demonstration), BCT.6.3 (information about others' approval), BCT.16.3 (vicarious consequences)

**EN:** BCT.8.7 (graded tasks), BCT.12.5 (adding objects), BCT.3.1 (social support), BCT.1.4 (action planning), BCT.7.1 (prompts/cues)

**ER:** BCT.12.2 (restructuring social environment), BCT.12.1 (restructuring physical environment), BCT.7.1 (prompts/cues)

**ED:** BCT.4.1 (instruction), BCT.4.3 (re-attribution), BCT.5.3 (information about social/environmental consequences)

**PE:** BCT.13.2 (framing/reframing), BCT.15.1 (verbal persuasion about capability), BCT.9.1 (credible source), BCT.13.5 (identity associated with changed behavior)

---

## Step 5: Recommendations

### Phase A: Summary and Key Insights

#### Summary

Most organizations trying to get employees to use AI as a thought partner are treating it as an awareness or tooling problem: they buy licenses, send emails, and host webinars. But the real barriers are elsewhere. The social environment is ambiguous — people don't know if AI use is truly welcome, rules are unclear, and leaders endorse AI without visibly using it themselves. This permission vacuum means even curious employees hesitate. Meanwhile, the people who do try AI often get disappointing results because they lack the procedural fluency to prompt effectively, and their mental models of what AI can and can't do are inaccurate. This creates a self-reinforcing cycle: poor results → low confidence → less practice → poorer results.

The highest-leverage path forward has three pillars. First, clear the permission space: publish transparent, permissive usage guidelines and have leaders model AI use in their own work (not just talk about it). Second, create structured first-win experiences: guided sessions where people use AI on their real work tasks and experience tangible value in a supported environment. Third, make AI-assisted success visible across the organization so that the descriptive norm shifts from "most people don't use AI" to "people like me use AI regularly and effectively." These three moves address the opportunity-capability-motivation cycle simultaneously and create the conditions for organic, sustained adoption.

#### Key Insights

1. **The biggest barrier isn't awareness or tools — it's social permission.** Most employees can access AI tools. What they can't access is clear, consistent signals that using AI is legitimate, encouraged, and professionally safe. The gap between what leaders say ("embrace AI") and what leaders do (not visibly using AI themselves) is the single most damaging dynamic. Fix this first.

2. **Low AI fluency is self-reinforcing, and information won't break the cycle.** People try AI once, get a mediocre result because they don't know how to prompt effectively, conclude AI isn't useful, and stop trying. More information about AI won't help — they need coached, successful first experiences with their own real work tasks. One guided 30-minute session where someone drafts a better document with AI does more than ten hours of AI literacy training.

3. **For senior professionals, the identity barrier is real and must be respected.** Experienced leaders and specialists may resist AI not because they're Luddites but because their professional identity is built on expertise and original thinking. Telling them to "just try it" feels dismissive. The effective approach is to reframe AI use as what the best practitioners do — a mark of sophistication, not inadequacy — and to let them see peers they respect using AI effectively.

4. **The intention-action gap is wide because nobody has specific plans.** Vague intentions ("I should use AI more") don't produce behavior. What works is if-then planning: "When I start drafting a client brief, I will first open Claude and brainstorm the key arguments." These specific cue-action links are the bridge between wanting to use AI and actually using it.

5. **Organizations get stuck at Level 1 because individual adoption stays invisible.** When AI use is private and ad-hoc, there's no way for the organization to learn from its best users, develop shared practices, or build the collective capability needed for Level 2. Making AI use visible — through showcases, shared examples, and team discussions — is what turns scattered individual value into the foundation for organizational capability.

---

### Phase B: In-Depth Report

#### Digest Block

```text
dimensions = PC.1.1.2 low, PC.1.2.1 low, PC.1.5.1 miscalibrated, PC.1.6.8 undefined, PO.2.4 high, PO.4.1 low, SO.1.4 low, SO.5.1 low-mid, SO.6.7 low, SO.4.1 misaligned, RM.1.2.1 low, RM.1.4.1 variable, RM.1.5.3 very low, AM.2.1.7 high, AM.2.3.5 moderate-high
tensions   = "C present in pockets but SO ambiguous; RM.1.2 vs RM.1.4 for senior staff; PO.4.1 vs SO.5.1 chicken-and-egg"
leverage   = SO.6.7 (transparent rules), SO.1.4 + PO.4.1 (leader modeling + visible success), PC.1.1.2 + RM.1.2.1 (first-win experiences)
functions  = MO > EN > ER > ED > PE
bcts       = MO→BCT.6.1,BCT.6.3,BCT.16.3 | EN→BCT.8.7,BCT.12.5,BCT.3.1,BCT.1.4,BCT.7.1 | ER→BCT.12.2,BCT.12.1,BCT.7.1 | ED→BCT.4.1,BCT.4.3,BCT.5.3 | PE→BCT.13.2,BCT.15.1,BCT.9.1,BCT.13.5
```

#### Lens Analysis: Capability Findings

##### Procedural Fluency (PC-1.1)

The defining capability gap is procedural, not declarative. Employees have been saturated with information about AI — articles, demos, vendor presentations — but very few have developed the *skill* of using AI effectively. Effective AI thought-partnership is a multi-step procedure: (1) frame the problem, (2) provide relevant context, (3) craft a specific prompt, (4) evaluate the response critically, (5) iterate with refinements, (6) extract and adapt the useful output. Most people perform step 1 and jump to step 3 with a vague prompt, skip steps 4-5, and either accept mediocre output or reject the tool entirely.

The skill stage (PC.1.1.4) is novice for the majority. This means scaffolded training with graded tasks (BCT.8.7) is the appropriate approach — start with simple tasks where AI clearly outperforms the unassisted approach (e.g., brainstorming 10 alternative titles for a document), then progress to more complex tasks (e.g., using AI to stress-test a strategy). The competing habit of traditional work methods (AM.2.1.7) means that new procedural knowledge must be explicitly linked to behavior substitution (BCT.8.2): "Instead of staring at a blank page, open Claude first."

##### Mental Models (PC-1.2)

Mental models of AI are polarized and inaccurate. The "magic" model leads to disappointment when AI can't read minds or produce perfect output on the first try. The "just a search engine" model leads to underuse — people ask AI for facts when its real value is in brainstorming, synthesis, critique, and drafting. The good news: model updateability (PC.1.2.7) is mid-range, meaning these models are not yet entrenched and can be corrected. The window for model-shaping is now. Behavioral experiments (BCT.4.4) — "Try asking AI to argue against your own proposal and see what happens" — are more effective than lectures because they produce surprise, which updates models.

##### Metacognition and Judgment (PC-1.5, PC-1.3)

Poor metacognition compounds the fluency gap. Overconfident users accept AI hallucinations without verification; underconfident users give up too quickly. Neither group can accurately self-assess their AI competence. This means that feedback on behavior (BCT.2.2) must be built into early training — not just teaching prompting skills, but teaching people to recognize when they're getting good vs. bad results and when their own evaluation is biased. Judgment about AI output quality (PC.1.3.4) can only be built through practice with varied examples and expert feedback; it cannot be taught declaratively.

##### Shared Representations (PC-1.6)

The absence of shared language and behavior specification is the primary barrier to progressing from Level 1 to Level 2. If "AI as a thought partner" means something different to every person and team, there's no foundation for shared practices, quality criteria, or organizational learning. Establishing common definitions — what counts as effective AI use, what "good looks like" for an AI-assisted brainstorm vs. an AI-assisted draft — is necessary infrastructure for scaling beyond individual ad-hoc usage.

#### Lens Analysis: Opportunity Findings

##### Physical Opportunity

Time scarcity (PO.2.1) and competing urgency (PO.2.4) are real but manageable. The key insight is that AI use should not be positioned as *additional* work that requires extra time. Instead, it should be embedded as the *first step* of existing work. If the activation overhead (PO.2.7) is reduced — tools pre-loaded, prompts pre-staged, templates available — the time cost of trying AI drops from "learn a new tool" to "type a sentence and see what happens." The invisibility of AI success (PO.4.1) is more pernicious than resource scarcity. Without visible success stories, the descriptive norm cannot shift, and each person must independently discover AI's value — a deeply inefficient adoption path.

##### Social Opportunity

Social opportunity is the primary bottleneck. Three forces interact to suppress adoption:

**Norm inconsistency (SO.1.4):** The gap between stated support and revealed behavior from leadership is the most corrosive dynamic. When a VP says "We should all be using AI" but has never visibly used it, employees read the implicit message: "AI is for you to adopt, not for me." This inconsistency is worse than silence because it signals inauthenticity.

**Absent rules (SO.6.7):** Without clear guidelines, every AI interaction carries ambiguity: Can I paste this data? Do I need to disclose? What if the output is wrong? The absence of rules creates a default-to-caution posture. Notably, restrictive rules are almost as bad as absent rules — if the policy says "Don't use AI for anything client-facing," it eliminates the highest-value use cases and signals that AI is dangerous rather than useful.

**Legitimacy gap (SO.5.1, SO.5.3):** Using AI still carries a stigma in many professional contexts. The "cheating" narrative — that AI-assisted work is somehow less valid — is the social-level expression of individual identity threats (RM.1.4). This narrative must be actively countered by credible figures modeling AI use without shame or qualification.

#### Lens Analysis: Motivation Findings

##### Reflective Motivation

Low self-efficacy (RM.1.2.1) is the central motivational barrier. It is tightly coupled with the capability gap: people correctly perceive that they're not good at using AI (because they aren't, yet), and this perception prevents them from practicing (which would make them better). The important distinction is between *correctly calibrated low efficacy* (people who accurately perceive they need to learn more) and *over-generalized low efficacy* (people who conclude "AI isn't for me" from a few bad experiences). The first group needs capability building (TR, EN); the second needs re-attribution (PE via BCT.4.3) before they'll engage.

The identity dimension (RM.1.4) is the most emotionally charged motivational barrier and requires the most careful handling. For senior professionals, suggesting they need AI is heard as "your expertise isn't enough." This is not irrational — it's a reasonable inference in an environment where AI is often framed as replacing human judgment. The reframing must be genuine: AI as a thought partner doesn't replace expertise; it amplifies it. The most effective intervention is demonstration by identity-congruent models — a respected senior strategist showing how they use AI to stress-test their own thinking, not to replace it.

##### Automatic Motivation

Competing habits (AM.2.1.7) are the primary automatic-motivation barrier. Knowledge workers have deeply ingrained workflows: open browser → search Google, open document → start typing, feel stuck → ask a colleague. These are high-automaticity routines that will continue to run unless deliberately disrupted. The habit-formation strategy must focus on behavior substitution: identifying the specific moment in the existing routine where AI can be inserted, and making that substitution as frictionless as possible.

The job-replacement anxiety (AM.2.3.5) is a background emotional force that doesn't always surface in conversation but consistently influences behavior. It creates an approach-avoidance conflict: people are curious about AI but also wary of engaging too deeply with something that might eliminate their role. This can't be resolved through reassurance alone — it requires organizational signals that AI fluency is a career asset, not a career risk. Embedding AI skills into career development frameworks and promotion criteria sends this signal more powerfully than any communication campaign.

#### Cross-Lens Assessment

The three highest-leverage findings, in order:

**1. Clear, permissive guidelines (SO.6.7) unlock everything downstream.** This is the prerequisite intervention. Without transparent rules, people can't experiment safely (SO.6.5), visible adoption can't emerge (SO.1.1), and anxiety (AM.2.3) persists. Establishing guidelines is fast, inexpensive, and immediately unblocking. The guidelines should be permissive by default ("You are encouraged to use AI for...") with specific restrictions only where legally or ethically necessary ("Do not input [specific data types]").

**2. Leader modeling (SO.1.4 → SO.1.1 → SO.5.1) resolves three social barriers simultaneously.** When leaders visibly use AI, it closes the norm consistency gap, raises the descriptive norm, and signals legitimacy. This is the most efficient multi-barrier intervention available. The prerequisite is that leaders must actually use AI — not perform a scripted demo, but genuinely integrate it into their work and share honestly about what works and what doesn't.

**3. Facilitated first-win experiences (PC.1.1.2 → RM.1.2.1 → AM.2.1.1) break the self-reinforcing downward cycle.** This intervention directly attacks the fluency-efficacy-habit spiral by producing positive outcomes that update beliefs and begin establishing new routines. The prerequisite is that the experience must use the person's real work tasks — artificial exercises don't transfer.

The primary tension is between Capability and Social Opportunity. TR/EN work to build capability requires practice, which requires social permission. But social permission depends partly on visible success, which depends on capability. The resolution is to start with the Opportunity interventions (guidelines + leader modeling) to create the permission space, then immediately follow with the Capability intervention (first-win experiences) while the permission space is fresh.

#### BCW and BCT Reasoning

**Modelling (MO) ranked first** because it simultaneously addresses social opportunity barriers that gate all other interventions. BCT.6.1 (demonstration) from leaders and respected peers normalizes AI use, raises descriptive norms, and provides vicarious efficacy. BCT.6.3 (information about others' approval) explicitly signals social permission. BCT.16.3 (vicarious consequences) lets non-users observe the positive outcomes of AI use without personal risk.

**Enablement (EN) ranked second** because it translates social permission into individual action. BCT.8.7 (graded tasks) designs a progressive skill-building path that guarantees early success (addressing RM.1.2.1). BCT.12.5 (adding objects) places prompt templates and quick-start guides at the point of action (addressing PO.2.7). BCT.3.1 (social support) through peer learning groups provides both practical help and emotional safety. BCT.1.4 (action planning) bridges intentions to specific if-then plans (addressing RM.1.5.3). BCT.7.1 (prompts/cues) triggers AI use at natural work inflection points.

**Environmental Restructuring (ER) ranked third** because it changes the structural conditions that suppress behavior. BCT.12.2 (restructuring social environment) establishes usage guidelines, creates forums for sharing, and integrates AI fluency into performance frameworks (addressing SO.6.7, SO.4.1). BCT.12.1 (restructuring physical environment) embeds AI tools into existing workflow software (addressing PO.2.7). BCT.7.1 (prompts/cues) adds "Have you tried AI?" nudges to existing process checkpoints.

**Education (ED) ranked fourth** because accurate mental models (PC.1.2) are a prerequisite for productive practice — but only a prerequisite, not a driver. BCT.4.1 (instruction) provides practical how-to content, not theoretical AI literacy. BCT.4.3 (re-attribution) corrects the polarized "magic vs. useless" model. BCT.5.3 (information about consequences) makes the organizational stakes concrete.

**Persuasion (PE) ranked fifth** because it addresses the identity and emotional barriers that ED and TR can't reach. BCT.13.2 (framing/reframing) repositions AI from threat to advantage. BCT.15.1 (verbal persuasion about capability) rebuilds confidence for the under-confident segment. BCT.9.1 (credible source) leverages respected figures to endorse the reframing. BCT.13.5 (identity associated with changed behavior) helps professionals incorporate AI fluency into their self-concept.

#### Framework Observations

This diagnosis reveals a pattern common to technology adoption in organizations: the problem is framed as a technology problem (better tools, more features, enterprise licenses) when it is actually a behavior-change problem involving capability gaps, social permission structures, identity dynamics, and habit formation. The COM-B framework surfaces three dynamics that a technology-first frame completely misses:

1. **The social permission layer is invisible but decisive.** Organizations invest heavily in tools and training while the social environment quietly vetoes adoption through norm ambiguity, inconsistent leadership signals, and absent rules. This is where most Level 1 organizations are stuck.

2. **The fluency-efficacy spiral is the primary retention mechanism.** Getting people to try AI once is relatively easy. Getting them to persist through the learning curve — where results are inconsistent and the old way is faster — requires deliberate scaffolding, not just access.

3. **Progression from Level 1 to Level 2 requires collective, not just individual, capability.** The shared representations gap (PC.1.6) is what prevents organizations from moving beyond ad-hoc usage. Until teams have shared language, shared quality criteria, and shared practices for AI use, organizational-level AI maturity cannot emerge.

The risk of over-indexing on Modelling and Persuasion without building Capability and Enablement is that adoption becomes performative — people talk about AI and endorse it but don't develop the fluency to use it effectively. The risk of over-indexing on Education and Training without addressing Social Opportunity is that skilled users hide their AI fluency because the social environment doesn't support it. The balanced approach — clear the permission space, build first wins, then sustain through structural changes — addresses both risks.
