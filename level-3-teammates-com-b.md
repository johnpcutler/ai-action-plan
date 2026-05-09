# COM-B Behavioral Diagnosis: AI as Teammates (Level 3)

## AI Maturity Model — Level 3: Automate repetitive work, increase team efficiency

---

# Step 1 — Behavior Canvas

## Behavior A: Adoption Behavior

| Field | Definition |
|-------|-----------|
| **Behavior** | Teams design, build, and operate AI agents that autonomously handle multi-step workflows, routing, triage, and cross-tool coordination |
| **Who** | Cross-functional teams (engineering, operations, support, product, finance) — with a critical dependency on engineering for initial enablement and platform/IT for infrastructure |
| **Will do what** | Identify automatable workflows → design agent logic (prompts, tool use, MCP integrations) → build and deploy agents → monitor agent performance → iterate on agent behavior → hand off routine operation to agents |
| **To what extent** | Multiple teams across the organization are running production agents that handle real workflow steps autonomously. Agents span multiple tools via connectors/MCPs. Agent governance is formalized. This is not a pilot — it is operating at team scale. |
| **In what context** | Enterprise environment with existing tool ecosystems (Slack, Jira, Salesforce, databases, internal APIs). Agents operate within security and compliance constraints. Teams have varying technical sophistication — some have engineers, some do not. |
| **For what outcome** | Teams operate with significantly higher leverage. Multi-step workflows run autonomously, freeing capacity. Cross-functional processes become faster and more reliable. Organizational capacity scales beyond headcount. |
| **Current state** | **Partially Realized / Inconsistent** — Exists in pockets (usually engineering-adjacent teams or teams with a technical champion). Most teams are still at Level 2 (individual AI tool use). Some teams have built one-off automations but haven't operationalized them. |
| **Prior attempts** | Many organizations have tried: (1) Top-down "AI transformation" mandates that produced training sessions but no production agents. (2) Innovation labs or hackathons that built demos but not operational systems. (3) Purchasing AI platforms without investing in workflow documentation or integration infrastructure. (4) Expecting non-technical teams to "just use" agent-building tools that assumed engineering fluency. These failed because they addressed motivation or tooling without addressing capability, workflow readiness, or governance simultaneously. |

## Behavior B: Progression Blocker

| Field | Definition |
|-------|-----------|
| **Behavior** | Organizations scale team-level AI automation to enterprise-wide AI-native operations (progressing from Level 3 to Level 4) |
| **Who** | Organizational leadership, platform/infrastructure teams, and cross-functional teams collectively |
| **Will do what** | Standardize agent architectures → establish shared agent platforms → create governance that enables rather than blocks → build agent-to-agent coordination → develop enterprise-wide AI operating models |
| **To what extent** | AI agents are the default operating mode, not an exception. Agent coordination happens across organizational boundaries. The organization has shifted from "teams using AI" to "AI-native operations." |
| **In what context** | Organizations that have achieved Level 3 in pockets but face fragmentation, governance gaps, inconsistent practices, and coordination failures when trying to scale |
| **For what outcome** | Enterprise-wide operational leverage. AI becomes the operating system of the organization, not a tool used by individual teams. |
| **Current state** | **Aspirational Only** — Identity-level desire without practice, infrastructure, or defined skill. Most organizations at Level 3 have pockets of success but no coherent path to Level 4. |
| **Prior attempts** | Attempts to standardize too early (before teams have enough experience). Governance frameworks that restrict rather than enable. Platform investments that don't match how teams actually build agents. |

---

# Step 2 — Dimensional Lens Analysis

## Capability (PC)

### PC-1.1-Knowledge: Declarative and Procedural Knowledge

**Diagnostic question:** Do teams have the technical knowledge to build agents — prompting, tool use, MCP, workflow design?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.1.1 Declarative knowledge | Low-to-mid | Most teams understand what AI agents are conceptually. Few understand the specifics: how prompt chaining works, what MCP (Model Context Protocol) does, how tool-use APIs function, or how to design reliable multi-step workflows. Knowledge is concentrated in engineering teams. |
| PC.1.1.2 Procedural fluency | Low | Even among those with conceptual understanding, few have built and deployed a production agent end-to-end. The procedure — from workflow analysis through prompt design, testing, deployment, monitoring — is unfamiliar. |
| PC.1.1.3 Sequence clarity | Low | The sequence for building an agent is not well-defined in most organizations. There is no established "playbook" for going from identified workflow to running agent. |
| PC.1.1.6 Exception handling | Very low | Teams building their first agents focus on the happy path. They don't anticipate agent failure modes — hallucination, tool errors, permission failures, edge cases in workflow logic. |
| PC.1.1.7 Transfer readiness | Low | Teams that have built one agent in one context (e.g., a Slack triage bot) can't easily transfer that knowledge to a different domain (e.g., a database automation or a cross-tool workflow). |

**Assessment:** This is a major gap. The knowledge to build AI agents is genuinely new and genuinely technical. It is not a matter of "just learning a new tool" — it requires understanding prompt engineering, API architectures, failure modes, and workflow design simultaneously. The gap is worst for non-engineering teams who are expected to build domain-specific agents but lack foundational technical fluency.

### PC-1.2-Models: Mental Models

**Diagnostic question:** Do teams understand how agents work, fail, and need oversight?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.2.1 Model accuracy | Low | Most people hold one of two wrong models: (a) "AI agents are magic — give them instructions and they work" or (b) "AI agents are unreliable toys — they can't handle real work." Neither model supports good agent design. |
| PC.1.2.2 Causal understanding | Low | Teams don't understand why agents fail. They can't trace a failure to prompt design, tool configuration, context window limits, or workflow logic errors. This makes debugging impossible. |
| PC.1.2.4 Dynamical understanding | Low | Teams don't understand how agent behavior changes over time — model updates, prompt drift, changing data patterns, accumulating edge cases. They treat agents as static deployments. |
| PC.1.2.7 Updateability | Low-to-mid | Some teams are open to updating their models; others are locked into initial impressions (either "AI is amazing" from a demo, or "AI failed us" from a bad early experience). |

**Assessment:** The mental model gap is perhaps more damaging than the knowledge gap. Wrong mental models lead to wrong design decisions. Teams that think agents are magic don't build oversight mechanisms. Teams that think agents are unreliable don't invest in making them work. The "agents as deterministic software" model (borrowed from traditional automation) is particularly harmful — it leads teams to expect 100% reliability and abandon agents at the first failure.

### PC-1.3-Judgment: Judgment and Decision Competence

**Diagnostic question:** Can teams judge which workflows to automate and which need human oversight?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.3.1 Judgment demand | High | The decision space is large: which workflows to automate, how much autonomy to give agents, where to insert human checkpoints, how to handle failures. Every workflow has different risk profiles. |
| PC.1.3.4 Recognition competence | Low | Teams lack pattern recognition for "good agent candidates" vs. "bad agent candidates." They tend to either automate the wrong things (high-stakes, judgment-heavy workflows) or fail to automate the right things (high-volume, rule-based workflows). |
| PC.1.3.5 Rule dependence | High | Organizations want simple rules: "automate everything" or "never automate anything customer-facing." Neither works. The judgment required is context-sensitive. |
| PC.1.3.7 Tradeoff handling | Low | Teams struggle with the automation-oversight tradeoff: too much autonomy creates risk, too little autonomy eliminates the value of automation. |

**Assessment:** Judgment is a critical and underappreciated gap. The most common failure pattern is not that agents are built poorly — it's that teams automate the wrong workflows or set the wrong autonomy boundaries. This is a judgment problem, not a technical one.

### PC-1.5-Meta: Metacognition and Calibration

**Diagnostic question:** Can teams detect when agents are failing silently?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.5.1 Calibration | Poor — overconfident | Teams that deploy agents tend to trust them too quickly. "It worked for a week, so it must be fine." Silent failures — agents producing plausible but wrong outputs — go undetected. |
| PC.1.5.3 Error detection | Low | Agent errors are often not obvious. Unlike software bugs that crash, agent failures look like reasonable outputs. Teams don't have the monitoring habits or tools to catch these. |
| PC.1.5.5 Uncertainty awareness | Low | Teams don't know what they don't know about their agents' behavior. They can't articulate the boundaries of their agents' competence. |

**Assessment:** This is the "silent killer" dimension. The most dangerous agent deployments are the ones that seem to work fine. Overconfidence after initial success leads to reduced monitoring, which leads to undetected failures, which leads to either a costly incident or a slow degradation of output quality that nobody notices.

### PC-1.6-Shared: Shared Representations and Conceptual Alignment

**Diagnostic question:** Is there shared understanding of agent capabilities across teams?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.6.1 Shared language | Low | "Agent," "automation," "workflow," "MCP," "tool use" — these terms mean different things to different teams. Engineering teams use precise technical definitions. Business teams use vague metaphors. This creates coordination failures. |
| PC.1.6.2 Conceptual alignment | Low | Teams have incompatible concepts of what agents can and should do. Support teams think of agents as chatbots. Engineering thinks of them as workflow orchestrators. Operations thinks of them as RPA replacements. |
| PC.1.6.5 Coordination literacy | Low | Nobody knows who has built what, what worked, what failed, or what's reusable. There is no organizational knowledge of distributed agent-building expertise. |
| PC.1.6.8 Behavior specification | Undefined | "What good looks like" for agent design, deployment, and operation is not defined. There are no shared standards for prompt quality, monitoring practices, or governance requirements. |

**Assessment:** Shared understanding is prerequisite to scaling from pockets to organization-wide practice. Without it, every team reinvents the wheel, repeats mistakes, and builds incompatible systems. This is a key blocker for the Level 3 → Level 4 transition.

### PC-1.7-Scaffold: Supported Performance and Scaffolding

**Diagnostic question:** Are teams being supported in building their first agents?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PC.1.7.1 Independence | Low | Most teams cannot build agents independently. They need significant support from engineering or AI-savvy colleagues. |
| PC.1.7.3 Prompt dependence | High | Teams that have built agents did so with heavy guidance. Remove the guidance, and they struggle to build the next one. |
| PC.1.7.8 Bootstrap accessibility | Low-to-mid | Some organizations have agent-building platforms (e.g., Cursor, Windsurf, internal tools), but the entry point for a non-technical team is still high. Templates and examples help but are often too generic. |

**Assessment:** The scaffolding gap is real and important. Teams need guided first experiences, not training decks. The absence of accessible scaffolding — templates, worked examples, pairing with experienced builders, graded complexity — is a primary reason why agent adoption stalls after initial enthusiasm.

---

## Opportunity — Physical (PO)

### PO-1-WorkSys: Work-System Configuration

**Diagnostic question:** Is the technical infrastructure ready — APIs, connectors, platforms?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.1.1 Work-system coherence | Low-to-mid | Most enterprise environments are a patchwork of tools with inconsistent API quality. Some tools have robust APIs; others have none. MCP connectors exist for some systems but not others. |
| PO.1.2 Tool-task fit | Low | Agent-building tools are designed for engineers. Non-technical teams face tools that assume coding fluency, understand API conventions, and can debug JSON errors. |
| PO.1.5 Feedback-loop strength | Weak | Agent performance monitoring is often ad hoc. Teams deploy agents and check outputs manually, if at all. Real-time feedback loops on agent performance are rare. |

**Assessment:** Infrastructure readiness is a genuine constraint. Even motivated, capable teams hit walls when the tools they need to connect don't have APIs, when MCPs don't exist for their systems, or when the agent-building platform assumes engineering skills they don't have. This is not a gap that training alone can close.

### PO-2-Resource: Resource and Capacity Conditions

**Diagnostic question:** Is there dedicated time and budget for building agents?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.2.1 Time availability | Scarce | Agent-building is treated as "extra" work on top of existing responsibilities. Teams are not given protected time to learn, experiment, or build. |
| PO.2.3 Slack margin | Low | Most teams are running at or above capacity. There is no slack to invest in automation — even when automation would create capacity in the future. |
| PO.2.4 Competing urgency | High | Urgent operational work consistently displaces agent-building work. "We'll automate it next quarter" becomes a standing deferral. |
| PO.2.7 Activation overhead | High | Getting started with agent-building requires significant upfront investment: learning tools, documenting workflows, securing API access, getting security approval. The startup cost is high relative to the time available. |

**Assessment:** This is the classic "investment paradox" — teams that most need automation are the ones with the least time to build it. Resource scarcity is not a perception problem; it's a structural one. Interventions that require significant time investment (lengthy training programs, complex platform onboarding) will fail in this context.

### PO-3-Workflow: Workflow and Process Architecture

**Diagnostic question:** Are existing workflows documented enough to automate?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.3.1 Path complexity | High | Real workflows are messy. They have exceptions, branches, human judgment steps, and undocumented tribal knowledge. The "clean" workflow that seems automatable on a whiteboard is much messier in practice. |
| PO.3.2 Handoff burden | High | Many valuable workflows span teams and tools. The handoff points — where one person's output becomes another person's input — are exactly where agents are most valuable and most fragile. |
| PO.3.7 Activation energy | High | Even when a workflow is identified as a good automation candidate, the effort to document it precisely enough for agent automation is substantial. |

**Assessment:** Workflow documentation is the hidden prerequisite. You can't automate what you can't describe. Most organizations dramatically underestimate how much implicit knowledge lives in their workflows — and how much work it takes to make that knowledge explicit enough for an agent.

### PO-5-Tooling: Tooling and Interface Affordances

**Diagnostic question:** Are agent-building tools accessible to non-engineers?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.5.1 Affordance clarity | Low for non-engineers | Agent-building platforms vary enormously. Some (like Cursor for code) are powerful but assume engineering context. "No-code" agent platforms exist but often can't handle the complexity of real workflows. |
| PO.5.4 Error tolerance | Low | Agent-building tools often fail with cryptic errors. A misconfigured MCP, a wrong API key, a malformed prompt — the error messages don't help non-technical users diagnose or fix the problem. |
| PO.5.6 Learnability in context | High burden | The learning curve for agent-building tools is steep, especially for teams that don't already understand APIs, JSON, or prompt engineering. |

**Assessment:** The tooling gap is a form of structural exclusion. When agent-building tools require engineering fluency, non-engineering teams are effectively locked out of Level 3 — they depend on engineering bottlenecks to build agents for them, which doesn't scale.

### PO-7-Control: Control Loops and Adaptive Regulation

**Diagnostic question:** Are there monitoring and feedback loops for agent performance?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| PO.7.1 Feedback latency | Long | Most agent deployments lack real-time monitoring. Teams discover agent failures through downstream effects — a customer complaint, a missed SLA, a bad data entry — rather than through proactive monitoring. |
| PO.7.2 Signal fidelity | Low | When monitoring exists, the signals are often noisy. "Agent completed successfully" doesn't mean the output was correct. Output quality monitoring requires domain expertise and is rarely automated. |
| PO.7.3 Corrective authority | Slow escalation | When an agent fails, the fix often requires engineering involvement. The team running the workflow can't correct the agent themselves. |
| PO.7.7 Variety handling | Exceeded | Real-world variability in inputs regularly exceeds what agents were designed to handle. Edge cases accumulate and aren't systematically addressed. |

**Assessment:** The monitoring and feedback gap is what separates "demo agents" from "production agents." Without robust feedback loops, agents degrade silently. This is especially dangerous because agent failures are often not catastrophic — they're subtle, producing outputs that are plausible but wrong.

---

## Opportunity — Social (SO)

### SO-1-Norms: Norms and Normative Climate

**Diagnostic question:** Is building and using agents normalized across teams?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.1.1 Descriptive norm | Low | In most organizations, building AI agents is not something most teams do. It's associated with "technical" or "innovative" teams. The descriptive norm says: "Normal teams don't build agents." |
| SO.1.2 Injunctive norm | Mid-to-high | Leadership often approves of AI adoption in principle. "We should be using AI" is a common leadership message. But approval without practice creates a gap. |
| SO.1.4 Norm consistency | Low | Leaders say "use AI" but don't change metrics, timelines, or resource allocations to make it possible. The message and the operating reality are misaligned. |
| SO.1.6 Norm volatility | Mid | AI priorities shift with executive attention cycles. Teams have seen previous technology initiatives ("digital transformation," "RPA," "data-driven") come and go. They are hesitant to invest heavily in what might be another passing trend. |

**Assessment:** There is a significant say-do gap. Leadership endorses AI adoption but doesn't create the conditions for it. This norm inconsistency (SO.1.4) is particularly damaging — teams learn to ignore stated priorities that aren't backed by structural change.

### SO-2-Roles: Roles, Authority, and Boundary Clarity

**Diagnostic question:** Who owns agent development — engineering vs. business teams?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.2.1 Ownership clarity | Ambiguous | Nobody clearly owns agent development. Engineering says it's a business decision (which workflows to automate). Business says it's a technical decision (how to build agents). The result is a jurisdictional gap where nobody acts. |
| SO.2.2 Decision-right clarity | Contested | Who decides whether a workflow should be automated? Who approves an agent for production use? Who is responsible when an agent makes a mistake? These questions are unresolved. |
| SO.2.5 Role conflict | High | Engineers are asked to "build agents for the business" while also maintaining their existing systems. Business teams are asked to "define what agents should do" but don't have the technical vocabulary. Both feel like they're being asked to do someone else's job. |
| SO.2.6 Accountability fit | Misaligned | Teams deploying agents often have responsibility for outcomes but no authority over the agent's design or the platform it runs on. |

**Assessment:** Role ambiguity is one of the top structural barriers. Agent development requires a new kind of collaboration between domain experts and technical builders. Most organizations haven't defined this collaboration model, so it defaults to ad hoc requests that bottleneck on engineering capacity.

### SO-4-Incentives: Incentives, Accountability, and Reinforcement

**Diagnostic question:** Are teams incentivized to automate, or does automation threaten roles?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.4.1 Reward alignment | Favors competing behavior | Teams are rewarded for output, not leverage. Building an agent that automates 40% of a workflow takes investment time that competes with delivering against current metrics. The reward system favors doing the work manually (visible output now) over automating (invisible investment for future capacity). |
| SO.4.4 Short-vs-long horizon | Short-term dominates | Quarterly targets and sprint commitments create short-term pressure. Agent-building is a long-term investment. The incentive structure consistently deprioritizes it. |
| SO.4.7 Penalty risk | Mid-to-high | If an agent makes a mistake, the team that deployed it bears the consequences. If the agent works well, the organization benefits but the team may not be recognized — or worse, may lose headcount because they're "more efficient." |

**Assessment:** The incentive misalignment is deep. Teams face a rational choice: invest scarce time in building agents (risky, delayed payoff, possible headcount reduction) or spend that time on immediate deliverables (safe, visible, rewarded). Until this calculus changes, adoption will be driven by intrinsic motivation and individual champions rather than systematic organizational behavior.

### SO-6-Power: Power, Politics, and Psychological Safety

**Diagnostic question:** Is it safe to experiment with agents that might fail?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.6.5 Permission to experiment | Low-to-mid | Agent experiments that fail visibly (e.g., a customer receives a bad automated response) create blame dynamics. Teams with low psychological safety won't take the risk. |
| SO.6.7 Transparency of rules | Low | What agents are allowed to do, what data they can access, what decisions they can make — these rules are often implicit or undefined. Teams operate in a gray zone where they don't know if they're allowed to build what they're building. |
| SO.6.8 Refinement openness | Low | Once an agent is deployed, the pressure is to "leave it alone" rather than iterate. Organizations with low refinement openness treat deployed agents like completed projects rather than living systems that need continuous improvement. |

**Assessment:** Psychological safety for agent experimentation is essential but rare. The combination of unclear rules (SO.6.7), risk of visible failure (SO.6.5), and low iteration culture (SO.6.8) creates a chilling effect. Teams build safe, limited agents — or don't build at all.

### SO-7-Governance: Governance Viability and Recursion

**Diagnostic question:** Are there governance frameworks for agent behavior and data access?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| SO.7.1 Local autonomy fit | Low | In most organizations, teams lack the authority to deploy agents without extensive approval processes. Security review, data access approval, compliance sign-off — each adds weeks to the deployment timeline. |
| SO.7.2 Coordination sufficiency | Weak | Teams building agents independently make incompatible choices: different platforms, different security approaches, different monitoring practices. Cross-team coordination on agent architecture is rare. |
| SO.7.5 Policy-operational coherence | Poor | Existing IT policies were written for human-operated systems. Applying them literally to AI agents creates absurdities (e.g., "every API call requires a human approval") or gaps (e.g., no policy for agent-to-agent communication). |
| SO.7.8 Cross-group consistency | Low | Every team that builds agents does it differently. There are no shared standards, shared platforms, or shared practices. This makes scaling from pockets to enterprise impossible. |

**Assessment:** Governance is the key blocker for the Level 3 → Level 4 transition. The paradox is that organizations need governance to scale safely, but premature governance (overly restrictive policies designed before anyone has experience) blocks the experimentation needed to inform good governance. The solution is governance that evolves with practice, not governance imposed in advance.

---

## Motivation — Reflective (RM)

### RM-1.1-SDT: Self-Determination Theory

**Diagnostic question:** Are teams intrinsically motivated to build agents, or is it a top-down mandate?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.1.1 Regulation quality | Mixed — ranges from controlled to autonomous | Some teams are genuinely excited about agent-building (autonomous motivation, usually technically fluent teams). Others experience it as another mandate from leadership (controlled motivation, "we have to use AI"). |
| RM.1.1.3 Autonomy support | Low-to-mid | Organizations vary, but many mandate *that* teams should use AI without giving them choice about *how* or *what to automate*. This undermines autonomy. |
| RM.1.1.6 Internalization | Surface for most | Leadership talking points about AI are repeated but not deeply internalized by most teams. "AI is the future" is mouthed but not felt. |

**Assessment:** Where intrinsic motivation exists — teams that are genuinely curious about what agents can do for their work — it is the strongest predictor of successful adoption. Top-down mandates without autonomy support produce compliance behaviors (attending training, installing tools) without real adoption (building and operating production agents).

### RM-1.2-Efficacy: Self-Efficacy

**Diagnostic question:** Do teams believe they can successfully build and operate agents?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.2.1 Efficacy belief | Low for non-technical teams, mid for engineering | Non-engineering teams see agent-building as "a developer thing." They doubt they have the skills, even when low-code tools exist. Engineering teams are more confident but still uncertain about new paradigms (prompt engineering vs. traditional coding). |
| RM.1.2.3 Recovery after setbacks | Fragile | A failed first agent attempt often kills further effort. "We tried AI and it didn't work" becomes the team's story. |
| RM.1.2.6 Source of efficacy | Weak mastery experiences | Most teams lack successful agent-building experiences to draw confidence from. They've seen demos (vicarious experience) but haven't done it themselves (mastery experience). |

**Assessment:** Efficacy is the motivational linchpin. Without it, capable teams don't attempt, and early failures become terminal. The most effective intervention is ensuring successful first experiences — not through unrealistically easy demos, but through genuinely useful agents built with appropriate scaffolding.

### RM-1.3-EVC: Expectancy-Value-Cost

**Diagnostic question:** Does the effort of building agents seem worth the payoff?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.3.1 Expectancy of success | Low-to-mid | Teams have seen impressive demos but are skeptical that agents will work reliably in their messy, real-world contexts. |
| RM.1.3.5 Effort cost | High | The perceived (and actual) effort to go from "no agent" to "production agent" is significant. Learning tools, documenting workflows, iterating on prompts, setting up monitoring — it's a substantial investment. |
| RM.1.3.7 Opportunity cost | High | Time spent building agents is time not spent on current deliverables. In resource-constrained teams, this is a real tradeoff, not just a perception. |
| RM.1.3.8 Present-vs-future weighting | Present cost dominates | The effort is now; the payoff is later. For teams under quarterly pressure, this temporal mismatch is decisive. |

**Assessment:** The cost-value calculus is rational, not irrational. Building agents *is* effortful, *does* have uncertain payoff, and *does* compete with immediate deliverables. Interventions that try to persuade teams that "it's worth it" without actually reducing the cost or accelerating the payoff will fail. The intervention must change the calculus, not just reframe it.

### RM-1.4-Identity: Identity-Based Motivation

**Diagnostic question:** Does building AI agents fit the professional identity of non-engineers?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.4.1 Identity congruence | Low for many roles | For operations managers, finance analysts, support leads, and other non-technical roles, "building AI agents" feels like stepping outside their professional identity. "I'm a support manager, not a developer." |
| RM.1.4.3 Identity conflict | Present | Some professionals feel that building agents to automate their own workflows is an identity threat: "Am I automating myself out of a job?" This creates an unresolvable conflict between professional survival and organizational benefit. |
| RM.1.4.5 Future-self pull | Weak | Few non-technical professionals have a vivid image of themselves as "agent builders." The identity aspiration doesn't exist yet. |

**Assessment:** Identity is the underappreciated motivational barrier. When building agents feels like "someone else's job" or threatens professional survival, no amount of training or tooling will drive adoption. The reframe must be genuine: agent-building as amplification of domain expertise, not replacement of it.

### RM-1.5-Intentions: Goal Intentions and Implementation Intentions

**Diagnostic question:** Have teams formed specific plans for which workflows to automate?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| RM.1.5.1 Intention strength | Weak for most teams | General interest in "using AI" does not translate to specific intentions about which workflows to automate, by when, or how. |
| RM.1.5.3 Plan specificity | Vague | Even teams that want to build agents haven't specified: "We will automate [this workflow] by [this date] using [this approach]." The intention stays abstract. |
| RM.1.5.5 Obstacle planning | Absent | Teams haven't anticipated what will go wrong when they try to build agents, or how they'll handle it when it does. |
| RM.1.5.6 Initiation readiness | Low | The first step is undefined. "Start building an agent" is not an actionable plan. |

**Assessment:** The intention-action gap is wide. Even motivated teams don't convert interest into specific plans, and without specific plans, no action follows. This is partly a symptom of other gaps (don't know enough to plan, don't have time to plan, don't have tools to plan with) and partly addressable directly through structured planning support.

---

## Motivation — Automatic (AM)

### AM-2.1-Habit: Habit Formation

**Diagnostic question:** How entrenched are manual workflow habits?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.1.1 Automaticity | High for manual workflows | Existing manual workflows are deeply habitual. Teams process tickets, route requests, update databases, and coordinate across tools on autopilot. The manual way of doing things runs automatically. |
| AM.2.1.5 Goal independence | High | Manual workflows persist even when teams agree they should be automated. The habit runs independently of the stated goal. |
| AM.2.1.7 Competing habit strength | Strong | Every manual workflow is a competing habit. Building agents requires replacing deeply entrenched routines, not just adding new ones. |

**Assessment:** Habit inertia is a powerful force. Teams don't continue doing things manually because they think it's better — they continue because it's automatic. The manual workflow requires no thought; the automated alternative requires sustained deliberate effort to establish. This asymmetry favors the status quo.

### AM-2.3-Affect: Affect and Emotion

**Diagnostic question:** Is there fear about agent reliability or "losing control"?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.3.1 Valence | Aversive for many | For many non-technical professionals, the emotional register around AI agents is anxiety: fear of looking incompetent, fear of agents making errors they'll be blamed for, fear of automation replacing their role. |
| AM.2.3.3 Anticipatory affect | Strong dread for some | "What if the agent messes up and I get blamed?" creates anticipatory dread that prevents even attempting to build agents. |
| AM.2.3.5 Social-emotional intensity | High | The shame of not understanding AI (in an environment that assumes everyone should) is real. So is the pride of building something that works. The emotional stakes are high in both directions. |

**Assessment:** The emotional landscape around AI agents is turbulent. Fear, anxiety, and shame coexist with excitement and aspiration. Interventions must manage the aversive emotions — not dismiss them as irrational — while building on the positive ones. The fear of losing control is especially important: it's not irrational, it reflects a genuine tension between automation and accountability.

### AM-2.4-Helplessness: Learned Helplessness

**Diagnostic question:** Have prior automation attempts failed, creating resignation?

| Dimension | Position | Evidence |
|-----------|----------|----------|
| AM.2.4.1 Perceived controllability | Low-to-mid | Teams that tried RPA, chatbot initiatives, or earlier "AI transformation" programs and saw them fail have learned that "automation initiatives don't work here." |
| AM.2.4.3 Generalization | Present | Failure with one technology (RPA, early chatbots) generalizes to skepticism about AI agents: "This is just the latest version of something that's failed before." |
| AM.2.4.7 Exposure duration | Prolonged for some | Organizations on their third or fourth "transformation" initiative have prolonged exposure to effort-outcome disconnection. |

**Assessment:** Prior failed automation attempts are the elephant in the room. Every organization that has tried and failed at RPA, chatbots, or digital transformation carries scar tissue. This isn't stubbornness — it's rational learning from experience. Interventions must acknowledge the history and demonstrate that this time is genuinely different, not just assert it.

---

# Step 3 — Practitioner Worksheet

## 1. COM-B Priority Ranking

| Rank | Branch | Rationale |
|------|--------|-----------|
| 1 | **Opportunity (O)** | The combination of infrastructure unreadiness (PO-1, PO-5), resource scarcity (PO-2), workflow documentation gaps (PO-3), missing feedback loops (PO-7), role ambiguity (SO-2), incentive misalignment (SO-4), and premature/absent governance (SO-7) creates the most powerful structural barrier. Even capable, motivated teams can't succeed when the infrastructure doesn't support agent-building, the time isn't protected, the roles aren't defined, and the incentives punish the investment. |
| 2 | **Capability (C)** | Genuine knowledge gaps (PC-1.1), wrong mental models (PC-1.2), poor judgment about what to automate (PC-1.3), inability to detect agent failures (PC-1.5), lack of shared understanding (PC-1.6), and insufficient scaffolding (PC-1.7) mean that even if opportunity existed, many teams couldn't execute. The capability gap is most acute for non-engineering teams. |
| 3 | **Motivation (M)** | Motivation barriers are real — especially identity threat (RM-1.4), low efficacy (RM-1.2), rational cost-benefit rejection (RM-1.3), entrenched habits (AM-2.1), fear (AM-2.3), and learned helplessness (AM-2.4). But motivation ranks third because it is substantially downstream of opportunity and capability: fixing the structural and capability barriers would resolve many of the motivational barriers. Teams that have the opportunity and capability to succeed are more likely to find the motivation. |

**Note:** Opportunity and Capability are roughly equal in importance and interact strongly. Neither can be addressed in isolation. Motivation is genuinely third, but it contains hidden gates — especially identity threat and learned helplessness — that can block adoption even when opportunity and capability are addressed.

---

## 2. Per-Lens Synthesis

### Capability (PC)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PC-1.1-Knowledge | PC.1.1.1 low-mid, PC.1.1.2 low, PC.1.1.3 low, PC.1.1.6 very low | Procedural fluency (PC.1.1.2) is the primary gap. Declarative knowledge exists but is shallow. TR via practice (BCT.8.1) with graded tasks (BCT.8.7) is needed, not more lectures. Exception handling (PC.1.1.6) requires BCT.1.2 problem solving after basic fluency is established. | BCT.8.1, BCT.8.7, BCT.6.1, BCT.4.1, BCT.1.2 |
| PC-1.2-Models | PC.1.2.1 low, PC.1.2.2 low, PC.1.2.4 low | Model accuracy gap is severe. BCT.4.4 (behavioral experiments) to surface wrong models. BCT.4.3 (re-attribution) to correct faulty causal reasoning about agent behavior. Static explanations won't build dynamic understanding (PC.1.2.4). | BCT.4.4, BCT.4.3, BCT.2.7 |
| PC-1.3-Judgment | PC.1.3.1 high, PC.1.3.4 low, PC.1.3.5 high, PC.1.3.7 low | Judgment demand is high but recognition competence is low. TR via realistic scenarios (BCT.8.1) with expert demonstration (BCT.6.1) to make tacit selection criteria visible. Rule dependence (PC.1.3.5) needs BCT.4.4 to build flexible judgment. | BCT.8.1, BCT.6.1, BCT.4.4, BCT.1.2 |
| PC-1.5-Meta | PC.1.5.1 poor (overconfident), PC.1.5.3 low | Overconfidence gates other capability interventions. Surface the calibration gap first with BCT.2.2 (feedback on behavior) before more training. BCT.4.4 to create "surprise" moments showing agents failing in non-obvious ways. | BCT.2.2, BCT.4.4, BCT.2.3 |
| PC-1.6-Shared | PC.1.6.1 low, PC.1.6.2 low, PC.1.6.5 low, PC.1.6.8 undefined | Shared definitions are prerequisite to scaling. ED via BCT.4.1 for common vocabulary. EN via BCT.12.5 (shared glossaries, pattern libraries). BCT.1.1 (goal setting) for shared "what good looks like" standards. | BCT.4.1, BCT.12.5, BCT.1.1, BCT.6.1, BCT.3.2 |
| PC-1.7-Scaffold | PC.1.7.1 low, PC.1.7.3 high, PC.1.7.8 low-mid | Teams need scaffolded first experiences. EN via BCT.8.7 (graded tasks) starting with simple agents. BCT.7.1 (prompts/cues) embedded in workflows. BCT.3.2 (social support, practical) through pairing with experienced builders. Don't rush to remove scaffolds. | BCT.8.7, BCT.7.1, BCT.3.2, BCT.12.5 |

**Narrative synthesis:** The capability picture is one of genuine, multi-layered gaps. This is not a case where people "already know but aren't doing" — they genuinely lack the knowledge, mental models, judgment, and meta-awareness needed to build production-quality agents. The critical insight is that these gaps are layered: you can't build judgment (PC-1.3) without accurate mental models (PC-1.2), and you can't build mental models without hands-on experience (PC-1.1), which requires scaffolding (PC-1.7). The intervention must address these in sequence, not in parallel. Training that jumps to advanced agent design without building foundational understanding will fail. The overconfidence calibration problem (PC-1.5) means that some teams think they don't need training, which makes ED harder to deliver.

**What to try:** Scaffolded, hands-on agent-building experiences (TR, EN) that build foundational fluency, correct mental models through direct experience, and develop judgment through realistic case analysis. Shared standards and vocabulary (ED, EN) to enable cross-team coordination.

**What not to try:** Lecture-based training programs, abstract "AI literacy" courses, or comprehensive certification programs. These address declarative knowledge (which is not the bottleneck) and consume the scarce resource (time) without producing the needed outcome (working agents).

### Opportunity (PO / SO)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| PO-1-WorkSys | PO.1.1 low-mid, PO.1.2 low, PO.1.5 weak | System-level misalignment requires ER (BCT.12.1) and EN (BCT.12.5). Tool-task fit (PO.1.2) for non-engineers is poor — tools need redesign, not just training. | BCT.12.1, BCT.12.5, BCT.1.2 |
| PO-2-Resource | PO.2.1 scarce, PO.2.3 low, PO.2.4 high, PO.2.7 high | Resource scarcity makes lengthy interventions impractical. ER to embed agent-building into existing work (BCT.12.1). EN to reduce activation overhead (BCT.12.5, BCT.7.1). Don't add training programs that consume more time. | BCT.12.1, BCT.12.5, BCT.7.1, BCT.1.4 |
| PO-3-Workflow | PO.3.1 high, PO.3.2 high, PO.3.7 high | Workflow documentation gap requires ER to simplify first automation targets. BCT.1.2 (problem solving) to identify which workflows are actually automatable vs. aspirationally automatable. | BCT.12.1, BCT.1.2, BCT.1.4 |
| PO-5-Tooling | PO.5.1 low, PO.5.4 low, PO.5.6 high burden | Tooling gap is structural exclusion. ER to improve agent-building tools (BCT.12.1). EN via BCT.12.5 (templates, guided workflows). TR via BCT.8.7 (graded tasks) with progressively complex tooling. | BCT.12.1, BCT.12.5, BCT.8.7, BCT.7.1 |
| PO-7-Control | PO.7.1 long, PO.7.2 low, PO.7.3 slow, PO.7.7 exceeded | Monitoring/feedback gap is critical for production agents. ER to build monitoring infrastructure (BCT.12.1). EN via BCT.2.2 and BCT.2.7 for feedback loops. BCT.1.2 for systematic error analysis. | BCT.12.1, BCT.2.2, BCT.2.7, BCT.1.2 |
| SO-1-Norms | SO.1.1 low, SO.1.2 mid-high, SO.1.4 low | Say-do gap (SO.1.4) is the key pattern. MO via BCT.6.1 to make agent-building visible. ER via BCT.12.2 to align leader behavior with stated priorities. Don't use BCT.6.2 (social comparison) — it highlights how few teams are actually doing it. | BCT.6.1, BCT.12.2, BCT.6.3 |
| SO-2-Roles | SO.2.1 ambiguous, SO.2.2 contested, SO.2.5 high | Role ambiguity blocks action. ER via BCT.12.2 to define agent-builder roles. BCT.1.8 (behavioral contract) to formalize ownership. BCT.4.1 for role boundary instruction. | BCT.12.2, BCT.1.8, BCT.4.1, BCT.1.1 |
| SO-4-Incentives | SO.4.1 misaligned, SO.4.4 short-term, SO.4.7 mid-high | Incentive misalignment is structural. ER via BCT.12.2 to realign reward systems. BCT.2.7 (feedback on outcomes) to make automation value visible. Don't layer new incentives on broken old ones. | BCT.12.2, BCT.2.7, BCT.10.4 |
| SO-6-Power | SO.6.5 low-mid, SO.6.7 low, SO.6.8 low | Create explicit safe-to-fail zones. ER via BCT.12.2 for structured experimentation. BCT.1.1 (goal setting) framed as learning experiments, not performance targets. | BCT.12.2, BCT.1.1, BCT.3.1, BCT.3.3 |
| SO-7-Governance | SO.7.1 low, SO.7.2 weak, SO.7.5 poor, SO.7.8 low | Governance must co-evolve with practice. ER via BCT.12.2 to create adaptive governance. BCT.4.4 (behavioral experiments) to test governance approaches. BCT.2.7 (feedback) across levels. Don't impose governance before practice has informed it. | BCT.12.2, BCT.4.4, BCT.2.7, BCT.1.1 |

**Narrative synthesis:** Opportunity is the largest barrier cluster, spanning both physical and social dimensions. The physical barriers (infrastructure gaps, resource scarcity, undocumented workflows, engineering-centric tools, missing monitoring) create the material conditions that make agent-building difficult. The social barriers (norm inconsistency, role ambiguity, incentive misalignment, political risk, governance gaps) create the organizational conditions that make agent-building unrewarded, unauthorized, or unsafe.

The critical interaction is between PO-2-Resource (no time to invest) and SO-4-Incentives (no reward for investing). Together, these create a rational case for non-adoption: "I don't have time to do this, and if I did, I wouldn't be rewarded for it — but I would be punished if it failed." Breaking this requires simultaneous action on resource protection and incentive realignment.

**What to try:** Environmental restructuring (ER) is the dominant function. Redesign the conditions: protect time for agent-building (PO-2), simplify tooling for non-engineers (PO-5), define roles and ownership (SO-2), realign incentives (SO-4), create safe experimentation zones (SO-6), and build adaptive governance (SO-7). Enable (EN) through reducing activation overhead, embedding agent-building into existing workflows, and building monitoring infrastructure.

**What not to try:** Individual-targeted interventions (PE, INC for individuals) won't overcome structural barriers. Don't incentivize individuals to use broken tools in their scarce time under misaligned reward systems. Fix the structure first.

### Motivation (RM / AM)

| Sub-lens | Key dimensions + positions | Pattern guidance conclusions | Relevant BCTs |
|----------|--------------------------|----------------------------|---------------|
| RM-1.1-SDT | RM.1.1.1 mixed, RM.1.1.3 low-mid, RM.1.1.6 surface | Where autonomous motivation exists, protect it. PE via BCT.13.2 (framing/reframing) to connect automation to personal values. EN via BCT.1.1 with genuine endorsement. Don't add more controlled motivation (mandates). | BCT.13.2, BCT.1.1, BCT.3.1 |
| RM-1.2-Efficacy | RM.1.2.1 low (non-eng), RM.1.2.3 fragile, RM.1.2.6 weak mastery | Efficacy is the motivational linchpin. PE via BCT.15.1 from relatable peers. EN via BCT.8.7 (graded tasks) for guaranteed early wins. BCT.6.1 (demonstration) from non-engineers who have built agents. | BCT.15.1, BCT.8.7, BCT.6.1, BCT.15.3 |
| RM-1.3-EVC | RM.1.3.1 low-mid, RM.1.3.5 high, RM.1.3.7 high, RM.1.3.8 present dominates | Cost-value calculus is rational. Don't just increase perceived value — reduce actual cost via PO-level friction reduction. BCT.5.2 (salience of consequences) to make future value vivid. BCT.10.4 (social reward) for proximal recognition. | BCT.5.2, BCT.10.4, BCT.9.3, BCT.13.2 |
| RM-1.4-Identity | RM.1.4.1 low, RM.1.4.3 present, RM.1.4.5 weak | Identity reframe is essential. PE via BCT.13.2 to reposition agent-building as "domain expertise amplification" not "learning to code." MO via BCT.6.1 from non-engineer agent builders. BCT.13.5 (identity associated with changed behavior) to construct new professional identity. | BCT.13.2, BCT.6.1, BCT.13.5, BCT.13.4 |
| RM-1.5-Intentions | RM.1.5.1 weak, RM.1.5.3 vague, RM.1.5.5 absent | EN via BCT.1.4 (action planning) for specific automation targets. BCT.1.1 (goal setting) for concrete first-agent goals. BCT.1.2 (problem solving) for obstacle planning. | BCT.1.4, BCT.1.1, BCT.1.2, BCT.7.1 |
| AM-2.1-Habit | AM.2.1.1 high for manual, AM.2.1.5 high, AM.2.1.7 strong | Manual workflow habits are deeply entrenched. ER via BCT.12.1 to disrupt cue-response chains (e.g., when a ticket comes in, the cue now triggers agent assignment, not manual processing). BCT.8.2 (behavior substitution) for specific workflow steps. Exploit natural disruption windows (tool migrations, reorgs). | BCT.12.1, BCT.8.2, BCT.8.3, BCT.7.1 |
| AM-2.3-Affect | AM.2.3.1 aversive for many, AM.2.3.3 strong dread, AM.2.3.5 high | Fear and anxiety are real and should not be dismissed. BCT.11.2 (reduce negative emotions) via safe experimentation. BCT.13.2 (framing/reframing) to reinterpret uncertainty as learning. BCT.3.3 (emotional support) through peer communities. | BCT.11.2, BCT.13.2, BCT.3.3, BCT.7.7 |
| AM-2.4-Helplessness | AM.2.4.1 low-mid, AM.2.4.3 present, AM.2.4.7 prolonged for some | Prior automation failures have created learned helplessness. BCT.4.3 (re-attribution) to distinguish current AI agents from prior failures. BCT.8.7 (graded tasks) for small, undeniable successes. BCT.2.2 (feedback on behavior) to make effort-outcome link visible again. | BCT.4.3, BCT.8.7, BCT.2.2, BCT.15.3 |

**Narrative synthesis:** The motivation landscape is complex because it combines rational barriers with emotional and habitual ones. The rational barriers (RM-1.3-EVC: the effort isn't worth the uncertain payoff) are downstream of opportunity problems and should be addressed through structural change, not persuasion. The emotional barriers (AM-2.3: fear and anxiety; RM-1.4: identity threat) require genuine psychological work — reframing, safe experiences, peer modeling. The habitual barriers (AM-2.1: entrenched manual workflows) require environmental disruption, not willpower.

The deepest motivational insight is the interaction between identity (RM-1.4) and efficacy (RM-1.2). For non-engineers, building AI agents is both "not who I am" (identity incongruence) and "not something I can do" (low efficacy). These reinforce each other: low efficacy confirms the identity belief ("I'm not a technical person, and my failure proves it"), and identity incongruence reduces effort ("Why would I invest in something that's not my job?"). Breaking this loop requires modeling from non-engineers who have succeeded (addresses both identity and efficacy simultaneously) combined with scaffolded wins (addresses efficacy through mastery experience).

**What to try:** Identity reframing (PE) combined with mastery experiences (EN, TR). Model successful non-engineer agent builders (MO). Build peer communities for emotional support (EN). Use environmental disruption to break manual habits (ER). Protect autonomous motivation where it exists.

**What not to try:** Mandates, compliance-based approaches, or "AI literacy" certification programs that feel like homework. These deepen controlled motivation (RM-1.1) without building efficacy (RM-1.2) or resolving identity tension (RM-1.4). Also avoid dismissing fear and anxiety as "resistance to change" — the emotions are signals about real structural problems.

---

## 3. Cross-Lens Interactions

### Tensions

- **Capability vs. Opportunity (Time):** Teams need hands-on practice to build capability (PC-1.1, PC-1.7), but they don't have the time for practice (PO-2.1). Training programs that require significant time investment will fail. The resolution: embed learning into real work, not separate training sessions.
- **Incentives vs. Identity:** Organizations incentivize agent-building (SO-4) but the behavior threatens professional identity (RM-1.4). Incentives push toward a behavior that feels alien. The resolution: redefine what the behavior means (identity reframe) before pushing harder on incentives.
- **Governance vs. Experimentation:** Organizations want governance for agent behavior (SO-7) but governance restrictions block the experimentation needed to learn what governance should look like (SO-6.5). The resolution: staged governance that starts permissive and tightens with experience, not comprehensive governance imposed upfront.
- **Norm inconsistency vs. Efficacy:** Leaders say "use AI" (SO.1.2) but don't change the operating reality (SO.1.4). Teams that try and face structural barriers lose efficacy (RM-1.2). The say-do gap actively damages motivation. The resolution: change the operating reality before amplifying the message.

### Reinforcements

- **Infrastructure and Capability reinforce each other:** Better tooling (PO-5) makes learning easier (PC-1.7), and more capable teams create demand for better tooling. This is a virtuous cycle once started.
- **Efficacy and Habit reinforce each other:** Successful agent-building experiences (RM-1.2) create new routines (AM-2.1) that displace manual habits. Each successful automation makes the next one easier and more motivating.
- **Shared understanding and Governance reinforce each other:** Common language and standards (PC-1.6) make governance more effective (SO-7), and good governance creates shared understanding of expectations.

### Prerequisites

1. **PO-2 (Resource) gates everything:** Without protected time and budget, no other intervention works. This must be addressed first or simultaneously with everything else.
2. **SO-2 (Roles) gates capability-building:** Until ownership is clear, teams don't know who should be learning what.
3. **PC-1.2 (Mental models) gates PC-1.3 (Judgment):** You can't judge which workflows to automate if you don't understand how agents work.
4. **SO-6 (Safety) gates SO-7 (Governance):** If experimentation is punished, governance can't evolve with practice.
5. **RM-1.2 (Efficacy) gates RM-1.5 (Intentions):** Teams that don't believe they can succeed won't form specific plans.

### Highest Leverage

1. **Scaffolded first-agent wins for non-engineering teams** (addresses PC-1.7, RM-1.2, RM-1.4, AM-2.4 simultaneously): A successful first agent, built with support, corrects mental models, builds efficacy, challenges identity assumptions, and disproves learned helplessness — all at once.
2. **Protected time + role clarity** (addresses PO-2, SO-2, SO-4 simultaneously): Giving teams explicit permission and time to build agents, with clear ownership, resolves the resource barrier, the role ambiguity, and the incentive misalignment in one structural move.
3. **Visible non-engineer agent builders as models** (addresses SO-1, RM-1.4, RM-1.2, AM-2.3 simultaneously): Internal examples of non-engineers building agents shift norms, reframe identity, build vicarious efficacy, and reduce fear — all through a single intervention type.

---

## 4. BCW Function Ranking

| Rank | Function | Rationale | Top 3 BCTs |
|------|----------|-----------|------------|
| 1 | **EN — Enablement** | The broadest and most foundational function for this situation. Enablement removes barriers beyond education/training — exactly what's needed when structural barriers (PO-2, PO-5, SO-2) are the top blockers. Enablement via scaffolding (PC-1.7), resource protection (PO-2), tooling improvement (PO-5), and social support addresses the most dimensions simultaneously. It is a prerequisite for other functions to work. | BCT.8.7 Graded tasks (scaffolded agent-building), BCT.3.2 Social support practical (pairing with experienced builders), BCT.12.5 Adding objects to environment (templates, monitoring dashboards, reference architectures) |
| 2 | **ER — Environmental Restructuring** | The opportunity landscape is dominated by structural barriers that require restructuring: role ambiguity (SO-2), incentive misalignment (SO-4), governance gaps (SO-7), workflow friction (PO-3), and missing monitoring (PO-7). These cannot be addressed through individual-level interventions. ER changes the conditions under which teams operate. | BCT.12.2 Restructuring social environment (role definitions, incentive realignment, governance frameworks), BCT.12.1 Restructuring physical environment (agent platforms, monitoring infrastructure, workflow tooling), BCT.7.1 Prompts/cues (embedding agent-building triggers into existing workflows) |
| 3 | **MO — Modelling** | With norm gaps (SO-1.1), identity barriers (RM-1.4), and efficacy gaps (RM-1.2), modeling from relatable peers is the most efficient intervention. Seeing a fellow operations manager build a working agent simultaneously shifts norms, identity, and efficacy. Modeling is especially important because abstract arguments about AI value don't work — people need to see peers succeeding. | BCT.6.1 Demonstration of behavior (internal showcases of non-engineer agent builders), BCT.6.3 Information about others' approval (signaling that agent-building is valued and normalized), BCT.9.1 Credible source (respected internal leaders demonstrating commitment through action, not just words) |
| 4 | **TR — Training** | Genuine capability gaps exist (PC-1.1, PC-1.3) that require skill-building. But training must be hands-on, embedded in real work, and scaffolded — not lecture-based or time-intensive. Training is ranked 4th because it depends on EN and ER being in place first: training without time (PO-2), without tools (PO-5), and without clear roles (SO-2) is wasted. | BCT.8.1 Behavioral practice/rehearsal (building real agents for real workflows), BCT.4.4 Behavioral experiments (testing hypotheses about agent behavior to build mental models), BCT.6.1 Demonstration (expert-guided walkthroughs of agent design and debugging) |
| 5 | **PE — Persuasion** | Identity reframing (RM-1.4), efficacy support (RM-1.2), and emotional management (AM-2.3) require persuasion. But persuasion without structural change is hollow — "believe you can do it" in an environment that makes it impossible is counterproductive. PE is effective after EN and ER have created conditions for success. | BCT.13.2 Framing/reframing (agent-building as "domain expertise amplification"), BCT.15.1 Verbal persuasion about capability (from relatable successful peers), BCT.4.3 Re-attribution (distinguishing current AI agents from prior failed automation) |

**Contraindicated:**

- **COE — Coercion:** Mandating agent adoption deepens controlled motivation (RM-1.1) and exacerbates identity conflict (RM-1.4). Organizations that make agent-building mandatory without addressing opportunity and capability barriers will get compliance theater — installed tools, attended trainings, no production agents.
- **INC — Incentivisation (as standalone):** Adding bonuses or recognition for agent-building on top of misaligned base incentives (SO-4.1) creates perverse dynamics: people build demo agents to claim incentives without creating real operational value. Incentives should only be introduced after ER has realigned the base reward structure.

---

## 5. Intervention Implications

### EN — Enablement (Rank 1)

**What it looks like in practice:**

- **Agent Starter Kits** (BCT.12.5, BCT.8.7): Pre-built templates for common automation patterns (triage routing, status updates, database operations). Each template is a graded task — start with a simple agent, add complexity incrementally. Templates include monitoring dashboards so teams can see agent performance from day one.
- **Agent-Building Pairing Program** (BCT.3.2): Match teams building their first agent with experienced builders (not just engineers — operations staff who have successfully built agents). The pair works on a real workflow, not a training exercise.
- **Protected "Agent Sprints"** (PO-2 resource protection): Designated 2-week sprints where teams are explicitly released from operational targets to build and deploy their first agent. Leadership visibly protects this time.
- **Embedded Workflow Analysis Support** (BCT.1.2): Before teams build agents, help them map their workflows in a format that supports automation. Provide lightweight workflow documentation templates that surface the implicit knowledge needed for agent design.

### ER — Environmental Restructuring (Rank 2)

**What it looks like in practice:**

- **Agent Ownership Charters** (BCT.12.2 for SO-2): Define who owns agent development for each team. Establish "Agent Leads" — domain experts (not necessarily engineers) who own the automation roadmap for their team's workflows. Give them explicit authority and accountability.
- **Incentive Realignment** (BCT.12.2 for SO-4): Add "operational leverage" as a performance metric alongside output metrics. Reward teams that build capacity (through agents) as highly as teams that deliver output (through manual effort). Make agent adoption a team-level metric, not an individual one.
- **Adaptive Governance Framework** (BCT.12.2, BCT.4.4 for SO-7): Start with a "sandbox" governance model: any team can deploy agents in sandboxed environments without approval. Graduated governance for production: low-risk agents (internal notifications, status updates) deploy with lightweight review; high-risk agents (customer-facing, financial) require structured approval. Evolve governance based on what teams learn, not theoretical risk frameworks.
- **Agent Monitoring Infrastructure** (BCT.12.1 for PO-7): Build shared monitoring tools that track agent performance, error rates, and output quality. Make monitoring a platform capability, not a per-team responsibility.

### MO — Modelling (Rank 3)

**What it looks like in practice:**

- **Internal Agent Showcases** (BCT.6.1): Monthly sessions where teams demo agents they've built. Prioritize non-engineering teams. Focus on the workflow problem solved, not the technical implementation. Make the format: "Here's the pain → Here's what we built → Here's what it does now."
- **Agent Builder Spotlights** (BCT.6.1, BCT.6.3): Feature non-engineer agent builders in internal communications. "How Sarah in Customer Success Built an Agent That Cut Triage Time by 60%." The message: people like you are doing this.
- **Leadership Modeling** (BCT.6.1, BCT.9.1 for SO-1.4): Leaders don't just endorse agent-building — they use agents themselves, publicly. "I built an agent that summarizes my weekly reports" from a VP carries more normative weight than a mandate.

### TR — Training (Rank 4)

**What it looks like in practice:**

- **Learn-by-Building Cohorts** (BCT.8.1): Small groups (4-6 teams) work through a structured sequence of increasingly complex agent builds over 4-6 weeks. Each week builds on the previous. Real workflows, not toy examples. Each cohort includes cross-functional teams so shared language (PC-1.6) develops naturally.
- **Agent Failure Labs** (BCT.4.4, BCT.2.2 for PC-1.5): Structured sessions where teams intentionally break agents to learn failure modes. "Here's an agent — find the three ways it can fail." Builds mental models (PC-1.2), calibration (PC-1.5), and exception handling (PC-1.1.6) simultaneously.
- **Judgment Workshops** (BCT.8.1, BCT.6.1 for PC-1.3): Case-study sessions: "Here are five workflows. Which should be automated first? Why? What autonomy level?" Expert facilitators share their reasoning process to make tacit judgment explicit.

### PE — Persuasion (Rank 5)

**What it looks like in practice:**

- **Identity Reframing Campaign** (BCT.13.2 for RM-1.4): Position agent-building as the next evolution of domain expertise: "The best support leads don't just handle tickets — they design the systems that handle tickets." Frame automation as empowerment, not replacement.
- **Prior Failure Re-Attribution** (BCT.4.3 for AM-2.4): Explicitly address "we tried AI before and it failed" narratives. "RPA failed because it was brittle rule-based automation applied to dynamic workflows. AI agents are fundamentally different — they understand context, handle variation, and learn from feedback. Here's the proof." Back claims with live demonstrations.
- **Efficacy Messaging from Peers** (BCT.15.1, BCT.15.3): Not "you can do this" from leadership (hollow), but "I did this and here's how" from peers. Focus on past success: "You already designed the workflow logic — that's the hard part. The agent just executes it."

---

# Step 4 — BCW and BCT Reasoning

```text
dimensions = PC.1.1.2 low, PC.1.2.1 low, PC.1.3.4 low, PC.1.5.1 overconfident, PC.1.6.1 low, PC.1.7.1 low, PO.1.2 low, PO.2.1 scarce, PO.5.1 low, PO.7.1 long, SO.1.4 low, SO.2.1 ambiguous, SO.4.1 misaligned, SO.6.5 low-mid, SO.7.5 poor, RM.1.2.1 low, RM.1.4.1 low, AM.2.1.7 strong, AM.2.3.1 aversive, AM.2.4.1 low-mid
tensions   = "O barriers make C interventions impractical" | "SO-4 incentives vs RM-1.4 identity" | "SO-7 governance vs SO-6 experimentation"
leverage   = PC.1.7 (scaffolding), PO.2 (resource protection), SO.2 (role clarity), RM.1.2 (efficacy via mastery), SO.1.4 (norm-practice alignment)
functions  = EN > ER > MO > TR > PE
bcts       = EN→BCT.8.7,BCT.3.2,BCT.12.5 | ER→BCT.12.2,BCT.12.1,BCT.7.1 | MO→BCT.6.1,BCT.6.3,BCT.9.1 | TR→BCT.8.1,BCT.4.4,BCT.6.1 | PE→BCT.13.2,BCT.15.1,BCT.4.3
```

### Detailed BCW-BCT Chains

**EN (Enablement) ← PO-2, PO-5, PC-1.7, RM-1.2:**
Resource scarcity (PO.2.1), poor tooling (PO.5.1), low independence (PC.1.7.1), and low efficacy (RM.1.2.1) all point to enablement as the foundational function. BCT.8.7 (graded tasks) addresses scaffolding needs and efficacy simultaneously — early wins build confidence while building real capability. BCT.3.2 (practical social support) through pairing programs addresses multiple gaps: knowledge transfer, emotional support, and norm-building happen in one intervention. BCT.12.5 (adding objects to environment) through templates and monitoring dashboards reduces activation overhead and embeds feedback loops.

**ER (Environmental Restructuring) ← SO-2, SO-4, SO-7, PO-7:**
Role ambiguity (SO.2.1), incentive misalignment (SO.4.1), governance incoherence (SO.7.5), and missing control loops (PO.7.1) are structural barriers that require environmental change, not individual change. BCT.12.2 (restructuring social environment) is the workhorse: redefine roles, realign incentives, establish governance. BCT.12.1 (restructuring physical environment) applies to platform and monitoring infrastructure. BCT.7.1 (prompts/cues) embeds agent-building triggers into existing workflows so the behavior doesn't require separate activation.

**MO (Modelling) ← SO-1, RM-1.4, RM-1.2, AM-2.3:**
Low descriptive norms (SO.1.1), identity incongruence (RM.1.4.1), low efficacy (RM.1.2.1), and aversive affect (AM.2.3.1) are all efficiently addressed through modeling. BCT.6.1 (demonstration) from relatable non-engineer peers addresses all four simultaneously. BCT.6.3 (information about others' approval) normalizes the behavior. BCT.9.1 (credible source) through respected leaders modeling the behavior resolves the say-do gap (SO.1.4).

**TR (Training) ← PC-1.1, PC-1.2, PC-1.3:**
Genuine knowledge gaps (PC.1.1.2), wrong mental models (PC.1.2.1), and weak judgment (PC.1.3.4) require skill-building through practice. BCT.8.1 (behavioral practice/rehearsal) on real workflows builds procedural fluency. BCT.4.4 (behavioral experiments) surface and correct wrong mental models through direct experience. BCT.6.1 (demonstration) from experts makes tacit judgment visible.

**PE (Persuasion) ← RM-1.4, RM-1.2, AM-2.3, AM-2.4:**
Identity barriers (RM.1.4.1), efficacy gaps (RM.1.2.1), fear (AM.2.3.1), and learned helplessness (AM.2.4.1) require belief and emotional shifts. BCT.13.2 (framing/reframing) repositions agent-building as domain expertise amplification. BCT.15.1 (verbal persuasion about capability) from relatable peers builds efficacy. BCT.4.3 (re-attribution) disconnects current AI agents from prior failed automation attempts.

---

# Step 5 — Recommendations

## Phase A: Summary and Key Insights

### Summary

The transition to Level 3 — "AI as Teammates" — is the hardest jump in the maturity model because it requires organizations to change not just what individuals do, but how teams are structured, resourced, and rewarded. The core dynamic is a three-way lock: teams don't have the time or infrastructure to build agents (opportunity barriers), don't yet have the skills or mental models to build them well (capability barriers), and face rational reasons not to try — from misaligned incentives to identity threat to learned helplessness from prior failed automation attempts (motivation barriers).

The highest-leverage intervention is not training, communication, or mandates. It is structural change: protect time for agent-building, define who owns it, realign incentives to reward operational leverage, build accessible tooling and monitoring infrastructure, and create governance that enables experimentation rather than blocking it. Once the structural conditions support agent-building, scaffold teams into their first successful agents through hands-on pairing with experienced builders, using real workflows — not toy demos. Model success through visible non-engineer agent builders who demonstrate that "people like me" do this. Persuasion and identity reframing become effective only after structural and capability barriers are addressed; before that, they feel hollow.

The progression blocker to Level 4 is governance fragmentation. Organizations that achieve Level 3 in pockets but can't establish shared standards, shared platforms, and adaptive governance across teams will never scale to enterprise-wide AI-native operations. The governance challenge is that it must co-evolve with practice — organizations need enough Level 3 experience to design governance that works, but they need some governance to allow Level 3 experimentation. The resolution is staged governance: start permissive in sandboxes, graduate to structured oversight for production agents, and evolve standards based on what teams learn.

### Key Insights

1. **The biggest barrier is not knowledge — it is structural.** Teams don't fail at agent-building because they don't understand AI. They fail because they don't have time (PO-2), the tools assume engineering skills (PO-5), nobody owns the work (SO-2), and the incentive system rewards manual output over automated leverage (SO-4). Training without structural change produces trained people who still can't act.

2. **Identity threat is the hidden motivation killer.** For non-engineering professionals — the majority of the workforce — "building AI agents" feels like stepping outside their professional identity. "I'm a finance manager, not a developer" is an identity statement, not a skills statement. Reframing agent-building as "amplifying domain expertise" rather than "learning to code" is essential, and the reframe only lands when non-engineer peers model it successfully.

3. **Prior automation failures have created rational skepticism, not irrational resistance.** Organizations that tried and failed at RPA, chatbots, or earlier AI initiatives carry scar tissue. Telling these teams "this time is different" without demonstrating how is counterproductive. The intervention must acknowledge the history and prove the difference through small, visible wins — not assertions.

4. **The governance paradox must be resolved with staged, adaptive governance.** Organizations need governance to scale AI safely, but they need experimentation to know what governance should look like. Imposing comprehensive governance upfront blocks learning; having no governance creates risk. The solution is a sandbox-to-production pathway where governance tightens based on accumulated experience and risk level.

5. **Scaffolded first wins are the single highest-leverage intervention.** A non-engineering team, paired with an experienced builder, building a real agent for a real workflow, in protected time, that actually works in production — this single experience addresses capability (learning by doing), efficacy (I did it), identity (people like me do this), norms (my team does this), and helplessness (this time it worked). No other intervention simultaneously affects as many dimensions.

---

## Phase B: In-Depth Report

### Lens Analysis Detail

#### Capability Findings

The capability landscape reveals six interconnected gaps, ordered by dependency:

**Scaffolding (PC-1.7)** is the entry point. Teams cannot perform independently (PC.1.7.1 low) and require structured support for their first agent builds. Bootstrap accessibility (PC.1.7.8) is low-to-mid — some tools and templates exist but aren't sufficient for non-technical teams. The intervention is scaffolded pairing with graded tasks, not self-serve learning.

**Knowledge (PC-1.1)** is the foundational gap. Declarative understanding is shallow (PC.1.1.1 low-mid) and procedural fluency is absent (PC.1.1.2 low). Teams know what agents are but can't build them. Sequence clarity (PC.1.1.3 low) means there's no established path from "identified workflow" to "deployed agent." Exception handling (PC.1.1.6 very low) means even teams that build agents can't handle the failures. The intervention is practice-based training on real workflows — not lectures, not demos, not certifications.

**Mental Models (PC-1.2)** are systematically wrong. The two dominant models — "agents are magic" and "agents are unreliable" — both lead to bad design decisions. The "agents as deterministic software" model (borrowed from traditional programming) sets expectations for 100% reliability that no probabilistic system can meet. Dynamical understanding (PC.1.2.4 low) means teams treat agents as static deployments rather than evolving systems. The intervention is behavioral experiments (BCT.4.4) — let teams see agents fail in controlled conditions to build accurate mental models.

**Judgment (PC-1.3)** is the overlooked gap. The most common failure mode is not building agents poorly — it's automating the wrong workflows or setting wrong autonomy boundaries. Recognition competence (PC.1.3.4 low) means teams can't distinguish good automation candidates from bad ones. Rule dependence (PC.1.3.5 high) means they want simple criteria ("automate everything routine") that don't capture the real complexity. The intervention is expert-facilitated case analysis with realistic scenarios.

**Metacognition (PC-1.5)** is the "silent killer." Overconfidence after initial success (PC.1.5.1 poor) leads to reduced monitoring, which leads to undetected failures. Teams can't detect when agents are failing silently because agent errors look like plausible outputs. The intervention is structured monitoring habits and "failure labs" that build error-detection capacity before agents are deployed to production.

**Shared Representations (PC-1.6)** become critical at scale. Different teams use "agent" to mean different things (PC.1.6.1 low). Conceptual alignment (PC.1.6.2 low) is absent — engineering and business teams have incompatible mental models of what agents can and should do. "What good looks like" (PC.1.6.8) is undefined. The intervention is shared vocabulary, pattern libraries, and cross-functional cohort programs that build common language through shared experience.

#### Opportunity Findings — Physical

**Infrastructure (PO-1)** gaps are real and non-trivial. Enterprise tool ecosystems are fragmented (PO.1.1 low-mid) with inconsistent API quality. Agent-building tools assume engineering context (PO.1.2 low). Feedback loops on agent performance are weak or absent (PO.1.5). These are not gaps that training closes — they require platform investment.

**Resource scarcity (PO-2)** is the structural foundation of the problem. Time is the scarcest resource (PO.2.1 scarce), slack is absent (PO.2.3 low), competing urgency is constant (PO.2.4 high), and the startup cost for agent-building is high (PO.2.7 high). Any intervention that requires significant time investment from teams will fail unless time is explicitly protected. This makes PO-2 a hard prerequisite for all other interventions.

**Workflow documentation (PO-3)** is the hidden prerequisite. Workflows are complex (PO.3.1 high), span multiple teams and tools (PO.3.2 high), and require substantial effort to document for automation (PO.3.7 high). The implication: agent-building programs need a workflow mapping phase before any building begins.

**Tooling accessibility (PO-5)** is a form of structural exclusion. When agent-building tools require engineering fluency (PO.5.1 low for non-engineers), non-engineering teams are locked out of Level 3 autonomy. The tools themselves fail with cryptic errors (PO.5.4 low) and have steep learning curves (PO.5.6 high burden). The intervention is improved tooling, not just training on existing tools.

**Monitoring (PO-7)** gaps separate demo agents from production agents. Feedback latency is long (PO.7.1), signal fidelity is low (PO.7.2), corrective authority is slow (PO.7.3), and real-world variability exceeds agent design (PO.7.7). The intervention is shared monitoring infrastructure — this should be a platform capability, not a per-team responsibility.

#### Opportunity Findings — Social

**Norms (SO-1)** show a classic say-do gap. Leadership approves of AI adoption (SO.1.2 mid-high) but teams don't see others doing it (SO.1.1 low). The critical dimension is norm consistency (SO.1.4 low) — leaders' words don't match the operating reality. This inconsistency actively damages credibility. The intervention: leaders must change the operating reality (resources, incentives, roles) before amplifying the message.

**Roles (SO-2)** are ambiguous along every dimension. Nobody owns agent development (SO.2.1 ambiguous), decision rights are contested (SO.2.2), role conflict is high (SO.2.5), and accountability doesn't match authority (SO.2.6). The intervention: explicit "Agent Lead" roles with clear authority, cross-functional collaboration models that define who does what.

**Incentives (SO-4)** are misaligned at a structural level. The reward system favors manual output over automated leverage (SO.4.1), short-term targets crowd out long-term investment (SO.4.4), and the penalty for agent failure is disproportionate to the reward for success (SO.4.7). The intervention: add "operational leverage" as a valued metric, reward teams for capacity creation alongside output delivery.

**Safety (SO-6)** is insufficient for the experimentation agents require. Permission to experiment (SO.6.5 low-mid) is constrained by undefined rules (SO.6.7 low) and low iteration culture (SO.6.8 low). The intervention: explicit safe-to-fail zones, sandbox environments, learning-framed goals.

**Governance (SO-7)** is the Level 4 gatekeeper. Local autonomy is constrained (SO.7.1 low), cross-team coordination is weak (SO.7.2), existing policies don't fit AI agents (SO.7.5 poor), and practice variation across teams is high (SO.7.8). The intervention: adaptive governance that starts permissive and evolves with experience — sandbox → graduated review → mature standards.

#### Motivation Findings — Reflective

**Self-determination (RM-1.1)** varies significantly. Where autonomous motivation exists (usually technically curious teams), it is the strongest predictor of adoption. Where motivation is controlled (top-down mandates), it produces compliance without genuine adoption. The intervention: protect autonomous motivation, don't add more controlled motivation.

**Efficacy (RM-1.2)** is the motivational linchpin, especially for non-engineers. Low efficacy belief (RM.1.2.1) prevents even attempting to build agents. Fragile recovery (RM.1.2.3) means early failures are terminal. Weak mastery experiences (RM.1.2.6) mean there's nothing to build confidence on. The intervention: guaranteed early wins through scaffolded, graded tasks with support from experienced builders.

**Cost-value (RM-1.3)** rejection is rational, not irrational. Effort cost is high (RM.1.3.5), opportunity cost is high (RM.1.3.7), and present cost dominates future benefit (RM.1.3.8). The intervention is not persuasion — it's reducing actual cost through better tools, templates, and infrastructure, while making future value vivid through concrete demonstrations.

**Identity (RM-1.4)** barriers are deep and underappreciated. Agent-building feels identity-incongruent for non-engineers (RM.1.4.1 low). Identity conflict between professional survival and organizational benefit (RM.1.4.3) creates paralysis. The intervention: reframe agent-building as domain expertise amplification, modeled by successful non-engineer peers.

**Intentions (RM-1.5)** are vague when they exist at all. Most teams haven't converted "we should use AI" into specific automation plans (RM.1.5.3 vague). The intervention: structured workflow-identification exercises that produce specific, concrete automation targets.

#### Motivation Findings — Automatic

**Habit (AM-2.1)** inertia is powerful. Manual workflows are deeply entrenched (AM.2.1.1 high), run independently of stated goals (AM.2.1.5 high), and strongly compete with new agent-mediated workflows (AM.2.1.7 strong). The intervention: environmental disruption — change the cue-response chain so that incoming workflow triggers route to agents first, with human fallback.

**Affect (AM-2.3)** is turbulent. Fear, anxiety, and shame around AI are real for many non-technical professionals (AM.2.3.1 aversive, AM.2.3.5 high). The intervention: validate emotions rather than dismissing them, create safe spaces for experimentation, and build emotional support through peer communities.

**Helplessness (AM-2.4)** from prior automation failures creates rational skepticism (AM.2.4.1 low-mid) that generalizes across technologies (AM.2.4.3 present). The intervention: acknowledge the history, demonstrate concrete differences through small wins, and make the effort-outcome link visible again.

### Cross-Lens Assessment

The three highest-leverage cross-lens interactions are:

1. **The investment paradox (PO-2 × SO-4 × RM-1.3):** Teams don't have time (PO-2), aren't rewarded (SO-4), and rationally conclude it's not worth the effort (RM-1.3). This three-way interaction creates a stable equilibrium at non-adoption. Breaking it requires simultaneous action on all three: protect time AND realign incentives AND reduce effort cost. Addressing any one alone doesn't shift the equilibrium.

2. **The identity-efficacy loop (RM-1.4 × RM-1.2 × SO-1.1 × MO):** "This isn't who I am" (RM-1.4) reinforces "I can't do this" (RM-1.2), which is confirmed by the absence of peer models (SO-1.1). This loop is efficiently broken by modeling (MO) from identity-congruent peers who have succeeded. One successful non-engineer agent builder modeled visibly addresses identity, efficacy, and norms simultaneously.

3. **The governance-experimentation paradox (SO-7 × SO-6 × PC-1.2):** Organizations need governance to scale (SO-7) but governance blocks the experimentation (SO-6) needed to learn what governance should look like — and teams need experience (PC-1.2 mental models) to inform good governance design. The resolution is temporal staging: start with permissive sandbox governance, accumulate experience, then formalize governance based on what teams have learned.

### BCW and BCT Reasoning

The intervention function priority — EN > ER > MO > TR > PE — reflects the structure of the problem:

**Enablement first** because the most immediate barriers are structural: teams can't act because conditions prevent it, not because they refuse to. EN (BCT.8.7, BCT.3.2, BCT.12.5) directly addresses the conditions: scaffolded tasks reduce the capability barrier, practical support reduces the isolation barrier, and environmental objects (templates, dashboards) reduce the infrastructure barrier.

**Environmental Restructuring second** because the social and physical environment actively discourages adoption. ER (BCT.12.2, BCT.12.1, BCT.7.1) addresses the deepest structural barriers: role definitions, incentive systems, governance frameworks, and physical infrastructure. These are changes to the system, not to individuals.

**Modelling third** because norms, identity, and efficacy are most efficiently shifted by seeing peers succeed. MO (BCT.6.1, BCT.6.3, BCT.9.1) is high-impact per unit of investment: a single visible success story from a non-engineer agent builder cascades across multiple motivational dimensions.

**Training fourth** because genuine capability gaps exist, but training is only effective after EN and ER have created conditions for practice. TR (BCT.8.1, BCT.4.4, BCT.6.1) builds the knowledge, mental models, and judgment needed for production-quality agents — but only when teams have time, tools, and roles that support learning.

**Persuasion fifth** because belief and emotional shifts matter, but they must follow structural change. PE (BCT.13.2, BCT.15.1, BCT.4.3) reframes identity, builds efficacy, and addresses learned helplessness — but these interventions are hollow when the environment still punishes the behavior.

### Framework Observations

This diagnosis surfaces several patterns worth noting:

**The "hardest transition" claim is validated by the COM-B analysis.** Level 3 is genuinely harder than other maturity levels because it requires simultaneous change across all three COM-B branches — capability, opportunity, and motivation — for diverse actor groups (engineers, non-engineers, managers, leadership). Earlier levels (individual tool use) require mostly capability and motivation changes for individuals. Later levels (enterprise-wide operations) require mostly governance and coordination changes at the organizational level. Level 3 sits at the inflection point where individual behavior meets organizational structure.

**The "pockets of success" pattern is a classic SO-7 signal.** Organizations that achieve Level 3 in some teams but can't spread it are exhibiting exactly what the Viable System lens predicts: local units with enough autonomy to succeed locally, but insufficient coordination and governance to produce system-wide coherence. The progression blocker (Behavior B) is fundamentally a governance viability problem.

**The role of non-engineers is the strategic surprise.** Most AI maturity discussions assume engineering teams are the primary actors. This analysis reveals that non-engineers are the bottleneck for Level 3: they hold the domain knowledge needed to identify and design automation, but they face the steepest capability, identity, and tooling barriers. Solving for non-engineer agent-building is the critical path.

**Prior automation failures are the most underestimated barrier.** The learned helplessness from RPA, chatbot, and digital transformation failures is real, rational, and widespread. It doesn't show up in surveys or assessments because people have learned not to say "I don't believe this will work" — they say "sounds great" and don't do it. Interventions that don't explicitly address this history will face invisible resistance.

---

*Analysis framework: COM-B / Behavior Change Wheel / BCT Taxonomy v1 (Michie, van Stralen, West, 2011; Michie et al., 2013). Dimensional sub-lenses adapted for organizational behavioral diagnosis.*
