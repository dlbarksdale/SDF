# What Is the Structured Decision Framework (SDF)?
I built SDF to solve a problem I kept running into: the most consequential decisions I faced were also the ones I was least equipped to make well. Incomplete information, no reliable advisor, and my own judgment clouded by what I wanted the answer to be. I'd evaluate things inconsistently, weigh factors differently depending on the day, and couldn't clearly explain my rationale afterward.
The solution I landed on was structural. Instead of trying to make better decisions in the moment, I built a framework that forces structure before reasoning begins. Hard requirements are defined and enforced before scoring starts. Preferences are weighted explicitly rather than felt implicitly. The AI handles structured reasoning within the constraint space I defined. I own the output and iterate the rules when the prior version breaks.
The result is a single, unambiguous decision with documented rationale every time — regardless of the domain, the complexity of the inputs, or how much I want a particular outcome to win.

-

**A note on AI access:**

Running SDF effectively requires access to a large language model. Claude, GPT, and Gemini all work — SDF has been validated across all three. Free tiers are available for all of them and are sufficient for occasional use, but they come with limitations: reduced context windows, daily message caps, and memory constraints that can affect longer or more complex evaluations. For consistent, uninterrupted use — especially if you're running JAF regularly against an active job pipeline — a paid subscription to at least one of these platforms is recommended.

Current paid options as of this writing: Claude Pro, ChatGPT Plus, and Gemini Advanced. Pricing and tier features change — check each platform directly for current details.

Ideally SDF would run on a purpose-built model trained specifically on the framework's logic, constraint architecture, and decision methodology. If the resources to build that existed, that's exactly what this would be. For now, general-purpose LLMs with the right constraint architecture applied on top produce consistent, reliable results — which is the whole point of building the framework the way it was built.

You don't need all three models. Pick one you're comfortable with and use it consistently. The framework works the same way regardless of which model is underneath it.

# The Problem SDF Solves
Most decision processes fail the same way: they treat hard requirements and preferences as equivalent, allow strong scores to rescue failed constraints, and produce outputs that change based on how the question was framed. That's not a decision framework — it's rationalization with extra steps.
SDF is built on a different premise. Hard requirements and preferences are architecturally separated and scored differently. A preference bonus can never compensate for a failed hard requirement. The constraint space is defined before reasoning begins and held constant through evaluation. Every output is traceable to the rules that produced it.
I've applied this across multiple decision domains. The architecture works the same way regardless of what's being decided because the failure mode it addresses — inconsistent inputs, emotional override, untraceable rationale — is structural, not situational.

# How SDF Works
SDF operates in a defined sequence. Each stage gates the next. There is no skipping, no reordering, and no adjusting rules mid-evaluation to accommodate a preferred outcome.
Pre-Stage: Investment Classification
Before any analysis begins, the decision is classified by the level of investment it justifies. Not every decision warrants the same depth of evaluation — spending maximum effort on a low-stakes input wastes resources, and spending minimum effort on a high-stakes input produces unreliable outputs.
Three investment tiers:
Standard — Full analytical sequence runs. No supplementary preparation or custom output work. Applied when the input is common, the stakes are moderate, and differentiation at the evaluation level is marginal.
Full — Complete analysis including tactical output guidance. Applied when the input source has meaningful signal value, the output ceiling represents a real improvement over the current baseline, or supplementary output materially improves the probability of a favorable result.
Elite — Maximum investment. Custom output preparation built from the base template with targeted adjustments. All analytical sections run in full. Applied when the input is rare, the output ceiling is career-defining, or a named gap exists that targeted framing could honestly close.
Hard rules: Investment tier is classified before analysis begins and documented. Tier can be upgraded mid-analysis if the input proves more valuable than initially assessed. Tier cannot be downgraded to skip uncomfortable gap analysis. Custom output work is Elite tier only.

# Stage 1: Hard-Gate Classification
Before any scoring occurs, every input is evaluated against classification rules in priority order. Classification determines the evaluation lens. Every input must be assigned to exactly one category before proceeding.
Classification follows three tiers in sequence:
Tier 1 — Hard Rules: Certain input characteristics trigger automatic classification regardless of other signals. These are defined before the framework runs. An input matching a Tier 1 rule is classified immediately.
Tier 2 — Signal-Based Routing: Inputs that don't match a Tier 1 rule are evaluated against defined signals. Signal presence or absence routes the input to the appropriate category.
Tier 3 — Content Evaluation: Inputs that don't match Tier 1 or Tier 2 rules are classified based on direct content evaluation against category definitions.
Once classified, the evaluation lens is bound to that category. It does not change mid-analysis to accommodate a preferred outcome.
Hard gates within classification are binary — pass or fail. An input that fails a hard gate is eliminated from consideration immediately regardless of how well it would score on everything else. Hard gates represent non-negotiable requirements defined by the human before the framework runs. They cannot be overridden by scoring logic.

# Stage 2: Weighted Scoring
Inputs that clear classification enter the weighted scoring phase. Two types of requirements are evaluated — they are architecturally separated and scored differently by design.
Hard requirements carry full weight. A failed hard requirement is a significant deduction. Multiple failed hard requirements can trigger DO NOT PROCEED regardless of performance elsewhere.
Preferred requirements follow a two-sided rule:

Absence — 0.25x weight maximum. Does not meaningfully hurt the score.
Presence — scoring bonus of 0.25–0.5 per strong match, up to 1.0 maximum added on top of the hard requirement baseline.

Hard guardrail: Preferred requirement bonuses can never compensate for hard requirement failures. A weak hard requirement score cannot be rescued by preferred requirement coverage. Ever.
Evidence Ceiling:
Every input to the scoring process must be traceable to evidenced capability. The evidence base is defined before scoring begins and represents the ceiling of what can be claimed. Scoring cannot reward capabilities that are not evidenced. The framework does not inflate — it evaluates what exists.
Gap Ramp Time Estimation:
Gaps are not binary. A gap closeable in three days before first contact is fundamentally different from a gap requiring six months of project work. Every gap is evaluated against a four-tier ramp time classification:




# Stage 3: Risk Tiering
Scored inputs are classified into risk tiers based on weighted score and risk-relevant signals identified during scoring.
Three risk levels:
Low — Capable now. Evaluation interactions are safe. No meaningful pressure points.
Medium — Capable with some ramp. Specific pressure points exist and are named explicitly.
High — Will be exposed. Domain, capability, or scope mismatch.
Hard disqualifiers that trigger High automatically:

Required scope conflicts with defined constraint preferences
Mandatory evaluation screens that cannot be passed with current capability
Explicitly required capability with no evidenced equivalent and no realistic closing timeline
Entire domain outside competency with no adjacent bridge

Scope Realism Rule: Evaluate what something actually requires, not what it is labeled. Labels are surface signals. Scope is what matters. The same label can describe fundamentally different levels of responsibility depending on context — and the same level of responsibility can carry different labels depending on who's doing the labeling. Always evaluate the actual requirements described, not the title or category assigned to them.
Each named pressure point includes an evaluation survivability call — one line stating whether the gap is closeable before first contact, requires immediate preparation, creates real exposure, or is a hard stop.

# Stage 4: Human Validation & Output Ownership
The framework produces a recommended decision with full documentation of the rationale — which hard gates were applied, how each input scored across each weighted category, what risk tier was assigned, and why the top recommendation was selected.
The human reviews this output and owns the final decision. The model never makes the call.
Trajectory Impact:
Before finalizing output, every decision is evaluated on what it does to longer-term positioning — not just whether it works now. Each dimension is rated independently:

Positioning elevation — does this strengthen your standing in the target domain?
Baseline movement — does this meaningfully move your floor for the next decision?
Primary domain leverage — does this expand your ability to compete where you're trying to go?
Constraint alignment — does the actual scope keep you aligned with your defined preferences?

Each dimension outputs: Accelerates / Neutral / Conflicts
Purpose: surfaces decisions that are technically passable but strategically wrong — and decisions that are a stretch but worth attempting because of trajectory impact.
Anchoring:
When output involves a negotiable value — compensation, terms, scope — anchor at the top third of the realistic range on strong-fit inputs. The current baseline is the problem to solve, not the reference point to protect. Let the other side say no to a high anchor rather than preemptively discounting.
Classification rules, weight assignments, and risk tier definitions are iterated by the human based on where prior outputs fell short. This is the human-in-the-loop design: AI handles structured reasoning and scoring within defined constraints. Human judgment owns classification decisions, rule iteration, and final output validation.   What Makes SDF Different
Most decision processes — with or without AI — fail the same way. They start with options and work backward to criteria, which means the criteria get shaped by the options already under consideration. Preferred outcomes contaminate the evaluation before it begins. SDF inverts this entirely. Criteria, constraints, and weights are defined and locked before any option is evaluated. The framework cannot be reverse-engineered toward a preferred answer once it's running.

Second difference: SDF separates hard requirements from preferences architecturally, not just conceptually. Most weighted scoring systems treat everything as a preference with different weights. SDF eliminates hard requirement failures before scoring begins. A high preference score has no mechanism to rescue a failed hard requirement — they operate in different stages and never interact.

Third difference: gaps are evaluated against closing timeline, not just presence or absence. A gap you can close in three days before first contact is not the same as a gap requiring six months of sustained work. SDF accounts for this in scoring rather than treating all gaps as equivalent deficiencies.

Fourth difference: every decision is evaluated on trajectory impact — what it does to longer-term positioning — not just immediate fit. Technically passable decisions that conflict with where you're trying to go get surfaced and flagged rather than passing through on score alone.

Fifth difference: the framework is model-agnostic. The constraint architecture enforces consistency regardless of which AI model is running underneath it. Output consistency is a property of the framework, not the model. Validated across Claude Sonnet 4.6, GPT-4, and Gemini — the architecture holds across all three. Where model behavior varied, the constraint layer absorbed the variance and produced consistent outputs. That's the point.

None of these differences are subtle. They are architectural decisions made deliberately to address specific failure modes identified through iteration. Each version of SDF exists because the prior version broke somewhere. The version history is the evidence.


# Design Principles

Constraints before reasoning.
The framework defines the boundaries of valid reasoning before evaluation begins. Criteria, weights, and hard requirements are locked before any option is considered. The framework cannot be reverse-engineered toward a preferred outcome once it's running.

Hard requirements are not preferences.
A system that allows high scores to compensate for failed requirements is not a decision framework — it's a rationalization engine. Hard requirements and preferences operate in different stages and never interact. A failed hard requirement cannot be rescued by preference performance. Ever.

Evidence is the ceiling.
Every input to the scoring process must be traceable to evidenced capability or verified fact. The evidence base is defined before scoring begins. The framework does not inflate, project, or extrapolate. It evaluates what exists and cannot reward what doesn't.

Gaps have timelines, not just presence.
A gap closeable before first contact is not the same as a gap requiring months of sustained work. Gaps are evaluated against their closing timeline — not just whether they exist. Scoring calibrates accordingly.

Investment matches stakes.
Not every decision justifies maximum analytical effort. The framework classifies investment level before analysis begins — standard for common inputs, full for high-value inputs, maximum for rare or high-consequence inputs where the output materially changes your trajectory. Spending elite-tier effort on a low-stakes decision wastes resources. Spending standard-tier effort on a high-stakes decision produces unreliable outputs.

Scope over label.
Evaluate what something actually requires, not what it is called. Labels are surface signals. Scope is what matters. The same label can describe fundamentally different levels of responsibility depending on context.

Trajectory over immediacy.
Every decision is evaluated on what it does to longer-term positioning, not just whether it works now. A technically passable decision that conflicts with where you're trying to go is flagged — not passed through on score alone.

Every output is traceable.
The rationale behind every recommendation is documented in full. Which hard gates were applied, how each input scored, what risk tier was assigned, and why the top recommendation was selected. There are no black box outputs.

The human owns the decision.
SDF is a reasoning tool, not a decision-maker. Human judgment defines the rules, validates the output, and iterates the framework. The model executes structured reasoning within constraints the human set. The human makes the call.

Failure modes are assets.
Every version of SDF exists because the prior version broke somewhere. Finding where it breaks and fixing the architecture is the development process. The version history is the evidence.

# Version History

SDF follows a deliberate versioning philosophy. Each version increment reflects a specific failure mode identified in the prior logic and the architectural fix introduced to address it. The version history is a regression record, not a feature log.

- v1.0 — Initial Architecture
Established the core four-stage structure: hard-gate classification, weighted scoring, risk tiering, human validation. First working implementation of constraint-first reasoning with AI as the structured reasoning layer.
Failure mode identified: Hard gates and preferences were not cleanly separated — high preference scores were partially compensating for borderline hard gate performance. The boundary between non-negotiable requirements and weighted preferences existed conceptually but was not enforced architecturally.

- v1.5 — Hard Gate Enforcement
Introduced strict binary enforcement of hard gates with zero tolerance for score compensation. Any input failing a hard gate is eliminated before entering the scoring phase regardless of projected preference performance.
Failure mode identified: Weight assignments were subjective and inconsistent across evaluations — the same preference carried different implicit weight depending on how the input was framed to the model.

- v2.0 — Explicit Weight Architecture
Formalized weight assignment as a human-defined input declared before the framework runs. Weights held constant across all inputs in a given evaluation set. The model no longer determines what matters — the human does, in advance.
Failure mode identified: Risk tiering was producing misleading confidence signals. High overall scores were masking significant weakness in specific categories.

- v2.1 — Risk Flag Surfacing
Introduced explicit risk flag identification at the category level. Weaknesses are surfaced in the output regardless of overall score, preventing high aggregate performance from obscuring material gaps.
Failure mode identified: Output documentation was inconsistent — rationale quality varied based on model behavior rather than following a defined structure.  

- v2.3 — Model-Agnostic Validation
Validated framework behavior across Claude, GPT-4, and Gemini. Constraint architecture confirmed model-agnostic — consistent outputs regardless of underlying model. Where model behavior varied, the constraint layer absorbed the variance and produced consistent outputs.
Failure mode identified: Gap penalties were applied uniformly regardless of whether the gap was realistically closeable within the evaluation timeline. A gap closeable in three days was penalized identically to a gap requiring six months of sustained work.

- v2.4 — Gap Ramp Time Estimation
Introduced gap ramp time estimation as a required component of scoring analysis. Four tiers: Days, Weeks, Months, Different Domain. Gap score penalty calibrated to realistic closing timeline rather than binary presence or absence. Days and Weeks ramp gaps carry reduced penalty reflecting their closeability within a standard evaluation cycle. Months gaps carry standard penalty with a mandatory roadmap note. Different Domain gaps carry full hard gap penalty.
Failure mode identified: The preferred requirement rule was asymmetric — it correctly avoided penalizing absences but did not reward presence. Strong preferred matches were being undervalued and had no mechanism to add positive signal to the output.

- v2.5 — Two-Sided Preferred Scoring
Expanded preferred requirement scoring to two-sided. Absence remains at 0.25x weight maximum — no penalty. Presence now scores as a bonus of 0.25–0.5 per strong match, up to 1.0 maximum, added on top of the hard requirement baseline. Hard guardrail added: preferred bonuses cannot compensate for hard requirement failures.
Failure mode identified: All inputs were receiving the same depth of analytical investment regardless of their consequence magnitude or rarity — high-stakes inputs were being evaluated with the same effort as routine ones, producing unreliable outputs on decisions that mattered most.

- v2.6 — Investment Tier Classification & Evaluator Probability Statement
Introduced formal investment tier classification before analysis begins. Three tiers — Standard, Full, and Elite — calibrate analytical depth to the consequence magnitude and rarity of the input. Standard for common inputs. Full for high-value inputs. Elite for rare or high-consequence inputs where the output materially changes trajectory. Investment tier is documented before analysis begins, can be upgraded mid-analysis, and cannot be downgraded to skip uncomfortable gap analysis. Added Evaluator Probability Statement immediately following fit score — written from the evaluator's perspective assessing likelihood of a favorable result based on output match, competitive pool, visible differentiators, and visible gaps.
Failure mode identified: High-consequence inputs were receiving consistent analytical outputs but the framework had no mechanism to verify that the strongest relevant credentials were explicitly surfaced rather than implied — elite inputs were being submitted without confirming the output template was optimally positioned for the specific evaluation context.

- v2.7 — Within-Category Emphasis Check & Evidence Library
Added Within-Category Emphasis Check for Elite tier evaluations. Runs after investment classification and before scoring. Identifies the two to three signals the evaluator will look for first, determines whether those signals are explicitly present or only implied in the output template, and flags what needs surfacing through targeted addition or reorder. Added Evidence Library as a canonical reference that defines the ceiling of what can be claimed during evaluation. Source documents define actual scope of evidenced capability. Framing guidance derived from evidence sources must remain truthful to actual capability performed. Does not authorize adding unevidenced capabilities regardless of what scoring would reward.
Current stable version.

# Current Status
SDF is at v2.7 — current stable version. The framework is actively running in production on real decisions. A fully implemented domain-specific application of SDF — the Job Analysis Framework — has been developed and iterated in parallel, currently at JAF v2.7. JAF demonstrates what SDF looks like when fully implemented against a specific decision domain: complete routing logic, evidence library, investment tiering, gap analysis, risk assessment, trajectory evaluation, and documented output. It serves as the reference implementation for anyone building a domain-specific SDF application.

Full open-source documentation of the framework logic, classification rule templates, weight assignment structure, and output documentation format is in progress. Code implementation is in development.   Contact doshuabarksdalework@gmail.com
