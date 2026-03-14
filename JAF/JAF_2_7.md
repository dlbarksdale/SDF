# Job Analysis Framework (JAF) v2.7
A Domain-Specific Implementation of the Structured Decision Framework
Reference Profile: Brennan Okafor
Shreveport, LA | Active Secret Clearance | 3 Years Professional Experience | IC Preferred


# What Is JAF
JAF is a fully implemented application of the Structured Decision Framework (SDF) applied to job opportunity evaluation. It takes the core SDF architecture — hard-gate classification, weighted scoring, risk tiering, and human validation — and builds a complete decision system around a specific, high-stakes, recurring decision: should I apply to this role, and if so, how?
JAF produces a binary verdict — APPLY vs DO NOT APPLY — with category placement, resume selection, fit scoring, risk assessment, compensation anchoring, constraint justification, trajectory impact, and tactical application guidance every time it runs.
This document is a template. The reference profile belongs to Brennan Okafor and reflects his specific market, experience level, clearance status, compensation baseline, and target categories. Every variable in this document is configurable. Replace Brennan's details with your own, rename or delete categories that don't apply, add categories for lanes he isn't running, and adjust compensation floors to reflect your market. The framework logic stays the same regardless of who is running it.

# What JAF Prevents
Applying to roles you cannot actually do
Resume fantasy — sending the wrong story to the wrong room
Under-anchoring compensation in negotiation
Wasting evaluation cycles on roles that don't justify the effort
Chasing titles instead of evaluating actual scope and compensation
Violating your own stated role scope preferences


# Baseline Variables
| Variable | Value | Configuration Note |
|---|---|---|
| Current Base Salary | $80,000 | Replace with your actual current base |
| Current Location | Shreveport, LA | Replace with your city and state |
| Clearance | Active Secret | See clearance note in Regulated category. Remove if not applicable. |
| Total Experience | 3 years | Replace with your actual YOE |
| Role Scope Preference | IC Preferred | Options: IC Only / Management Track / Agnostic. Set to whatever applies. IC Only means management scope is a hard disqualifier. Management Track means IC-only scope conflicts with your goal. Agnostic means scope preference is not a hard gate. |
| Regulated Floor | $125,000 | Minimum acceptable compensation for any regulated/cleared role. Set your own floor. |
| Primary Market Floor | $110,000 | Minimum for roles in your current market — Shreveport. Set your own floor. |
| Secondary Market Floor | $115,000 | Minimum for roles requiring relocation to a secondary market — Atlanta. Set your own floor and target city. |
# Section 1 — Category Classification
Every opportunity must be assigned to exactly one category before evaluation begins. Classification determines the evaluation lens and the resume assigned. No mixing. No alternates.
**How Classification Works**

Classification follows a priority order. Check Tier 1 first. If a Tier 1 rule applies, classify immediately and stop. If not, check Tier 2. If no Tier 2 signal applies, evaluate content and route to the appropriate category in Tier 3.

**Tier 1 — Hard Classification Rules**

| Condition | Classification |
|---|---|
| Employer is a recognized prime contractor or major player in your regulated domain | Regulated — always, regardless of other signals |
| Define your own Tier 1 rules here | — |

**Tier 2 — Signal-Based Routing**

| Signal | Classification |
|---|---|
| Role requires or prefers a regulated credential — clearance, certification, license | Regulated |
| Role does not mention regulated credentials OR explicitly states they are not required | Evaluate content → Tier 3 routing |
| Define your own Tier 2 signals here | — |

**Tier 3 — Content-Based Routing**

| Content Signal | Classification |
|---|---|
| Role content aligns with your Portfolio-Led category — the core requirement matches your independent project or work product | Portfolio-Led |
| Role content aligns with your Technical Specialty category — deep specific technical credentials are the primary requirement | Technical Specialty |
| Role content aligns with your Aspirational category — adjacent experience with translation required | Aspirational |
| Role content aligns with your Regulated category and was not caught by Tier 1 or Tier 2 | Regulated |

**Category Definitions & Configuration Guide**

JAF ships with four default categories. These are starting points — not requirements. Rename them, delete them, add new ones, or reconfigure them entirely based on your specific targets. The only rule is that every input must route to exactly one category and each category must have exactly one resume assigned to it.
The point of multiple categories is simple: distinct targets deserve distinct positioning. A resume optimized for one audience is rarely optimized for another. If you're targeting two meaningfully different roles or industries, you should have two meaningfully different resumes. The category system enforces that discipline — it prevents you from sending the wrong story to the wrong room.
Examples of how configurable this is: if your specialty is embedded firmware, call it Embedded. If you're aspiring to break into software engineering from another field, call it SWE. If you're targeting product management, call it PM. If you only have one target market and one resume, you only need one category. The framework scales to however many lanes you're actually running.

**1. Aspirational**

The Aspirational category is for roles in a domain you are actively targeting but have not yet fully broken into. You have transferable experience, adjacent credentials, or an independent project that makes you a credible candidate — but your resume needs to do more translation work than your other categories. This is your highest-ceiling lane and your longest timeline. The resume assigned here leads with your strongest differentiator for that domain, bridges your existing experience toward it explicitly, and doesn't bury the lead.
Use this category when: you're targeting a new industry, a new function, or a role type where your background is adjacent rather than direct. The fit score bar is lower here by design — you're reaching, and the framework accounts for that.
Example: a validation engineer targeting AI evaluation roles. A mechanical engineer targeting robotics software. A defense contractor targeting commercial tech.
Brennan's Aspirational resume: **Aspirational Resume**
Hard rule: This resume only. No exceptions.

**2. Technical Specialty**

The Technical Specialty category is for roles where you have deep, specific, hard-to-replicate technical credentials that a narrow but well-defined audience will immediately recognize and value. This is your most defensible lane on technical depth. The resume assigned here leads with the specialized work, uses domain-specific vocabulary without translation, and positions you as someone who has done the exact work rather than something adjacent to it. This category is commercial-facing by design — it targets audiences who value the technical depth itself without requiring regulated context to understand it.
Use this category when: the role requires specific technical depth — a particular stack, a particular domain, a particular methodology — that you genuinely have and that differentiates you from a generalist candidate pool.
Example: an RF simulation engineer targeting signal processing roles. A firmware engineer targeting embedded systems positions. A systems engineer targeting HW/SW boundary validation roles.
Note: If your deepest technical credentials exist entirely within a regulated environment — defense, cleared programs, government contracting — your Regulated category may already be functioning as your Technical Specialty. In that case, Technical Specialty should target the commercial translation of that depth rather than duplicating it. The question to ask is: which resume leads with domain-specific technical vocabulary for a commercial audience that wouldn't require regulated context to understand it? That's your Technical Specialty.
Brennan's Technical Specialty resume: **Technical Specialty Resume**
Hard rule: This resume only. No exceptions.

**3. Portfolio-Led**

The Portfolio-Led category is for roles where an independent project, open-source contribution, or self-directed work product is your strongest differentiator — stronger than your employment history alone. This category exists because some audiences care more about what you've built independently than where you've worked. The resume assigned here leads with the project, frames employment history as supporting evidence, and treats the portfolio work as primary rather than supplementary.
Use this category when: you have a project that directly evidences the core capability a target audience is hiring for. The project must be real, documented, and defensible under questioning. This is not a category for listing side projects — it's a category for leading with a work product that changes how your entire profile reads.
Example: an engineer who built an AI decision framework targeting AI evaluation roles. A developer who built and open-sourced a widely used tool targeting developer tools companies. A designer with a strong independent portfolio targeting product design roles.
Brennan's Portfolio-Led resume: **Portfolio-Led Resume**
Hard rule: This resume only. No exceptions.

**4. Regulated**

The Regulated category is for roles in industries or environments where compliance, clearance, certification, or regulatory context is a primary hiring signal — not just a background check. This is your most immediately accessible lane if you already operate in a regulated environment, and your most inaccessible lane if you don't. The resume assigned here speaks the language of the regulated environment natively — it doesn't translate or soften the domain-specific vocabulary because the audience expects it.
Note on security clearance: Some regulated environments — particularly defense, intelligence, and certain government-adjacent industries in the United States — require candidates to hold an active security clearance. Clearance levels in the US range from Confidential to Secret to Top Secret, with additional access designations beyond Top Secret for specific programs. Holding an active clearance is a significant hiring signal in these markets because obtaining one takes time, cost, and government sponsorship — a candidate who already holds one removes a major friction point for the hiring organization. If clearance is not relevant to your target market, remove all clearance references from this section and treat Regulated as applying to your industry's specific compliance or certification requirements instead — healthcare, finance, aviation, and other regulated industries have analogous credentialing signals that serve the same function. If none of your target roles exist in a regulated environment, delete this category entirely.*
Use this category when: your target roles exist in an environment where regulatory context, clearance status, or compliance credentials are explicitly required or strongly preferred.
Example: a defense contractor targeting DoD prime contractor roles. A healthcare engineer targeting FDA-regulated medical device companies. A financial engineer targeting roles requiring FINRA licensing.
Brennan's Regulated resume: **Regulated Resume**
Hard rule: This resume only. No exceptions.

# Section 2 — Resume Selection
| Category | Resume | Rule |
|---|---|---|
| Aspirational | [RESUME_NAME] | No exceptions |
| Technical Specialty | [RESUME_NAME] | No exceptions |
| Portfolio-Led | [RESUME_NAME] | No exceptions |
| Regulated | [RESUME_NAME] | No exceptions |

# Section 2.5 — Submission Tier Classification
Runs immediately after category routing and resume assignment. Determines the level of analytical and preparation investment this application justifies. Tier classification is documented before analysis begins. Tier can be upgraded mid-analysis — never downgraded.
Three Tiers
Volume
Standard submission. Base resume assigned per routing rules. Full analytical sections run to produce a defensible verdict. No tactical preparation work. No cover letter guidance. No custom resume.
Apply this tier when:

Employer is at a generic or mid-tier level without strong brand or trajectory value
Compensation band is at or near floor thresholds — strong enough to apply but not strong enough to justify deep investment
Role type is common and the applicant pool is large
This is a volume play — worth submitting because fit is reasonable but not worth slowing the pipeline

Sections run: 1, 2, 2.5, 3, 4, 5, 6, 7, 8. Section 9 skipped.
Value
Full analysis with tactical preparation. Base resume assigned per routing rules. All nine sections run in full including Section 9 with cover letter guidance where the Evaluator Read indicates it is needed.
Apply this tier when any of the following are true:

Employer has meaningful brand value or market recognition above mid-tier
Compensation ceiling is above pipeline average and represents a real floor improvement
Role scope is a strong fit match — fit score expected at 7.5 or above before analysis begins
Role type is less common and the applicant pool is more selective
A cover letter or targeted framing materially improves the probability of a call

Sections run: All nine sections in full order including Section 9.
Vanguard
Elite application. Custom resume built from base resume with targeted edits pulled from the Evidence Library per Section 2.7. Within-Category Emphasis Check run per Section 2.6. All nine sections run in full. Section 9 explicitly references the custom resume variant and the specific framing decisions made. Cover letter treated as required unless Evaluator Read explicitly indicates the resume alone is earning the call.
Apply this tier when any of the following are true:

Employer is a named target or recognized elite brand in your target domain
Compensation ceiling is materially above pipeline average and top placement would be a career-defining reset
Role is rare — low posting frequency, unusual scope match, or a domain actively being pursued as a strategic entry point
Fit score is 8.0 or above and Evaluator Read indicates the resume is already earning the call — custom resume pushes a strong application to the top
A named gap exists that targeted framing could honestly close

Sections run: All nine sections plus Section 2.6 and Section 2.7. Custom resume edits provided as text suggestions in Section 9 before submission.
Hard Rules Across All Tiers

Tier classification documented at the top of every analysis immediately after category and resume assignment
Tier can be upgraded during analysis if a role scores higher than initially assessed
Tier cannot be downgraded to skip uncomfortable gap analysis or risk assessment
Custom resumes are Vanguard only — never built for Volume or Value applications
Custom resume edits are provided as text suggestions. The candidate maintains and stores resulting variants locally

Decision Rule
Apply this test in order. Is the employer elite or the compensation band career-defining? → Vanguard. Is the fit strong and the employer worth a cover letter? → Value. Is this a reasonable fit at a mid-tier employer where the resume alone is the whole play? → Volume.

# Section 2.6 — Within-Category Emphasis Check
Vanguard tier only. Runs after tier classification and before scoring analysis.
Purpose
The routing logic identifies the correct resume. This check identifies whether the assigned resume — or the custom resume being built — is surfacing the strongest credentials in the right order for this specific role's emphasis before submission. The base resume identity does not change. The framing, bullet order, and submission preparation does.
Process
Review the role's hard requirements and identify the two or three signals the hiring manager will look for first. Then answer:

Are those signals explicitly present on the assigned resume or only implied?
Is the strongest credential for this specific role visible in the first third of the resume?
Is there a role-specific bridge between an evidenced credential and a stated requirement that needs to be made explicit rather than left to inference?
Does the Evidence Library contain language from original employer JDs that supports stronger framing of any evidenced credential?

Output Format
Emphasis signals for this role: [two to three role-specific credentials that must be explicitly visible]
Currently explicit on assigned resume: [which of those are already surface-level]
Needs surfacing: [which require a bullet addition, reorder, or cover letter bridge]
Evidence Library pull recommended: [which employer JD contains supporting language and what it adds]
Hard Rule
This check does not authorize adding credentials that cannot be defended under questioning. It only surfaces and makes explicit what is already evidenced. If a required signal is not evidenced it belongs in the gap analysis in Section 3.

# Section 2.7 — Evidence Library
Vanguard tier only. Always available but actively consulted only on Vanguard applications.
Purpose
Your previous employer job descriptions are a gold mine of information that most candidates discard after accepting an offer. They contain the authoritative, employer-written description of the actual work performed — often with more specificity, stronger framing, and more precise vocabulary than what ends up on a resume. When a gap analysis identifies a credential that may be partially addressed by work you performed but didn't fully capture on your resume, the Evidence Library is where you go to find out what you can truthfully claim and how to frame it.
The Evidence Library is not a license to inflate. It defines the ceiling of what can be claimed — not a floor to build from aspirationally. If the source JD describes a responsibility you performed at a supporting level, frame accordingly. The Evidence Library makes explicit what is already evidenced. It never adds what isn't.
What To Include
Add the original job description for every role on your resume. Keep them on file permanently. A JD you accepted three years ago may contain framing language directly relevant to a role you're applying to today that your current resume bullet doesn't capture as precisely.
For each source document, note:

Which role it covers
Which resume category it primarily supports
What credentials it most strongly evidences that may not be fully captured on the current resume

Brennan's Evidence Library
RoleSource DocumentPrimary CategoryKey Evidence[Most Recent Role][JD filename or link][Category][Key credentials evidenced][Prior Role][JD filename or link][Category][Key credentials evidenced][Earlier Role][JD filename or link][Category][Key credentials evidenced]
Replace Brennan's placeholder entries with your own roles and source documents. Every role on your resume should have a corresponding source JD in this library if one exists. If you no longer have access to the original JD, reconstruct it as accurately as possible from memory or LinkedIn — even a partial reconstruction is more useful than nothing.
Per-Category Framing Priorities
For each of your categories, identify which source JDs are the primary evidence anchor:

Aspirational — which JD contains work performed that translates most directly to the aspirational domain even if it wasn't framed that way at the time?
Technical Specialty — which JD contains the most specific and defensible technical depth for your specialty?
Portfolio-Led — which JDs support the employment history that surrounds your portfolio work?
Regulated — which JDs contain regulated domain credentials, clearance context, or compliance-specific work?

Hard Rule
Source JDs define the ceiling of what can be claimed. Framing guidance derived from them must remain truthful to actual scope performed.

# Section 3 — Skills Match Analysis & Fit Score
Evaluate against real, evidenced capability only — not aspirational or rampable learning.
Requirement Weighting
TypeWeightLabel SignalsHard RequirementsFull weight"required," "must have," "basic qualifications," or listed without qualifierPreferred RequirementsTwo-sided rule — see below"preferred," "desired," "a plus," "familiarity," "exposure to"
Preferred Requirement Scoring Rule
Missing a preferred requirement: 0.25x weight maximum. Does not meaningfully hurt score. Do not flag absence.
Having a preferred requirement: Scoring bonus of 0.25–0.5 added on top of the hard requirement baseline. Multiple strong matches add up to 1.0 maximum.
Hard guardrail: Preferred bonuses cannot compensate for hard requirement gaps. A weak hard requirement score cannot be rescued by preferred requirement coverage. Ever.

**Experience Requirement Rules**

| Gap | Impact |
|---|---|
| Met or exceeded | No impact |
| Within 2 years short | No meaningful impact — do not flag |
| 3–5 years short | Minor flag only — never a primary disqualifier |
| 5+ years short | Moderate flag — not a hard stop unless combined with multiple other hard gaps |

Experience requirements are threshold signals — not precise filters. They never trigger DO NOT APPLY on their own.

Gap Ramp Time Estimation
Every gap must include a ramp time estimate and an evaluation survivability call.
Ramp TierDefinitionScore ImpactSurvivabilityDaysCloseable before first contact with minimal effortMinimal — treat near equivalent to partial matchYes — close it before the screenWeeksCloseable within a standard 2–4 week cycle with focused effortSoft partial — small deductionPossibly — prep immediatelyMonthsRequires sustained project work. Cannot be closed within a standard cycleStandard gap penaltyUnlikely without adjacent experienceDifferent DomainYears of specialized experience required. No prep bridges thisFull hard gap penaltyNo
Skills Match Table Format
| Requirement | Match | Ramp Time | Survivability |
|---|---|---|---|
| Example hard requirement met | Strong | — | — |
| Example gap — weeks ramp | Gap | Weeks | Possibly — prep immediately |
| Example gap — months ramp | Gap | Months | Unlikely — roadmap note required |
| Example gap — different domain | Hard Gap | Different Domain | No |

***Months Gap Roadmap Note — Required Format***
For every gap rated Months ramp, include a roadmap note immediately following the gap entry.
Format: [Skill] — Months ramp. Not closeable within a standard hiring cycle. To target this gap intentionally: [specific activity]. Estimated [timeframe] of active effort to speak confidently in a screen. [Similar roles] become viable in [approximate timeframe] with focused effort.

**Portfolio & Project Scoring Rules**
If you have an independent project, open-source contribution, or portfolio work on your resume — this section applies to you. If you don't, stop reading and go make one.
(Just kidding. Sort of.)
You can just delete this section and move on. But you'll be leaving one of the highest-leverage differentiators on the table that this framework has to offer.
A portfolio or independent project cannot hurt a fit score in any category. It either adds value or scores zero. Never negative.
The weight it carries depends entirely on how directly it addresses the stated requirements of the category being evaluated. A project that evidences the core capability a target audience is hiring for scores at full weight as direct experience — it is not a side project, not a nice-to-have, not a differentiator. It is primary evidence. A project adjacent to the category scores as a bonus signal. A project tangentially related scores as a minor positive when it connects to a stated requirement.
For this to work, your project must be framed differently for each category it appears in. A project described in embedded signal processing language for a Technical Specialty application reads completely differently than the same project described in product reliability language for an Aspirational application targeting consumer hardware companies. The project doesn't change. The framing does. Each resume should already reflect this — if it doesn't, fix the resume before running JAF.
Your project does not need to be fully polished, production-ready, or feature-complete to earn interviews. It also doesn't need to be something the world has never seen before — especially as an engineer. The point is not novelty. The point is demonstrating that you have genuine interest outside of work hours and that you apply your skills to real problems on your own initiative. A framework you built to solve a recurring decision problem. A tool you wrote because the existing ones didn't work the way you needed. A system you designed because you were curious whether it could be done better. These are all legitimate. What matters is that it's real, documented well enough that someone can understand what you built and why, and something you can go deep on when asked. An interviewer who finds your project interesting will ask you to walk through it — the problem you identified, the architectural decisions you made, why you iterated the way you did, and what broke along the way. Depth of understanding matters more than polish of execution. Build it, document it, and be prepared to defend every line of it in the room.

**Fit Score & Evaluator Probability Statement**
Output the fit score first. Immediately following, output the Evaluator Probability Statement.
| Output | Format |
|---|---|
| Fit Score | X / 10 |
| Evaluator Read | One to two sentences written as if you are the evaluator reviewing this resume cold against this specific role and applicant pool. Would you call? Why or why not? |

**The Evaluator Read must account for:**
- How well the resume matches stated requirements on paper
- How competitive the applicant pool is likely to be
- Whether any credential is a genuine differentiator that stands out in a stack
- Whether any gap is visible enough to cause a skip before a call is made

If the Evaluator Read indicates the resume alone is not earning the call, Section 9 must explicitly address what the cover letter needs to bridge.

# Section 4 — Technical Risk Assessment
| Level | Definition |
|---|---|
| Low | Capable now. Evaluation interactions are safe. No meaningful pressure points. |
| Medium | Capable with some ramp. Specific pressure points exist and are named. |
| High | Will be exposed. Domain, capability, or scope mismatch. |
Hard Disqualifiers → High Risk

Role scope conflicts with stated role scope preference and preference is set to a hard constraint
Mandatory assessment screens that cannot be passed with current capability
Explicitly required capability with no evidenced equivalent and no realistic closing timeline
Entire domain outside competency with no adjacent bridge

**Scope Realism Rule**
Evaluate what something actually requires, not what it is labeled. Labels are surface signals. Scope is what matters. The same label can describe fundamentally different levels of responsibility depending on context. Always evaluate the actual requirements described.
Pressure Point Format
Each named pressure point must include an evaluation survivability call.
Format: [Skill] — [Ramp tier]. [One sentence on survivability and recommended action.]

# Section 5 — Compensation Positioning
Every analysis must output a band, realistic placement with dollar figures, and a single anchor number.
Case A — Band Listed

State the posted band
State realistic placement within the band with dollar amounts
State one anchor number — aggressive but defensible

Case B — Band Not Listed
Estimate based on scope, employer tier, location, and category. Output estimated band, realistic placement, and anchor.
Anchoring Rule
For any role scoring 7.0 or above, anchor in the top third of the band. The current baseline is the problem to solve, not the reference point to protect. Let them say no to a high anchor rather than preemptively discounting.
Anchor must account for: current base salary, years of experience, any regulated credential as a value-add even when not required by the role, and market positioning for the actual scope of the role.
Rate Conversion
For contract or hourly roles: annualize at 2,080 hours. Subtract 15–20% to account for absence of benefits, PTO, and retirement matching when comparing to salaried equivalent.

# Section 6 — Location & Constraint Justification
If a role introduces a constraint not present in your current situation — relocation, onsite requirement, schedule change — the analysis must explicitly answer: does the output justify accepting that constraint?

| Assessment | Definition |
|---|---|
| Justified | Output clearly covers the constraint friction. Meaningful improvement. |
| Borderline | Output improvement present but constraint creates a real tradeoff worth naming. |
| Not Justified | Output improvement insufficient to justify the constraint. State this clearly. |
| N/A | No new constraint introduced — state compensation delta vs current baseline instead. |

# Section 7 — Trajectory Impact
Every analysis must evaluate what this role does for your longer-term positioning — not just immediate fit. Rate each dimension independently.

| Dimension | Definition |
|---|---|
| Positioning Elevation | Does this role strengthen your standing in the target domain? |
| Baseline Movement | Does this meaningfully move your compensation floor for the next negotiation? |
| Primary Domain Leverage | Does this expand your ability to compete where you're trying to go? |
| Secondary Domain Leverage | Does this strengthen positioning in any secondary target domain? |
| Scope Alignment | Does the actual scope keep you aligned with your stated role scope preference? |

Each dimension outputs: Accelerates / Neutral / Conflicts
Purpose: surfaces roles that are technically passable but strategically wrong — and roles that are a stretch but worth attempting because of trajectory impact.

# Section 8 — Final Verdict
Output exactly one of the following. No ambiguity. No hedging.

| Verdict | Definition |
|---|---|
| APPLY | Strong fit. Low-medium risk. Compensation justified. Go. |
| APPLY (Selective Effort) | Good fit with real constraints — remote ambiguity, one notable gap, conditional factors. |
| APPLY (Stretch but Defensible) | Reach role. Gap is real but framing makes it defensible. High risk acknowledged. |
| DO NOT APPLY | True mismatch — domain, capability, or scope conflict. Hard stop. No encouragement padding. |

Role Scope Rule
If role scope preference is set to IC Only and the role requires people management of engineers — hard disqualifier regardless of all other fit factors. If preference is set to Management Track and the role is IC only — flag as a Conflicts rating in trajectory impact but not a hard disqualifier unless management track is set as a hard gate. If preference is set to Agnostic — scope is not evaluated as a constraint.

# Section 9 — Tactical Application Notes
Required for every APPLY verdict on Value and Vanguard tiers. Skipped for Volume tier.
Format

Keywords to verify are present on the resume — truthfully
Experience that maps conceptually to a required capability even when exact match differs
Framing language that positions existing experience toward role requirements
Do not recommend claiming capabilities that cannot be defended under questioning
If Evaluator Read indicates resume alone is not earning the call — explicitly state what the cover letter must bridge
For Vanguard tier — include custom resume edit suggestions as text with specific bullet additions, removals, or reorders recommended before submission


# Required Output Format
Every JAF analysis must include all sections in order. Volume tier omits Section 9. Vanguard tier includes Sections 2.6 and 2.7 before Section 3.

| # | Section | Key Output | Tier |
|---|---|---|---|
| 1 | Category + Resume | Hard rule applied, routing documented | All |
| 2 | Resume Selection | Resume assigned per hard rule | All |
| 2.5 | Submission Tier | Volume / Value / Vanguard — documented and justified | All |
| 2.6 | Emphasis Check | Emphasis signals, explicit vs implied, Evidence Library pull | Vanguard only |
| 2.7 | Evidence Library | Consulted for framing guidance and custom resume edits | Vanguard only |
| 3 | Skills Match | Four column table with ramp time and survivability | All |
| 4 | Risk Level | Low / Medium / High — pressure points named | All |
| 5 | Compensation | Band + realistic placement + single anchor number | All |
| 6 | Location | Constraint justification — or N/A with comp delta | All |
| 7 | Trajectory | Five dimensions rated | All |
| 8 | Verdict | One of four options, no ambiguity | All |
| 9 | Tactical Notes | Keywords, framing, cover letter, custom resume edits | Value + Vanguard only |

# Changelog
| Version | Changes |
|---|---|
| JAF 2.7 | Added Section 2.5 Submission Tier Classification — three tiers: Volume, Value, Vanguard. Added Section 2.6 Within-Category Emphasis Check — Vanguard only, runs after tier classification and before skills match. Added Section 2.7 Evidence Library — Vanguard only, canonical source documents define ceiling of what can be claimed, previous employer JDs identified as primary evidence source. Anchoring rule formalized in Section 5: anchor in top third of band for roles scoring 7.0+. Section 9 tier-gated: required for Value and Vanguard, skipped for Volume. |
| JAF 2.6 | Added gap ramp time estimation — four tiers: Days, Weeks, Months, Different Domain. Ramp time and survivability added as columns to skills match table. Days and Weeks carry reduced penalty. Months require mandatory roadmap note. Different Domain carries full hard gap penalty. Added Evaluator Probability Statement following fit score. Cover letter guidance in Section 9 triggered when Evaluator Read indicates resume alone is insufficient. |
| JAF 2.5 | Preferred requirement scoring expanded to two-sided. Absence remains 0.25x maximum. Presence adds 0.25–0.5 bonus per strong match up to 1.0 maximum. Hard guardrail added: preferred bonuses cannot compensate for hard requirement gaps. Per-category SDF scoring rules introduced replacing universal rule. |
| JAF 2.4 | Added fourth category with full positioning, target list, identity keywords, and routing logic. Corresponding resume assigned as hard rule. SDF scoring rule formalized. Four-way routing logic table added. |
| JAF 2.3 | Added Section 7 Trajectory Impact — five dimensions. Tactical Application Notes formalized. Hard and preferred requirement weighting formalized. Experience requirement rules codified. Scope realism rule added. Role scope preference confirmed as configurable hard constraint. Rate conversion rule added. Three-tier input classification and signal-based routing formalized. Anchor number required on all APPLY verdicts. |
| JAF 2.2 | Core framework established: category classification, resume hard rules, skills match, risk assessment, compensation positioning, constraint justification, final verdict. |
| JAF 2.1 and prior | Iterative development — category logic, resume selection, compensation anchoring, fit scoring foundations. |

JAF 2.7 — Reference Implementation of the Structured Decision Framework
Reference Profile: Brennan Okafor | Shreveport, LA
Built by and for anyone evaluating job opportunities with more rigor than gut feeling.
