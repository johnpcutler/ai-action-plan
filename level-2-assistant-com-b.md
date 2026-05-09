← [Home](README.md) | [Deep Dives](deep-dives.md) | [Diagnostic Report](combined-com-b-report.md) | [Action Plan](ai-maturity-action-plan.md)

---

# COM-B Behavioral Diagnosis: AI as an Assistant (Level 2)

**AI Maturity Model — Level 2**
**Subtitle:** Complete individual tasks faster, save employee time

---

## Step 1: Behavior Canvas

### Behavior A — Adoption Behavior

| Field | Definition |
|-------|-----------|
| **Behavior** | Employees consistently use AI assistants embedded in their daily tools (writing, meeting notes, search, data entry) to save time and improve output quality |
| **Who** | Individual contributors across the organization — knowledge workers, managers, operational staff — varying by role, technical comfort, and tool access |
| **Will do what** | Use AI features within their existing tools (Notion AI, GitHub Copilot, Otter.ai, enterprise search, smart auto-fill) as a regular part of task execution — prompting, reviewing AI output, accepting/editing suggestions, and incorporating AI-generated summaries into their workflow |
| **To what extent** | Daily use across at least 2-3 core work activities (writing/editing, meeting follow-up, information retrieval); AI-assisted output becomes the default starting point rather than a blank page; measurable time savings of 2-5 hours/week per employee |
| **In what context** | Within existing enterprise tools and platforms that have embedded AI features; during normal work hours; governed by company AI usage guidelines; across distributed and in-office settings |
| **For what outcome** | Measurable individual time savings; fewer manual, repetitive tasks; higher quality outputs with AI-assisted editing and review; meeting time becomes more actionable with AI summaries; organization builds the behavioral foundation for workflow-level AI integration (Level 3) |
| **Current state** | **Partially Realized / Inconsistent** — AI tools are available and some employees use them regularly, but adoption is patchy. Early adopters are enthusiastic; a large middle group has tried tools but hasn't built habits; a trailing group hasn't engaged meaningfully. Productivity gains exist in pockets but are not yet compounding across the organization. |
| **Prior attempts** | Many organizations have tried: (1) mass license provisioning without training — tools sit unused; (2) lunch-and-learn demos that generate excitement but no sustained behavior change; (3) top-down mandates to "use AI" without specifying what that looks like — creates compliance theater; (4) sharing "prompt libraries" that don't connect to people's actual workflows. These attempts typically address capability or motivation in isolation without touching the opportunity and social structures that sustain behavior. |

### Behavior B — Progression Blocker

| Field | Definition |
|-------|-----------|
| **Behavior** | Organizations achieve individual productivity gains but can't compound them into team-level workflow automation (Level 3) |
| **Who** | Team leads, managers, and operational leaders who would need to redesign workflows; individual contributors whose AI use remains siloed; IT/ops teams who would need to integrate AI into shared systems |
| **Will do what** | Transition from individual AI tool use to shared, team-level AI-augmented workflows — connecting individual AI outputs into collaborative processes, automating handoffs, building shared prompt libraries, and redesigning team workflows around AI capabilities |
| **To what extent** | At least one core team workflow per quarter is redesigned to incorporate AI at the process level (not just individual task level); team-level metrics show compounding gains beyond the sum of individual time savings |
| **In what context** | Cross-functional team settings; existing project management and collaboration infrastructure; within governance frameworks that may not yet accommodate AI-augmented processes |
| **For what outcome** | Transition from individual productivity to team-level efficiency; workflow automation that compounds individual gains; organizational readiness for Level 3 (AI-augmented workflows) |
| **Current state** | **Aspirational Only** — Individual gains are visible but remain siloed. No systematic mechanism exists to aggregate individual AI use into team-level workflow redesign. The organizational conversation is still about individual tool adoption, not process transformation. |
| **Prior attempts** | Some organizations have tried: (1) appointing "AI champions" who evangelize but lack authority to redesign workflows; (2) running hackathons that produce prototypes but not sustained process changes; (3) creating centers of excellence that produce documentation nobody reads. The common failure mode is treating progression as an education problem when it's actually a governance, role clarity, and workflow architecture problem. |

---

## Step 2: Dimensional Lens Analysis

### Capability (PC)

#### PC-1.1-Knowledge: Declarative and Procedural Knowledge

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.1.1 Declarative knowledge | Low-to-Mid | Most employees have heard of AI features in their tools but lack understanding of what the tools can actually do across use cases. They know "Notion has AI" but not the fifteen different ways it can be applied. |
| PC.1.1.2 Procedural fluency | Low | Even employees who know AI features exist often lack fluency in using them — they don't know how to write effective prompts, how to iterate on AI output, or how to integrate AI steps into their existing task sequences. |
| PC.1.1.3 Sequence clarity | Low | The "how to" of AI-assisted work is poorly specified. When should you prompt AI vs. write from scratch? What's the edit-review cycle for AI-generated content? People lack clear procedural sequences. |
| PC.1.1.6 Exception handling | Low | Users struggle when AI output is mediocre — they either accept bad output or abandon the tool entirely. They lack strategies for debugging prompts, adjusting context, or knowing when to switch approaches. |

**Relevance:** High. This is a foundational gap. Most organizations have provided tools without building the procedural knowledge needed to use them effectively.

#### PC-1.2-Models: Mental Models

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.2.1 Model accuracy | Low-to-Mid | Many employees hold inaccurate mental models of AI — either "it's magic and should be perfect" or "it's useless hype." Few understand that AI assistants are probabilistic text generators that require human judgment. |
| PC.1.2.2 Causal understanding | Low | People don't understand why AI produces good output sometimes and poor output other times. Without understanding how context, prompt quality, and model limitations interact, they can't systematically improve their results. |
| PC.1.2.7 Updateability | Mid | Most employees are willing to update their understanding, but many have formed initial impressions (positive or negative) based on early experiences that now anchor their expectations. |

**Relevance:** High. Faulty mental models drive both over-trust (accepting hallucinated content) and under-trust (dismissing useful output because one bad experience poisoned the well).

#### PC-1.3-Judgment: Judgment and Decision Competence

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.3.3 Heuristic quality | Low | People lack good decision rules for AI use. Common bad heuristics: "If it sounds right, it's right" (over-trust), "AI can't do anything creative" (under-trust), "I'll just paste the whole document in" (context overload). |
| PC.1.3.5 Rule dependence | Mid-High | Many users follow rigid rules ("always use AI for summaries, never for strategy docs") rather than developing context-sensitive judgment about when AI adds value. |
| PC.1.3.7 Tradeoff handling | Low | Users struggle with the speed-vs-quality tradeoff: when is AI-generated "good enough" versus when does it need heavy editing? When does the time spent editing AI output exceed the time to write from scratch? |

**Relevance:** High. The core Level 2 behavior requires calibrated judgment — knowing when to use AI, when to trust its output, and when to invest in editing versus starting fresh.

#### PC-1.5-Meta: Metacognition and Calibration

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.5.1 Calibration | Bimodal | Two failure modes coexist: over-confident users who trust AI output without review ("it's from the AI, it must be well-researched") and under-confident users who redo everything AI produces ("I need to check every sentence"). Both waste time. |
| PC.1.5.3 Error detection | Low | Users frequently miss AI errors — factual inaccuracies, subtle tone mismatches, hallucinated citations — because they lack the metacognitive habit of critical review of AI output. |
| PC.1.5.6 Help-seeking readiness | Low-Mid | Many employees won't ask colleagues for help with AI tools because they feel they "should already know this" or fear appearing incompetent with technology. |

**Relevance:** High. Calibration is the gateway to safe, productive AI use. Without it, the organization either gets low-quality AI-assisted output or abandons the tools.

#### PC-1.6-Shared: Shared Representations

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.6.1 Shared language | Low | Teams lack shared vocabulary for AI use — "prompt," "context window," "hallucination" mean different things to different people, or mean nothing at all. |
| PC.1.6.4 Common ground | Low | No shared understanding of what "using AI well" looks like across the organization. One team's power user is another team's cautionary tale. |
| PC.1.6.8 Behavior specification | Low | "Use AI in your daily work" is undefined. What counts as AI-assisted work? What quality bar applies? There's no shared specification of the target behavior. |

**Relevance:** High for Behavior B (progression blocker). Individual adoption can proceed with individual capability, but compounding gains requires shared representations and aligned practices across teams.

#### PC-1.7-Scaffold: Supported Performance

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.7.1 Independence | Low | Most employees can use AI tools with step-by-step guidance but cannot independently identify opportunities for AI use or design their own AI-assisted workflows. |
| PC.1.7.3 Prompt dependence | High | Many users depend on pre-made prompt templates and cannot generalize to new situations. Remove the template library and usage drops. |
| PC.1.7.8 Bootstrap accessibility | Mid | The embedded nature of AI features (Notion AI, Copilot inline suggestions) provides relatively low barriers to first attempts — you can start with one click. But the gap between first attempt and effective use is large. |

**Relevance:** High. The current state of AI tool adoption is heavily scaffold-dependent. This is appropriate for Level 2 but becomes the progression blocker for Level 3 unless scaffolding is deliberately faded.

---

### Opportunity (PO — Physical Opportunity)

#### PO-1-WorkSys: Work-System Configuration

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.1.1 Work-system coherence | Mid | Many organizations have added AI tools on top of existing tool stacks without redesigning the work system. AI is an add-on, not integrated into the workflow architecture. Notion AI exists alongside the old "start from blank page" habit. |
| PO.1.2 Tool-task fit | Mid | Embedded AI features (Copilot, Notion AI) are generally well-fitted to their immediate task contexts but may not cover the full range of tasks employees need help with. Gaps between tools create friction — AI summarizes in one tool but doesn't flow into the task management tool. |
| PO.1.5 Feedback-loop strength | Low | Users get no systematic feedback on whether AI-assisted output was better, faster, or more effective than manual work. Learning about AI effectiveness happens by feel, not by data. |

**Relevance:** Mid-High. The work system supports basic AI use (tools are available and somewhat integrated) but doesn't actively facilitate it or provide feedback.

#### PO-2-Resource: Resource and Capacity

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.2.1 Time availability | Low-Mid | The core contradiction: people who most need AI time savings are too busy to learn AI tools. The "learning dip" — the period where AI slows you down before it speeds you up — competes with delivery pressure. |
| PO.2.7 Activation overhead | Mid | For well-designed embedded AI (inline suggestions, one-click summaries), activation overhead is low. For more powerful features (custom prompts, AI-assisted data extraction), activation overhead is higher — you need to learn the feature, craft the prompt, review the output. |

**Relevance:** High. Time scarcity is the single most common reason employees cite for not adopting AI tools. The irony — "too busy to save time" — is a classic PO-2 pattern.

#### PO-3-Workflow: Workflow Architecture

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.3.7 Activation energy | Mid-High | Starting to use AI for a new task type requires figuring out which tool to use, how to prompt it, and whether the output is trustworthy — all before any time savings materialize. For simple tasks (summarize this, fix this grammar), activation energy is low. For complex tasks (synthesize these meeting notes into action items across three projects), it's high. |

**Relevance:** Mid. Activation energy varies dramatically by use case, which is why adoption tends to cluster around low-activation use cases (grammar, summarization) and stall on higher-value applications.

#### PO-4-Visibility: Information and State Visibility

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.4.1 Signal surfacing | Low | Productivity gains from AI use are invisible to others. When someone saves 2 hours using AI meeting notes, their manager and peers don't see the gain — they just see the output. |
| PO.4.8 Cost visibility | Low | The cost of *not* using AI (manual transcription, writing from scratch, re-searching for information) is invisible. People have normalized these costs. |
| PO.4.9 Friction visibility | Low | Friction in AI-assisted workflows is also invisible — time spent crafting prompts, reviewing AI output, fixing errors. This makes it hard to improve the process. |

**Relevance:** High. Invisible gains can't compound. If teams can't see each other's productivity improvements, there's no mechanism for social learning, norm formation, or organizational investment in scaling what works.

#### PO-5-Tooling: Tooling and Interface Affordances

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.5.1 Affordance clarity | Mid | Well-designed AI features (Copilot's inline suggestions, Notion AI's context menus) have decent affordance clarity — it's obvious you can click to get AI help. But more powerful features are often hidden in menus or require knowledge of keyboard shortcuts. |
| PO.5.6 Learnability in context | Mid | AI features within familiar tools (Notion, Google Docs) benefit from existing tool familiarity. But AI-specific interaction patterns (prompting, iterating, providing context) are genuinely new and have their own learning curve. |
| PO.5.7 Automation fit | Mid | Current AI features are largely "request-response" rather than proactive. The automation does what you ask but doesn't proactively suggest when AI could help. This puts the burden on the user to recognize AI opportunities. |

**Relevance:** Mid. Tooling is adequate for Level 2 but not optimized for it. The biggest gap is PO.5.7 — tools don't proactively nudge users toward AI use.

---

### Opportunity (SO — Social Opportunity)

#### SO-1-Norms: Norms and Normative Climate

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.1.1 Descriptive norm | Low-Mid | AI tool use is visible among early adopters but not yet the majority behavior. Most employees see a few enthusiasts using AI prominently but don't perceive it as "what everyone does." |
| SO.1.2 Injunctive norm | Mid | Most organizations officially encourage AI use, but the injunctive norm is mixed — some managers actively promote it, others are indifferent, a few subtly discourage it by questioning the quality of AI-assisted work. |
| SO.1.3 Norm clarity | Low | Mixed signals abound. "We encourage AI use" coexists with "make sure everything is reviewed" and "don't use AI for client-facing work" — without clear guidance on where the boundaries are. |
| SO.1.4 Norm consistency | Low | Leadership says "embrace AI" while middle management continues to evaluate work by traditional standards. The gap between stated policy and operational norms creates confusion. |

**Relevance:** High. The normative environment is the single biggest social barrier. Until AI-assisted work becomes the default expectation rather than an optional extra, adoption will remain patchy and inconsistent.

#### SO-2-Roles: Roles and Authority

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.2.1 Ownership clarity | Low | Who owns AI tool rollout? IT provisions licenses. L&D runs training. Individual managers decide team norms. Nobody owns the integration of AI into actual work practices. |
| SO.2.2 Decision-right clarity | Low | Can a team lead mandate AI tool use? Can an IC decide to use AI for a client deliverable? Decision rights around AI use are ambiguous, leading to conservative defaults. |

**Relevance:** High for Behavior B. The absence of clear ownership is the primary structural barrier preventing individual gains from compounding into organizational capability.

#### SO-4-Incentives: Incentives and Reinforcement

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.4.1 Reward alignment | Misaligned | Most performance evaluation systems reward output quality and delivery speed but don't recognize AI adoption or efficiency gains. An employee who uses AI to save 5 hours/week and spends that time on higher-value work is evaluated the same as one who brute-forced the same output. |
| SO.4.5 Recognition visibility | Low | There's no mechanism to recognize or celebrate AI-driven productivity gains. "I saved 3 hours this week using AI meeting notes" has no organizational visibility. |
| SO.4.7 Penalty risk | Mid | Some employees fear that demonstrating AI-driven efficiency will lead to headcount reduction ("if AI can do half my job, why do they need me?") or increased workload ("you saved 5 hours, here's 5 hours more work"). |

**Relevance:** High. The incentive structure is neutral-to-negative for AI adoption. The absence of reward for adoption combined with implicit penalty risk creates a rational disincentive for visible AI use.

#### SO-5-Legitimacy: Legitimacy and Identity Safety

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.5.1 Legitimacy signal | Mid | AI-assisted work is broadly seen as acceptable but not yet fully legitimate. In some professional contexts (legal, medical, creative), AI-assisted output is viewed with suspicion. |
| SO.5.3 Identity safety | Low-Mid | For some roles, using AI feels like admitting you can't do your job. Writers fear that using AI undermines their craft. Analysts worry that AI summarization devalues their synthesis skills. |
| SO.5.5 Professional congruence | Variable | Varies dramatically by role: software engineers see Copilot as professionally congruent ("better tools make better engineers"); copywriters see AI writing as professionally threatening ("if AI writes the first draft, what am I for?"). |

**Relevance:** High. Legitimacy and identity safety are the hidden barriers that determine whether technically capable employees will *choose* to adopt AI tools. This is where motivation and social opportunity intersect.

#### SO-7-Governance: Governance Viability

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.7.1 Local autonomy fit | Mid | Teams generally have autonomy to use AI tools but lack guidance on what's appropriate. The result is inconsistent adoption driven by individual manager preferences. |
| SO.7.5 Policy-operational coherence | Low | Formal AI policies (where they exist) often lag operational reality. Policies written for ChatGPT don't address embedded AI features. "Don't put proprietary data in AI" conflicts with "use Notion AI on our internal docs." |
| SO.7.8 Cross-group consistency | Low | Massive variation across teams. Some teams are all-in on AI; adjacent teams haven't started. This inconsistency blocks progression to Level 3 because team-level workflows require cross-team consistency. |

**Relevance:** High for Behavior B. Governance gaps mean that even successful individual adoption can't scale into organizational practice.

---

### Motivation (RM — Reflective Motivation)

#### RM-1.1-SDT: Self-Determination Theory

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.1.1 Regulation quality | Mixed | Early adopters are autonomously motivated — they find AI genuinely useful and interesting. The middle majority is externally motivated — they'll use AI if told to but won't seek it out. The trailing group is amotivated — they see no reason to change working methods that already work. |
| RM.1.1.3 Autonomy support | Mid | Most organizations provide tools and encourage use without mandating specific behaviors — reasonably autonomy-supportive. But the flip side is that without clear expectations, the optional nature of AI adoption means it gets displaced by non-optional work. |
| RM.1.1.6 Internalization | Low-Mid | Few employees have internalized AI use as part of their professional identity. For most, it's still an "extra thing" rather than "how I work." |

**Relevance:** High. The motivational profile matters for intervention design — what works for autonomously motivated early adopters (more tools, fewer restrictions) backfires for controlled-motivation middle adopters (who need structure and social proof).

#### RM-1.2-Efficacy: Self-Efficacy

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.2.1 Efficacy belief | Bimodal | Technical employees and early adopters report high self-efficacy ("I can figure out any AI tool"). Many non-technical employees report low self-efficacy ("I'm not a tech person, AI isn't for me"). This split correlates with adoption. |
| RM.1.2.3 Recovery after setbacks | Low | When AI produces a bad output — hallucinated facts, wrong tone, useless summary — many users give up on that use case entirely rather than iterating. One bad experience poisons the well. |
| RM.1.2.4 Task specificity | Low | Even users who feel confident with one AI tool (e.g., Copilot for code) may feel uncertain about others (e.g., Notion AI for strategic writing). Confidence doesn't transfer well across AI tools and use cases. |

**Relevance:** High. Self-efficacy is the strongest individual-level predictor of AI tool adoption. Low efficacy users avoid the tools; fragile efficacy users abandon them after setbacks.

#### RM-1.3-EVC: Expectancy-Value-Cost

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.3.1 Expectancy of success | Mid | Most employees believe AI *could* help but are uncertain whether it will help *them* with *their specific* work. Generic "AI saves time" messaging doesn't map to their experience. |
| RM.1.3.4 Utility value | Mid-High | The practical benefit proposition is strong — saving time on meeting notes, first drafts, and search is obviously useful. This is a tailwind for Level 2. |
| RM.1.3.5 Effort cost | Mid-High | The learning investment is real. Learning to prompt effectively, building new habits, adjusting quality review processes — all require upfront effort before payoff materializes. |
| RM.1.3.8 Present-vs-future weighting | High (present dominates) | The costs of AI adoption (learning time, workflow disruption) are immediate and certain. The benefits (time savings, quality improvement) are future and uncertain. Present costs dominate the calculus for many employees. |

**Relevance:** High. The effort-cost-to-perceived-benefit ratio is the pragmatic barrier. When someone is deciding whether to use AI for a specific task, they're running an implicit EVC calculation: "Will this save me time net of learning cost, right now?" If the answer isn't clearly yes, they default to their existing method.

#### RM-1.4-Identity: Identity-Based Motivation

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.4.1 Identity congruence | Variable | For many knowledge workers, "using AI tools" doesn't yet feel like part of their professional identity. Engineers are closer ("tools are my craft"); writers, analysts, and strategists are further ("my thinking is my value"). |
| RM.1.4.3 Identity conflict | Mid | Some employees experience identity conflict: "I value craftsmanship" conflicts with "I use AI to produce faster output." The fear is that AI adoption signals a downgrade from "thinker" to "editor." |
| RM.1.4.7 Reputation risk | Mid | Visible AI use carries reputation risk in some contexts: "Did she actually write that, or did AI?" undermines perceived contribution. |

**Relevance:** High. Identity is the motivational dimension most often underestimated in AI adoption programs. It explains why technically capable people with access to good tools still don't adopt — the behavior doesn't fit who they believe they are.

#### RM-1.5-Intentions: Goal and Implementation Intentions

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.5.1 Intention strength | Mid | Many employees express intent to use AI more ("I should really start using Copilot") but haven't converted that into specific plans. |
| RM.1.5.3 Plan specificity | Low | Very few employees have specific if-then plans: "When I start writing a document, I will first prompt Notion AI for a draft." Intentions are vague ("I'll try using AI more") rather than specific. |
| RM.1.5.4 Cue linkage | Low | AI use is not linked to existing workflow triggers. There's no "when I open a new doc, I prompt AI" cue-response pattern in place. |

**Relevance:** High. This is the intention-action gap. Many employees intend to use AI more but lack the implementation intentions that bridge intention to behavior. This makes the behavior vulnerable to displacement by any competing demand.

---

### Motivation (AM — Automatic Motivation)

#### AM-2.1-Habit: Habit Formation

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.1.1 Automaticity | Low | For most employees, AI tool use is still deliberate and effortful — it requires conscious decision-making rather than running on autopilot. |
| AM.2.1.3 Repetition history | Low | Most employees haven't accumulated enough consistent repetitions in stable contexts to build AI-use habits. Usage is sporadic. |
| AM.2.1.7 Competing habit strength | High | Existing non-AI workflows are deeply habitual. "Open blank doc, start typing" is automatic. "Open doc, prompt AI, review output, edit" is effortful. The old habit wins under cognitive load or time pressure. |

**Relevance:** High. This is the core automatic motivation barrier. Existing work habits are strong and automated; AI-assisted alternatives are weak and deliberate. Under any pressure, people revert to what's automatic.

#### AM-2.2-Reward: Reinforcement and Wanting

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.2.1 Reward immediacy | Variable | For simple use cases (grammar check, quick summary), AI reward is immediate — visible time savings in minutes. For complex use cases (strategic writing, data analysis), reward is delayed — you invest time prompting and editing before payoff. |
| AM.2.2.2 Reward magnitude | Mid | When AI works well, the reward is compelling — a 20-minute meeting summary in 30 seconds is a powerful experience. But reward magnitude varies wildly by use case and prompt quality, creating an unreliable reinforcement schedule. |

**Relevance:** Mid. The reward profile of AI use is actually favorable for habit formation — immediate, tangible time savings. The problem is the variability: inconsistent reward undermines the reinforcement loop that builds habits.

#### AM-2.3-Affect: Affect and Emotion

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.3.1 Valence | Mixed | Some employees find AI use genuinely exciting and fun ("it's like having a superpower"). Others find it anxiety-inducing ("what if it makes mistakes I don't catch?") or threatening ("what does this mean for my job?"). |
| AM.2.3.3 Anticipatory affect | Mid-negative | A significant subset of employees experience anticipatory anxiety about AI: concern about job displacement, concern about becoming dependent on tools, concern about AI making errors in their name. |
| AM.2.3.5 Social-emotional intensity | Mid | The emotional charge around AI is higher than around most workplace tools. It touches on professional identity, job security, and competence — emotionally loaded topics. |

**Relevance:** Mid-High. The affective landscape of AI adoption is more emotionally complex than typical tool adoption. Anxiety about dependency and job displacement creates an emotional headwind that rational "AI saves time" messaging doesn't address.

---

## Step 3: Practitioner Worksheet

### 1. COM-B Priority Ranking

| Rank | Branch | Rationale |
|------|--------|-----------|
| 1 | **Opportunity (O)** | The dominant barrier is structural and social, not individual. Physical opportunity gaps (PO.4 visibility, PO.2 time scarcity, PO.3 activation energy) prevent behavior from embedding in workflows. Social opportunity gaps (SO.1 norms, SO.2 role clarity, SO.4 incentive alignment, SO.7 governance) prevent individual gains from compounding. Even capable, motivated employees face an environment that doesn't actively support or reinforce AI use. |
| 2 | **Capability (C)** | Capability gaps are real and widespread — especially PC.1.1 procedural fluency, PC.1.2 mental models, PC.1.3 judgment, and PC.1.5 calibration. However, many employees have enough capability to start (PC.1.7 scaffold accessibility is mid) and tools are designed to be learnable. Capability is a barrier to *effective* use more than to *initial* adoption. |
| 3 | **Motivation (M)** | Motivation is the most complex but least primary barrier. RM.1.3 EVC is favorable (the value proposition is clear), but RM.1.4 identity and AM.2.1 habit compete against adoption. Motivation issues are largely *downstream* of opportunity problems: fix the incentive structure, make gains visible, normalize AI use, and much of the motivation barrier dissolves. The exception is AM.2.1 competing habit strength, which is an independent barrier requiring direct intervention. |

### 2. Per-Lens Synthesis

#### Capability (PC / PHC)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PC-1.1-Knowledge | PC.1.1.1 declarative: low-mid; PC.1.1.2 procedural fluency: low; PC.1.1.3 sequence clarity: low; PC.1.1.6 exception handling: low | Declarative knowledge is partial but procedural fluency is the real gap. Training (TR) is needed over education (ED). When PO.2.1 (time) is scarce, embed knowledge at point of action via EN rather than extended training programs. | BCT.4.1 Instruction on how to perform a behavior; BCT.8.1 Behavioral practice/rehearsal; BCT.8.7 Graded tasks; BCT.7.1 Prompts/cues; BCT.12.5 Adding objects to the environment |
| PC-1.2-Models | PC.1.2.1 model accuracy: low-mid; PC.1.2.2 causal understanding: low; PC.1.2.7 updateability: mid | Wrong mental models drive both over-trust and under-trust. BCT.4.4 behavioral experiments are more effective than lectures because users need to experience model errors themselves. | BCT.4.4 Behavioral experiments; BCT.4.3 Re-attribution; BCT.2.7 Feedback on outcomes of behavior |
| PC-1.3-Judgment | PC.1.3.3 heuristic quality: low; PC.1.3.5 rule dependence: mid-high; PC.1.3.7 tradeoff handling: low | Judgment develops through practice with feedback, not instruction. TR via realistic scenarios with BCT.2.2 feedback. Rigid rule-following (PC.1.3.5) is normal for early adopters — don't fight it, provide good rules that can later be relaxed. | BCT.8.1 Behavioral practice/rehearsal; BCT.2.2 Feedback on behaviour; BCT.1.2 Problem solving |
| PC-1.5-Meta | PC.1.5.1 calibration: bimodal; PC.1.5.3 error detection: low; PC.1.5.6 help-seeking: low-mid | Calibration is the gateway skill. Over-confident users need BCT.2.2 feedback to surface accuracy gaps. Under-confident users need BCT.15.1 persuasion about capability. Both need BCT.2.3 self-monitoring to build accurate self-assessment. | BCT.2.2 Feedback on behaviour; BCT.2.3 Self-monitoring of behaviour; BCT.15.1 Verbal persuasion about capability |
| PC-1.6-Shared | PC.1.6.1 shared language: low; PC.1.6.4 common ground: low; PC.1.6.8 behavior specification: low | Critical for progression (Behavior B). Individual adoption can proceed without shared representations, but compounding gains cannot. ED to establish shared definitions, EN via shared glossaries and reference artifacts. | BCT.4.1 Instruction; BCT.12.5 Adding objects to the environment; BCT.1.1 Goal setting (behavior); BCT.6.1 Demonstration |
| PC-1.7-Scaffold | PC.1.7.1 independence: low; PC.1.7.3 prompt dependence: high; PC.1.7.8 bootstrap accessibility: mid | Current state is scaffold-dependent, which is appropriate for Level 2. Design scaffolds deliberately (prompt templates, guided workflows, inline help) rather than treating scaffold-dependence as a failure. Plan for fading via BCT.7.3 as capability builds. | BCT.7.1 Prompts/cues; BCT.12.5 Adding objects; BCT.8.7 Graded tasks; BCT.3.2 Social support (practical) |

**Narrative synthesis:** The capability picture reveals a workforce that is aware of AI tools but lacks the procedural fluency, mental models, and calibrated judgment to use them effectively. The critical insight is that capability gaps are better addressed through scaffolded practice in context (EN + TR) than through classroom training (ED alone). Extended training programs face a PO.2 resource constraint — people don't have time for them. The highest-leverage capability intervention is embedding learning at point of action: inline help, prompt templates, and guided first-use experiences that build procedural fluency through doing rather than through instruction. Exception handling (PC.1.1.6) and judgment (PC.1.3) develop through repeated use with feedback — they cannot be taught in advance. This means the capability strategy must be interleaved with opportunity interventions that create space for practice.

What *not* to try: Comprehensive upfront training programs, certification requirements, or mandatory "AI literacy" courses. These fail because (a) PO.2.1 time scarcity makes attendance competitive, (b) PC.1.7 scaffold dependency means knowledge doesn't transfer without contextual support, and (c) SO.1.4 norm inconsistency means trained employees return to teams that don't support the behavior.

#### Opportunity (PO / SO)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PO-1-WorkSys | PO.1.1 coherence: mid; PO.1.2 tool-task fit: mid; PO.1.5 feedback: low | AI is added atop existing systems rather than integrated. Feedback loops are weak — users don't learn whether AI-assisted work was better. ER to build feedback mechanisms; EN to bridge tool gaps. | BCT.12.1 Restructuring physical environment; BCT.2.7 Feedback on outcomes; BCT.12.5 Adding objects |
| PO-2-Resource | PO.2.1 time: low-mid; PO.2.7 activation overhead: mid | Time scarcity is the primary physical barrier. Don't add learning burden — reduce it. ER to embed AI into existing flows. EN via BCT.1.4 action planning for time protection. | BCT.12.1 Restructuring physical environment; BCT.1.4 Action planning; BCT.7.1 Prompts/cues |
| PO-4-Visibility | PO.4.1 signal surfacing: low; PO.4.8 cost visibility: low; PO.4.9 friction visibility: low | Invisible gains can't spread. Make productivity improvements visible via BCT.2.7 feedback on outcomes. Make the cost of *not* using AI visible via BCT.5.3. | BCT.2.7 Feedback on outcomes; BCT.5.3 Information about social/environmental consequences; BCT.12.5 Adding objects (dashboards) |
| PO-5-Tooling | PO.5.1 affordance: mid; PO.5.6 learnability: mid; PO.5.7 automation fit: mid | Tools are adequate but not optimized. Biggest gap is PO.5.7 — tools don't proactively suggest AI use. ER to configure proactive nudges where possible. | BCT.7.1 Prompts/cues; BCT.12.1 Restructuring physical environment |
| SO-1-Norms | SO.1.1 descriptive: low-mid; SO.1.2 injunctive: mid; SO.1.3 clarity: low; SO.1.4 consistency: low | Classic "approved but uncommon" pattern. MO via demonstration is the priority — make AI use visible. Avoid BCT.6.2 social comparison (can backfire by highlighting low adoption). Address SO.1.4 norm consistency between leadership messaging and operational reality. | BCT.6.1 Demonstration of behavior; BCT.6.3 Information about others' approval; BCT.12.2 Restructuring social environment |
| SO-2-Roles | SO.2.1 ownership: low; SO.2.2 decision-rights: low | Nobody owns AI adoption as a practice. ER to assign explicit ownership. BCT.1.8 behavioral contract to formalize responsibility for AI integration at team level. | BCT.12.2 Restructuring social environment; BCT.1.8 Behavioral contract; BCT.4.1 Instruction |
| SO-4-Incentives | SO.4.1 reward alignment: misaligned; SO.4.5 recognition: low; SO.4.7 penalty risk: mid | The incentive structure is neutral-to-hostile. INC via BCT.10.4 social reward for AI-driven productivity gains. ER to realign performance metrics. Address SO.4.7 penalty risk directly — employees need explicit assurance that efficiency gains won't lead to headcount cuts or workload inflation. | BCT.10.4 Social reward; BCT.10.5 Social incentive; BCT.12.2 Restructuring social environment; BCT.5.3 Information about consequences |
| SO-5-Legitimacy | SO.5.1 legitimacy: mid; SO.5.3 identity safety: low-mid; SO.5.5 professional congruence: variable | Legitimacy is the hidden gatekeeper. PE via BCT.13.2 framing to make AI use identity-safe. MO via BCT.6.1 demonstration from respected, identity-congruent figures — the senior writer who uses AI, the experienced analyst who relies on AI summaries. | BCT.13.2 Framing/reframing; BCT.6.1 Demonstration; BCT.9.1 Credible source |
| SO-7-Governance | SO.7.1 local autonomy: mid; SO.7.5 policy-ops coherence: low; SO.7.8 cross-group consistency: low | Governance gaps block progression. ER to create coherent, practical AI usage guidelines that resolve the tension between "use AI" and "don't put data in AI." EN via cross-group sharing to reduce practice variation. | BCT.12.2 Restructuring social environment; BCT.4.4 Behavioral experiments; BCT.6.1 Demonstration |

**Narrative synthesis:** Opportunity is the primary barrier cluster and contains both the biggest blockers and the highest-leverage intervention points. The physical opportunity picture is one of *adequacy without optimization*: tools exist, time is scarce, feedback is absent. The social opportunity picture is more concerning: norms are unclear, ownership is absent, incentives are misaligned, and governance lags reality.

The highest-leverage opportunity intervention is making productivity gains visible (PO.4) while simultaneously normalizing AI use (SO.1) and protecting adopters from penalty risk (SO.4.7). These three create a reinforcing loop: visible gains → social proof → norm shift → more adoption → more visible gains.

What *not* to try: Top-down mandates without infrastructure (creates compliance theater and triggers SO.5 legitimacy backlash), adding more tools without fixing the work system (PO.1 fragmentation worsens), or creating AI policies that restrict without enabling (RE without EN generates resentment).

#### Motivation (RM / AM)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| RM-1.1-SDT | RM.1.1.1 regulation: mixed; RM.1.1.3 autonomy support: mid; RM.1.1.6 internalization: low-mid | Autonomously motivated early adopters are already on board. The middle majority needs structure and social proof more than autonomy. Don't add more INC/COE — these deepen controlled regulation. Use PE via BCT.13.2 framing to connect AI to personal professional values. | BCT.13.2 Framing/reframing; BCT.1.1 Goal setting (behavior); BCT.3.1 Social support |
| RM-1.2-Efficacy | RM.1.2.1 efficacy: bimodal; RM.1.2.3 recovery after setbacks: low; RM.1.2.4 task specificity: low | Efficacy is the individual-level swing factor. BCT.8.7 graded tasks to ensure early wins. BCT.6.1 demonstration from relatable peers (not tech experts) to build vicarious efficacy. BCT.15.3 focus on past success to rebuild confidence after bad AI experiences. | BCT.8.7 Graded tasks; BCT.6.1 Demonstration; BCT.15.1 Verbal persuasion about capability; BCT.15.3 Focus on past success |
| RM-1.3-EVC | RM.1.3.1 expectancy: mid; RM.1.3.4 utility value: mid-high; RM.1.3.5 effort cost: mid-high; RM.1.3.8 temporal weighting: present-dominated | Value is recognized but effort cost and temporal discounting suppress action. Reduce cost via PO-level friction reduction (not motivation-level persuasion). BCT.5.2 salience of consequences to make future benefits vivid. BCT.10.4 social reward to bridge temporal gap with proximal reinforcement. | BCT.5.2 Salience of consequences; BCT.10.4 Social reward; BCT.9.3 Comparative imagining of future outcomes |
| RM-1.4-Identity | RM.1.4.1 identity congruence: variable; RM.1.4.3 identity conflict: mid; RM.1.4.7 reputation risk: mid | Identity is the hidden veto. PE via BCT.13.2 reframing to make AI use compatible with valued professional identities. "AI makes a great writer better" rather than "AI replaces writing." MO via BCT.6.1 from identity-congruent models. | BCT.13.2 Framing/reframing; BCT.13.5 Identity associated with changed behavior; BCT.6.1 Demonstration |
| RM-1.5-Intentions | RM.1.5.1 intention: mid; RM.1.5.3 plan specificity: low; RM.1.5.4 cue linkage: low | Classic intention-action gap. Bridge it with BCT.1.4 action planning for specific if-then plans. BCT.7.1 prompts/cues to externalize initiation. This connects directly to AM-2.1 habit formation. | BCT.1.4 Action planning; BCT.7.1 Prompts/cues; BCT.8.3 Habit formation |
| AM-2.1-Habit | AM.2.1.1 automaticity: low; AM.2.1.3 repetition: low; AM.2.1.7 competing habit strength: high | The core AM barrier. Existing workflows are automatic; AI-assisted alternatives require deliberate effort. ER to disrupt existing cues where possible (BCT.12.1). Form new habits by anchoring AI use to existing workflow triggers (BCT.8.3). BCT.8.2 behavior substitution for specific task types. | BCT.8.3 Habit formation; BCT.8.2 Behavior substitution; BCT.12.1 Restructuring physical environment; BCT.7.1 Prompts/cues |
| AM-2.2-Reward | AM.2.2.1 immediacy: variable; AM.2.2.2 magnitude: mid | Reward variability undermines habit formation. Steer toward use cases with immediate, consistent reward (meeting summaries, grammar/editing, search) before complex, variable-reward use cases (strategic writing, analysis). | BCT.10.4 Social reward; BCT.14.4 Reward approximation |
| AM-2.3-Affect | AM.2.3.1 valence: mixed; AM.2.3.3 anticipatory affect: mid-negative; AM.2.3.5 social-emotional intensity: mid | Anxiety about job displacement and dependency cannot be addressed by rational argument alone. BCT.11.2 reduce negative emotions through explicit organizational commitments about job security. BCT.13.2 reframing AI as "augmentation not replacement." | BCT.11.2 Reduce negative emotions; BCT.13.2 Framing/reframing; BCT.3.3 Social support (emotional) |

**Narrative synthesis:** The motivation picture is more favorable than it first appears. The value proposition is clear (RM.1.3.4 utility value is mid-high), and the affective barriers — while real — are addressable through framing and organizational assurance rather than requiring deep individual-level change. The two motivation dimensions that require direct intervention are: (1) AM.2.1 competing habit strength, which requires environmental restructuring and deliberate habit-formation strategies, and (2) RM.1.4 identity, which requires careful framing and identity-congruent modeling to make AI use feel professionally enhancing rather than professionally threatening.

What *not* to try: Coercion (COE) through mandates — this deepens controlled regulation and triggers identity backlash. Heavy external incentivisation (INC via material rewards for AI use) — this crowds out intrinsic motivation and creates compliance without internalization. Rational persuasion alone ("AI saves time, here are the statistics") — this doesn't reach the identity and habit layers where the real resistance lives.

### 3. Cross-Lens Interactions

**Tensions:**
- **C ↔ SO:** Capability can be built through practice, but SO.1 (norms) and SO.5 (legitimacy) determine whether people feel safe practicing. Building PC.1.1 procedural fluency requires repeated use, but if SO.1.1 (descriptive norm) says "most people don't use AI" and SO.5.3 (identity safety) says "AI use threatens my professional identity," people won't accumulate the practice needed to build capability.
- **RM ↔ PO:** RM.1.3.4 (utility value) is mid-high — people see the value. But PO.2.1 (time availability) is low — they don't have time to realize it. The motivation exists but the opportunity doesn't. Persuasion-based interventions (PE) will fail if PO barriers remain.
- **SO.4 ↔ AM.2.1:** The incentive structure (SO.4.1 misaligned) reinforces existing habits (AM.2.1.7 high competing habit strength). If performance evaluation rewards output without recognizing efficiency, there's no incentive to invest in the habit-formation period where AI use is slower before it becomes faster.

**Reinforcements:**
- **PO.4 → SO.1 → RM.1.2:** Making gains visible (PO.4) creates social proof (SO.1 norm shift), which builds efficacy in observers (RM.1.2 "if they can do it, I can too"). This is a high-leverage reinforcing loop.
- **PC.1.7 + PO.5 → AM.2.1:** Good scaffolding (PC.1.7) embedded in well-designed tools (PO.5) lowers activation energy, which accelerates habit formation (AM.2.1). Scaffold design is a capability intervention that operates through the opportunity and habit channels.
- **SO.5 → RM.1.4 → RM.1.5:** When AI use becomes socially legitimate (SO.5), it becomes identity-safe (RM.1.4), which strengthens intention (RM.1.5), which enables plan specificity and habit formation.

**Prerequisites:**
- **SO.4 (incentive alignment) before RM-focused interventions:** Trying to build motivation while the incentive structure is neutral-to-hostile is swimming upstream. Address SO.4.7 (penalty risk) and SO.4.1 (reward alignment) before investing in PE or INC.
- **SO.7 (governance) before SO.1 (norms):** Norm campaigns without coherent governance create confusion. Resolve the "use AI" vs. "don't put data in AI" tension (SO.7.5) before asking people to adopt.
- **PC.1.7 (scaffolding) before PC.1.1 (knowledge):** Don't train people in a vacuum. Provide scaffolds first, then build knowledge through supported practice.

**Highest leverage (top 3):**
1. **Make gains visible + normalize AI use (PO.4 + SO.1):** This single intervention cluster activates the most reinforcing loops — visible gains create social proof, social proof shifts norms, shifted norms make AI use identity-safe, identity safety strengthens intention.
2. **Fix the incentive structure (SO.4):** Remove the penalty risk (SO.4.7) and create recognition for AI-driven efficiency (SO.4.5). This is a prerequisite for most other interventions to stick.
3. **Embed scaffolded practice in workflows (PC.1.7 + PO.5 + AM.2.1):** Design AI tool experiences that scaffold first use, anchor to existing workflow triggers, and build habit through low-activation, high-reward use cases. This attacks capability, opportunity, and habit simultaneously.

### 4. BCW Function Ranking

| Rank | Function | Rationale | Top 3 BCTs |
|------|----------|-----------|------------|
| 1 | **EN — Enablement** | Enablement is the foundation because the primary barriers are structural (PO.2 time scarcity, PO.4 invisible gains, PC.1.7 scaffold dependence, RM.1.5 intention-action gap). EN removes barriers beyond education and training — making the behavior possible and easier. It bridges the gap between "available tools" and "usable tools in context." | BCT.1.4 Action planning (bridge intention-action gap); BCT.7.1 Prompts/cues (trigger AI use at natural workflow moments); BCT.3.2 Social support, practical (peer pairing for supported practice) |
| 2 | **ER — Environmental Restructuring** | ER addresses the opportunity layer — the physical and social environment that currently defaults to non-AI workflows. Restructuring makes AI the path of least resistance rather than an add-on. Addresses PO.1 work-system coherence, SO.1 norms, SO.2 role clarity, SO.4 incentive alignment, and AM.2.1 competing habits via cue disruption. | BCT.12.2 Restructuring social environment (assign ownership, create AI champion roles, realign incentives); BCT.12.1 Restructuring physical environment (configure tools for AI-first defaults, embed AI in workflow templates); BCT.12.5 Adding objects (visibility dashboards, prompt libraries, shared success stories) |
| 3 | **MO — Modelling** | Modeling directly addresses the SO.1 normative gap (behavior appears uncommon), SO.5 legitimacy gap (is AI-assisted work "real" work?), RM.1.2 efficacy (vicarious experience), and RM.1.4 identity (seeing identity-congruent peers use AI). Modeling is especially effective when models are relatable peers, not technology experts. | BCT.6.1 Demonstration of the behavior (visible AI use by respected, non-technical peers); BCT.6.3 Information about others' approval (sharing that teams find AI helpful); BCT.9.1 Credible source (senior leaders visibly using AI in their own work) |
| 4 | **TR — Training** | Training addresses PC.1.1 procedural fluency, PC.1.3 judgment, and PC.1.5 calibration. Ranks fourth (not first) because training without EN and ER infrastructure doesn't stick — trained employees return to environments that don't support the behavior. Training should be embedded, scaffolded, and practice-based, not classroom-style. | BCT.8.7 Graded tasks (start with easy, high-reward use cases before complex ones); BCT.8.1 Behavioral practice/rehearsal (hands-on practice with own work, not artificial exercises); BCT.2.2 Feedback on behaviour (coaching on prompt quality and output review) |
| 5 | **PE — Persuasion** | Persuasion addresses RM.1.4 identity, RM.1.3 EVC, AM.2.3 affect, and SO.5 legitimacy. Ranks fifth because much of what PE addresses (identity safety, anxiety, perceived cost) is better resolved through environmental changes (ER, EN) and social proof (MO) than through direct argument. PE is most effective for reframing AI use as professionally enhancing and reducing job-displacement anxiety. | BCT.13.2 Framing/reframing ("AI augments your expertise, not replaces it"); BCT.5.3 Information about social/environmental consequences (what teams gain from AI adoption); BCT.11.2 Reduce negative emotions (explicit job-security assurances, anxiety normalization) |

**Contraindicated:**
- **COE — Coercion:** Mandating AI use without infrastructure creates compliance theater and triggers identity backlash (RM.1.4). It deepens controlled regulation (RM.1.1.1) and can increase anxiety (AM.2.3). The evidence clearly shows that when SO.5.3 identity safety is already fragile, coercive approaches damage rather than build adoption.
- **RE — Restriction:** Restricting non-AI workflows (e.g., removing access to manual processes) is premature at Level 2. AI tools are not yet reliable enough to justify removing fallbacks, and restriction without capability creates helplessness (AM.2.4).

### 5. Intervention Implications

**EN (Enablement):** Design "AI-ready" workflow templates in existing tools — Notion templates with AI prompts pre-loaded, meeting agenda templates that auto-trigger AI summarization, document templates that prompt "ask AI for a first draft." Pair new AI users with experienced peers for supported first-use experiences. Create explicit "AI time" blocks in team calendars for learning and experimentation. Build specific if-then plans: "When I get meeting notes, I will run AI summary before reading. When I start a new document, I will prompt AI for a structure."

**ER (Environmental Restructuring):** Assign an explicit "AI Integration Lead" role per team — someone who owns the team's AI adoption and workflow integration. Configure tool defaults to surface AI options (e.g., Notion documents default to showing AI assist button). Create a shared team dashboard showing AI-driven time savings. Realign performance reviews to recognize efficiency gains, not just output volume. Create explicit organizational assurances about AI and job security, signed by leadership.

**MO (Modelling):** Launch an internal "AI at Work" series where respected non-technical employees demonstrate their actual AI workflows — not polished demos but messy, real usage including failures and iterations. Have senior leaders visibly use AI in their own work and share results (including imperfect ones). Create cross-team "show and tell" sessions where teams demonstrate AI-assisted workflows to peers. Prioritize models who represent the identity profiles of the target audience (the senior copywriter using AI, the operations manager using AI meeting notes, the analyst using AI data extraction).

**TR (Training):** Structure training as guided, graded task sequences using employees' actual work — not artificial exercises. Start with highest-reward, lowest-complexity use cases: meeting summarization, grammar and tone editing, enterprise search. Progress to mid-complexity: first drafts, data extraction, structured summarization. Include feedback cycles where trainers review how employees are prompting and using AI output, not just whether they're using it.

**PE (Persuasion):** Frame AI adoption as "professional growth" not "efficiency mandate." Share the narrative: "The best professionals in every field are learning to work with AI — not because they can't do the work, but because AI amplifies what they already do well." Address job-displacement anxiety directly with organizational commitments: "AI savings will be reinvested in more interesting work, not fewer people." Help specific roles reframe their identity relationship with AI: writers become "AI-augmented editors," analysts become "AI-assisted strategists."

---

## Step 4: BCW and BCT Reasoning

### Dimensional Findings → BCW Functions

```text
dimensions = PO.4.1 low, PO.2.1 low-mid, SO.1.1 low-mid, SO.1.4 low, SO.4.1 misaligned, SO.4.7 mid, SO.2.1 low, SO.7.5 low, PC.1.1.2 low, PC.1.2.1 low-mid, PC.1.5.1 bimodal, PC.1.7.1 low, AM.2.1.7 high, RM.1.4.1 variable, RM.1.5.3 low, RM.1.2.1 bimodal
tensions   = "C present in scaffolded form but SO doesn't support practice"; "RM value recognized but PO time scarcity blocks realization"; "SO.4 incentives reinforce AM.2.1 competing habits"
leverage   = PO.4 + SO.1 (visibility → norms), SO.4 (incentive realignment), PC.1.7 + PO.5 + AM.2.1 (scaffolded practice → habit)
functions  = EN > ER > MO > TR > PE
bcts       = EN→BCT.1.4,BCT.7.1,BCT.3.2 | ER→BCT.12.2,BCT.12.1,BCT.12.5 | MO→BCT.6.1,BCT.6.3,BCT.9.1 | TR→BCT.8.7,BCT.8.1,BCT.2.2 | PE→BCT.13.2,BCT.5.3,BCT.11.2
```

### Consolidated Priority Order

1. **EN (Enablement):** The primary barriers are structural. People need scaffolds (BCT.7.1, BCT.12.5), action plans (BCT.1.4), and social support (BCT.3.2) to bridge the gap between "AI tools are available" and "AI tools are part of how I work." EN is the prerequisite for other functions — without it, training doesn't stick and modeling doesn't translate to practice.

2. **ER (Environmental Restructuring):** The environment currently defaults to non-AI workflows. ER changes the default: tool configurations that surface AI (BCT.12.1), social structures that assign ownership (BCT.12.2), and visibility artifacts that make gains tangible (BCT.12.5). ER also addresses the incentive structure (SO.4) through BCT.12.2.

3. **MO (Modelling):** Norms shift through observation, not instruction. BCT.6.1 (demonstration) from identity-congruent peers is the single most effective technique for addressing the SO.1 normative gap, SO.5 legitimacy gap, and RM.1.4 identity barrier simultaneously.

4. **TR (Training):** Capability building through practice. BCT.8.7 (graded tasks) ensures early wins that build RM.1.2 efficacy. BCT.8.1 (practice) with BCT.2.2 (feedback) builds PC.1.1 procedural fluency and PC.1.3 judgment over time. Training must be embedded in workflow, not separated from it.

5. **PE (Persuasion):** Reframing to address the motivational undertow. BCT.13.2 (framing/reframing) makes AI use identity-safe. BCT.11.2 (reduce negative emotions) addresses job-displacement anxiety. BCT.5.3 (information about consequences) makes the organizational case vivid.

---

## Step 5: Recommendations

### Phase A: Summary and Key Insights

#### Summary

AI adoption at Level 2 is stuck in a classic "partially realized / inconsistent" pattern — the tools are available, some people love them, but organizational adoption isn't compounding. The primary barrier isn't that people lack capability or motivation; it's that the organizational environment doesn't actively support, reinforce, or make visible the productivity gains from AI use. Employees face an environment where AI use is optional, invisible, un-incentivized, and in some cases reputationally risky. This means the highest-leverage interventions are environmental, not educational: make gains visible, normalize AI use through modeling, fix the incentive structure, and embed AI into workflow defaults.

The secondary barrier is a deeply entrenched set of non-AI work habits. People have been typing first drafts, manually summarizing meetings, and searching through documents for years — these behaviors are automatic. AI-assisted alternatives require conscious effort, learning investment, and tolerance for imperfect outputs. Breaking this habit-behavior pattern requires more than awareness; it requires deliberate habit-formation strategies anchored to existing workflow triggers, starting with the use cases where AI reward is most immediate and consistent.

The recommended direction is to invest first in environmental restructuring and enablement (making AI the easy, visible, recognized choice), then layer in embedded training and social modeling (making AI use normal and buildable), and use persuasion strategically to address identity concerns and job-displacement anxiety. Avoid mandates, comprehensive training programs, and heavy external incentivization — these address the wrong barriers and risk creating compliance without commitment.

#### Key Insights

1. **The incentive structure is the silent killer.** Most organizations have focused on tool provisioning and training while ignoring the fact that performance evaluation systems don't recognize AI-driven efficiency. An employee who saves 5 hours/week using AI meeting notes is evaluated identically to one who manually transcribes. Worse, visible efficiency can trigger fear of headcount reduction. Until the incentive structure rewards — or at minimum doesn't penalize — AI adoption, persuasion and training investments will be wasted on a misaligned environment.

2. **Identity, not capability, is the hidden veto.** Many technically capable employees don't adopt AI tools because using AI conflicts with their professional self-concept. Writers who value craftsmanship, analysts who value deep synthesis, strategists who value original thinking — these employees see AI as a threat to what makes their work *theirs*. Framing matters enormously: "AI augments your expertise" lands very differently than "AI saves you time." The most effective modeling comes not from tech enthusiasts but from respected professionals who share the audience's identity and demonstrate that AI enhances rather than diminishes their craft.

3. **Visibility creates a virtuous cycle — but it doesn't exist yet.** Individual AI productivity gains are completely invisible to the organization. No one sees that a colleague saved 3 hours using AI meeting notes. Without visibility, there's no social proof (people don't know others use AI), no norm formation (AI use doesn't become "what we do"), no organizational learning (successful practices can't spread), and no investment case (leadership can't quantify the ROI). Making gains visible is the single highest-leverage intervention because it activates multiple reinforcing loops simultaneously.

4. **Competing habits are stronger than competing attitudes.** The main thing preventing AI adoption isn't opposition — most employees are positive or neutral about AI. It's that existing work habits are deeply automatic: "open doc, start typing" beats "open doc, prompt AI, review, edit" every time cognitive load is high or time is short. Habit change requires anchoring AI use to specific existing workflow triggers ("when I get meeting notes, I run AI summary first"), starting with high-reward use cases that deliver immediate time savings, and accepting that habit formation takes weeks of consistent repetition.

5. **The progression blocker is governance, not capability.** Individual employees can learn to use AI tools effectively at Level 2. What they cannot do is compound their individual gains into team-level workflow automation (Level 3) without governance infrastructure: clear ownership of AI integration, coherent policies that resolve "use AI" vs. "protect data" tensions, cross-team consistency in AI practices, and workflow authority to redesign team processes around AI capabilities. The organization that solves Level 2 adoption without solving Level 2 governance will hit a ceiling.

### Phase B: In-Depth Report

#### Lens Analysis

##### Capability Findings

The capability landscape at Level 2 reveals a workforce in early-stage supported performance. Most employees sit at PC.1.7.1 (independence) low — they can use AI features when guided but cannot independently identify AI opportunities or design their own AI-assisted workflows. This is appropriate and expected at Level 2; the error would be treating scaffold-dependence as a failure rather than as the natural precursor to fluency.

**Knowledge and procedural fluency (PC-1.1):** Declarative knowledge (PC.1.1.1) is partial — employees generally know AI features exist in their tools but lack specifics about what the tools can do across their full range of use cases. The larger gap is procedural fluency (PC.1.1.2): even employees who know about AI features lack the step-by-step competence to use them effectively. They don't know how to write good prompts, how to iterate on AI output, or how to judge when AI-generated content is good enough. Sequence clarity (PC.1.1.3) is low — "how to incorporate AI into my task flow" is not specified. Exception handling (PC.1.1.6) is particularly weak: when AI produces mediocre output, users either accept it uncritically or abandon the tool entirely, lacking strategies for improvement.

**Mental models (PC-1.2):** Most employees hold inaccurate models of AI capabilities — either "magic box" (over-trust) or "useless toy" (under-trust). Few understand that embedded AI assistants are probabilistic systems that respond to context and prompt quality. This mental model gap (PC.1.2.1) drives systematic errors: over-trusters accept hallucinated content, under-trusters dismiss useful output based on a single bad experience. Causal understanding (PC.1.2.2) is low — people don't understand *why* AI gives good output sometimes and poor output other times, which prevents them from systematically improving their use.

**Judgment (PC-1.3):** The judgment demands of AI-assisted work are underappreciated. Deciding when AI output needs editing versus when it's good enough, when to use AI versus write from scratch, and how much context to provide requires calibrated judgment that develops through experience, not instruction. Currently, heuristic quality (PC.1.3.3) is low (people rely on "if it sounds right, it's right"), rule dependence (PC.1.3.5) is mid-high (rigid rules rather than flexible judgment), and tradeoff handling (PC.1.3.7) is weak.

**Metacognition (PC-1.5):** Calibration (PC.1.5.1) is bimodal — a dangerous pattern. Over-confident users form one failure mode; under-confident users form the other. Error detection (PC.1.5.3) is the most concerning gap: users routinely miss AI errors (factual inaccuracies, tone mismatches, hallucinated citations) because they haven't developed the metacognitive habit of critical AI output review.

**Shared representations (PC-1.6):** Low across the board. Teams lack shared language (PC.1.6.1) for AI use, common ground (PC.1.6.4) about what good AI-assisted work looks like, and behavior specification (PC.1.6.8) for the target behavior. This matters most for Behavior B (the progression blocker) — individual adoption can proceed with individual capability, but compounding requires shared frames.

##### Opportunity Findings

**Physical Opportunity (PO):**

Work-system coherence (PO.1.1) is mid — AI has been added atop existing systems rather than integrated into them. This "bolt-on" architecture means AI tools exist alongside the old workflows rather than replacing them, and the choice to use AI requires an active decision at every task. Feedback loops (PO.1.5) are notably weak — there is no systematic mechanism for users to learn whether their AI-assisted output was better, faster, or more effective. Learning happens by anecdote and intuition.

Time scarcity (PO.2.1) is the most cited physical barrier. The "learning dip" — where AI use initially takes longer before it saves time — competes directly with delivery pressure. This creates a painful irony: the people who would benefit most from AI time savings can least afford the upfront learning investment. Activation overhead (PO.2.7) varies by use case: low for simple embedded features (inline Copilot suggestions), high for more powerful applications (custom prompting, complex summarization).

The most consequential PO gap is visibility (PO.4). Signal surfacing (PO.4.1), cost visibility (PO.4.8), and friction visibility (PO.4.9) are all low. Productivity gains are invisible to peers, managers, and the organization. The cost of *not* using AI is equally invisible — manual work is normalized. Without visibility, there is no mechanism for social learning, norm formation, investment justification, or workflow improvement.

**Social Opportunity (SO):**

The normative environment (SO-1) shows the classic "approved but uncommon" pattern: injunctive norms (SO.1.2) are mid (organizations officially encourage AI), but descriptive norms (SO.1.1) are low-mid (most employees see AI use as a minority behavior). Critically, norm consistency (SO.1.4) is low — leadership messaging ("embrace AI") contradicts operational norms (work evaluated by traditional standards, no recognition for efficiency). Norm clarity (SO.1.3) is also low: mixed signals about what's acceptable AI use create conservative defaults.

Ownership and role clarity (SO-2) is a primary structural gap. Nobody owns AI adoption as an organizational practice. IT provisions licenses; L&D runs training sessions; individual managers set team norms. The result is inconsistent adoption driven by managerial preference rather than organizational strategy. This gap is the single biggest barrier to progression from Level 2 to Level 3.

The incentive architecture (SO-4) is neutral-to-hostile. Reward alignment (SO.4.1) favors output over efficiency — there's no incentive to do the same work faster. Recognition visibility (SO.4.5) is absent — AI-driven gains can't be celebrated because they can't be seen. Most concerning is penalty risk (SO.4.7): a significant number of employees fear that demonstrating AI-driven efficiency will trigger headcount reduction or workload inflation. This is a rational fear based on organizational history, not paranoia.

Legitimacy (SO-5) varies dramatically by professional identity. AI-assisted work is broadly "acceptable" (SO.5.1 mid) but not universally seen as professionally legitimate. Identity safety (SO.5.3) is the hidden variable: for roles where craft and expertise are core to identity (writers, analysts, strategists), AI assistance can feel like an admission of inadequacy. Professional congruence (SO.5.5) ranges from high (engineers: "better tools make better engineers") to low (writers: "if AI writes it, what am I for?").

Governance (SO-7) lags reality. Local autonomy (SO.7.1) is mid — teams can adopt AI but lack guidance. Policy-operational coherence (SO.7.5) is low — AI policies don't keep pace with tool capabilities, creating contradictions. Cross-group consistency (SO.7.8) is low — neighboring teams have wildly different AI adoption levels, blocking workflow integration.

##### Motivation Findings

**Reflective Motivation (RM):**

Self-determination (RM-1.1) presents a segmented picture. Early adopters (~15-20% of knowledge workers) are autonomously motivated — they find AI genuinely interesting and useful. The middle majority (~50-60%) is in a motivation limbo: positively disposed but not internally driven. The trailing group (~20-30%) ranges from indifferent to resistant. Internalization (RM.1.1.6) is low-mid overall — for most, AI use is still "an extra thing" rather than "how I work."

Self-efficacy (RM-1.2) is bimodal and fragile. Technical employees and early adopters report high efficacy; non-technical employees and the middle majority report low-to-mid. Crucially, recovery after setbacks (RM.1.2.3) is low across the board — one bad AI experience often poisons the well for that entire use case. Task specificity (RM.1.2.4) is low: confidence with one AI tool doesn't transfer to another.

Expectancy-value-cost (RM-1.3) reveals that the value proposition is recognized (utility value RM.1.3.4 is mid-high) but effort cost (RM.1.3.5) is also mid-high, and present-vs-future weighting (RM.1.3.8) favors present costs over future benefits. The practical implication: people acknowledge AI could save them time but perceive the learning investment as not worth it *right now*, especially under delivery pressure.

Identity (RM-1.4) is the most underappreciated barrier. Identity congruence (RM.1.4.1) varies by role and is strongly predictive of adoption. Identity conflict (RM.1.4.3) is mid — some employees experience genuine tension between "I value craftsmanship" and "I use AI to produce faster." Reputation risk (RM.1.4.7) adds a social layer: "Did she actually write that, or did AI?" can undermine perceived contribution.

Intentions (RM-1.5) show the classic gap: many employees express intention to use AI more (RM.1.5.1 mid) but have not converted that into specific plans (RM.1.5.3 low) or cue linkages (RM.1.5.4 low). The intention exists but lacks the implementation-intention structure to bridge to action.

**Automatic Motivation (AM):**

Habit (AM-2.1) is the primary automatic motivation barrier. Existing work habits are deeply entrenched (AM.2.1.7 high competing habit strength) — "open doc, start typing" is automatic. AI-assisted alternatives (AM.2.1.1 low automaticity) require deliberate decision-making. Under cognitive load or time pressure, the old habit wins every time. This is not a motivation problem in the reflective sense — it's an automaticity problem that requires environmental and behavioral interventions.

Reward (AM-2.2) presents a mixed but fundamentally favorable picture. For simple use cases, AI reward is immediate and compelling. The variability in reward magnitude (AM.2.2.2 mid) is the concern — inconsistent AI output quality creates an unreliable reinforcement schedule that undermines habit formation.

Affect (AM-2.3) adds emotional complexity. Anticipatory anxiety (AM.2.3.3) about job displacement and AI dependency is real and cannot be addressed by rational argument alone. The social-emotional intensity (AM.2.3.5) around AI is higher than around typical workplace tools because it touches professional identity and job security.

#### Cross-Lens Assessment

The central dynamic is a three-way interaction between **opportunity structures**, **habit patterns**, and **identity**:

1. The opportunity structure (PO + SO) currently defaults to non-AI workflows. Tools are available but not configured for AI-first use. Gains are invisible. Incentives don't reward adoption. Norms are unclear. Governance lags reality. This environmental default *reinforces* existing habits.

2. Existing work habits (AM.2.1) are strong and automated. Without environmental restructuring, these habits will persist regardless of capability-building or motivational interventions. The habit layer is where capability and motivation go to die if the environment doesn't support them.

3. Professional identity (RM.1.4 + SO.5) acts as a hidden veto. Even when tools are available, time exists, and the value proposition is clear, employees whose professional identity conflicts with AI use will avoid or resist adoption. Identity-based resistance looks like many things — "I don't have time," "the AI isn't good enough," "I prefer to do it myself" — but the root is identity threat, not the stated objection.

The prerequisite logic runs: **SO.4 → SO.7 → SO.1 → RM.1.4 → RM.1.5 → AM.2.1**. Fix the incentive structure (SO.4) and governance (SO.7) first, because these are structural barriers that block everything downstream. Then address norms (SO.1) through modeling. Then reframe identity (RM.1.4). Then build specific implementation intentions (RM.1.5). Then anchor new habits (AM.2.1). Throughout, layer in capability-building (PC) through scaffolded practice — but always in service of the opportunity and habit agenda, never as a standalone program.

#### BCW and BCT Reasoning

**EN (Enablement) — Priority 1:**
Enablement is the connective tissue of the intervention strategy. BCT.1.4 (action planning) bridges the RM.1.5 intention-action gap — converting "I should use AI more" into "when I receive meeting notes, I will run AI summary before reading." BCT.7.1 (prompts/cues) embeds AI triggers at natural workflow moments — contextual nudges that make AI the default rather than the alternative. BCT.3.2 (social support, practical) creates peer support structures — pairing new AI users with experienced peers for the first attempts that build or break confidence.

EN also works through BCT.12.5 (adding objects to the environment): prompt libraries in team workspaces, AI-ready document templates, shared dashboards showing time-savings data. These objects lower PO.2.7 activation overhead and make PO.4 gains visible simultaneously.

**ER (Environmental Restructuring) — Priority 2:**
Environmental restructuring changes the defaults. BCT.12.2 (restructuring the social environment) assigns clear ownership for AI integration per team, creates AI champion roles, and realigns the performance evaluation to recognize efficiency. BCT.12.1 (restructuring the physical environment) configures tools for AI-first interaction — default templates that prompt AI use, meeting tools that auto-generate summaries, document editors that surface AI assist prominently. BCT.12.5 (adding objects) creates visibility dashboards, success-story archives, and shared prompt libraries.

ER directly addresses the three highest-leverage opportunity gaps: incentive alignment (SO.4) through BCT.12.2, visibility (PO.4) through BCT.12.5, and norm formation (SO.1) through environmental signals that make AI use the expected default.

**MO (Modelling) — Priority 3:**
Modeling shifts norms through observation rather than instruction. BCT.6.1 (demonstration of behavior) from identity-congruent peers — the senior writer who uses AI for first drafts, the operations manager who relies on AI meeting notes, the financial analyst who uses AI data extraction — is more persuasive than any training program. BCT.6.3 (information about others' approval) signals social permission. BCT.9.1 (credible source) from senior leadership who visibly use AI in their own work (not just advocate for it) resolves SO.1.4 norm consistency.

The key design principle for modeling: models must share the audience's professional identity. An engineer demonstrating Copilot doesn't move a copywriter. A product manager demonstrating Notion AI doesn't move a legal analyst. Identity-congruent modeling (RM.1.4) addresses both the norm gap and the identity gap simultaneously.

**TR (Training) — Priority 4:**
Training builds PC.1.1 procedural fluency, PC.1.3 judgment, and PC.1.5 calibration through practice. BCT.8.7 (graded tasks) structures the learning path: start with meeting summarization (immediate reward, low complexity), progress to writing assistance (mid reward, mid complexity), then to data extraction and analysis (high reward, higher complexity). BCT.8.1 (behavioral practice/rehearsal) uses employees' own work — real tasks, real documents, real meetings — not artificial exercises. BCT.2.2 (feedback on behaviour) provides coaching on prompt quality, output evaluation, and AI output editing — the skills that standard training misses.

Training must be interleaved with EN and ER: scaffolds in the workflow, peer support structures, and environmental defaults that sustain practice beyond the training session.

**PE (Persuasion) — Priority 5:**
Persuasion addresses the emotional and identity layers that persist even after environmental changes. BCT.13.2 (framing/reframing) reframes AI as professional augmentation: "AI makes a great analyst better" rather than "AI replaces analysis." BCT.5.3 (information about social and environmental consequences) makes the organizational case vivid — what teams and companies gain from AI adoption, what they lose from non-adoption. BCT.11.2 (reduce negative emotions) directly addresses AM.2.3 anxiety through explicit organizational commitments about job security and workload.

#### Framework Observations

This diagnosis reveals that AI tool adoption at Level 2 is substantially an *organizational behavior change* problem, not an individual learning problem. The typical approach — provide tools, run training, hope for adoption — addresses the least important barriers (individual capability) while ignoring the most important ones (environmental defaults, habit patterns, normative climate, incentive alignment, and professional identity).

The most surprising finding is the degree to which **professional identity** (RM.1.4) acts as a hidden adoption veto. Many organizations underestimate this because identity-based resistance presents as something else ("I don't have time," "the tool isn't good enough"). Identity work through modeling and reframing is not a "soft" intervention — it is a structural prerequisite for adoption among the professional roles that arguably have the most to gain from AI assistance.

The progression blocker (Behavior B) reveals that individual adoption and organizational progression require fundamentally different intervention strategies. Individual adoption can be addressed through EN, MO, and TR targeted at individuals. Organizational progression requires ER targeted at governance structures (SO.7), role clarity (SO.2), and cross-team consistency (SO.7.8) — structural changes that individuals cannot make for themselves.

A notable tension exists between autonomy and structure. Early adopters thrive with autonomy (more tools, fewer restrictions). The middle majority needs structure (clear expectations, specific guidance, social proof). A single intervention strategy cannot serve both — the organization needs a segmented approach that gives early adopters freedom while providing the middle majority with scaffolded, socially supported entry paths.

Finally, the habit barrier (AM.2.1) deserves more attention than it typically receives. Even after all other barriers are addressed — tools available, capability built, identity safe, incentives aligned — the old habit of manual work will persist under cognitive load unless deliberately displaced. Habit formation is slow (weeks of consistent repetition in stable contexts) and requires specific if-then triggers anchored to existing workflow moments. This is the long game of AI adoption, and it cannot be shortcutted.

---

*Analysis conducted using COM-B (Michie, van Stralen & West), the Behaviour Change Wheel (Michie, Atkins & West, 2014), and BCT Taxonomy v1 (Michie et al., 2013).*
