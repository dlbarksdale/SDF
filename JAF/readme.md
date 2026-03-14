# Job Analysis Framework (JAF)

### A Domain-Specific Implementation of the Structured Decision Framework (SDF)


---
**Think LinkedIn skills match — but actually useful.**

LinkedIn recommends roles based on keyword overlap. Indeed matches on similar logic with less precision. ClearanceJobs has the strongest platform-native matching of the three — but it requires an active clearance and only surfaces cleared or contractor roles. All three share the same fundamental limitation: they match what your resume says against what a job posting says, with no understanding of domain depth, career trajectory, compensation positioning, or whether the role actually fits where you're trying to go.

JAF does what none of them do. It doesn't match keywords — it evaluates fit. It accounts for what you can actually defend in an interview, what the role is worth relative to your baseline, what accepting it does to your positioning two years from now, and whether the effort of applying is justified by the quality of the opportunity. It produces a verdict, not a percentage.

You can use all three platforms to find opportunities. Use JAF to decide which ones are actually worth your time.

# What Is JAF

JAF is a fully built application of SDF applied to a single, high-stakes, recurring decision: should I apply to this job, and if so, how much effort does it deserve?

Most people evaluate job opportunities inconsistently. They apply to roles they can't defend in an interview, undersell themselves in compensation negotiations, send the wrong resume to the wrong audience, and spend the same amount of preparation energy on a long-shot application as they do on a role they're genuinely built for. JAF fixes that by running every opportunity through the same structured sequence every time — investment classification, hard-gate routing, weighted scoring, risk assessment, compensation anchoring, trajectory evaluation, and a binary verdict with no ambiguity.

The output is not a feeling about whether to apply. It is a documented, traceable decision with rationale that can be reviewed, explained, and improved.

---

## How JAF Relates To SDF

SDF is the general framework. JAF is one implementation of it.

SDF's architecture — investment classification, hard-gate classification, weighted scoring, risk tiering, and human validation — applies to any complex multi-variable decision. JAF takes that architecture and builds a complete decision system around the specific domain of job opportunity evaluation. The routing logic, category definitions, evidence library, submission tiering, and verdict framework are all JAF-specific constructs built on top of SDF's core principles.

If you want to understand why JAF works the way it does, read the SDF documentation first. If you want to run JAF on a job opportunity, this document is all you need.

---

## What JAF Produces

For every opportunity evaluated, JAF produces:

- Category classification and resume assignment
- Submission tier — Volume, Value, or Vanguard
- Skills match analysis with gap ramp time and interview survivability
- Technical risk assessment with named pressure points
- Compensation band, realistic placement, and a single anchor number
- Location and constraint justification
- Trajectory impact across five dimensions
- A binary verdict — APPLY or DO NOT APPLY — with no hedging

---

## The Category System

The category system is the most important and most configurable part of JAF. Before you run a single analysis, you need to define your categories. Everything else in the framework flows from this decision.

The core principle is simple: distinct targets deserve distinct positioning. A resume optimized for one audience is rarely optimized for another. If you are targeting two meaningfully different roles or industries, you should have two meaningfully different resumes — each one telling the right story to the right room. The category system enforces that discipline. It prevents you from sending the wrong story to the wrong audience, and it prevents you from running the wrong analysis on a role that belongs in a different lane.

JAF ships with four default categories. These are starting points — not requirements. Rename them, delete them, add new ones, or reconfigure them entirely based on your specific targets. The only rules are that every opportunity routes to exactly one category, and every category has exactly one resume assigned to it.

Examples of how configurable this is: if your specialty is embedded firmware, call it Embedded. If you are aspiring to break into software engineering from another field, call it SWE. If you are targeting product management, call it PM. If you only have one target market and one resume, you only need one category. The framework scales to however many lanes you are actually running.

---

### Aspirational

The Aspirational category is for roles in a domain you are actively targeting but have not yet fully broken into. You have transferable experience, adjacent credentials, or an independent project that makes you a credible candidate — but your resume needs to do more translation work than your other categories. This is your highest-ceiling lane and your longest timeline. The resume assigned here leads with your strongest differentiator for that domain, bridges your existing experience toward it explicitly, and doesn't bury the lead.

Use this category when you are targeting a new industry, a new function, or a role type where your background is adjacent rather than direct. The fit score bar is lower here by design — you are reaching, and the framework accounts for that.

Example: a validation engineer targeting AI evaluation roles. A mechanical engineer targeting robotics software. A defense contractor targeting commercial tech.

---

### Technical Specialty

The Technical Specialty category is for roles where you have deep, specific, hard-to-replicate technical credentials that a narrow but well-defined audience will immediately recognize and value. This is your most defensible lane on technical depth. The resume assigned here leads with the specialized work, uses domain-specific vocabulary without translation, and positions you as someone who has done the exact work rather than something adjacent to it. This category is commercial-facing by design — it targets audiences who value the technical depth itself without requiring regulated context to understand it.

Use this category when the role requires specific technical depth — a particular stack, a particular domain, a particular methodology — that you genuinely have and that differentiates you from a generalist candidate pool.

Example: an RF simulation engineer targeting signal processing roles. A firmware engineer targeting embedded systems positions. A systems engineer targeting HW/SW boundary validation roles.

*Note: If your deepest technical credentials exist entirely within a regulated environment — defense, cleared programs, government contracting — your Regulated category may already be functioning as your Technical Specialty. In that case, Technical Specialty should target the commercial translation of that depth rather than duplicating it. The question to ask is: which resume leads with domain-specific technical vocabulary for a commercial audience that wouldn't require regulated context to understand it? That's your Technical Specialty.*

***Another note on discovering your Technical Specialty:***
*Most people underestimate what their specialty actually is. Not because they lack one — but because they've been inside it so long they can't see it from the outside anymore.*
*You might think you're a Software Engineer who knows Python. Your JDs might reveal you're a Financial Systems Engineer who has spent five years validating high-frequency trading infrastructure at scale. You might think you're a Project Manager who runs meetings and tracks deadlines. Your JDs might reveal you're a Technical Program Manager who has been coordinating cross-functional engineering dependencies across multi-million dollar product launches — a fundamentally different profile that commands $40–60K more in the right market than the title you've been selling yourself as. You might think you're a Designer. Your JDs might reveal you're a UX Research Engineer who has been translating user behavior data into product architecture decisions. You might think you're an IT Analyst. Your JDs might reveal you're a Cybersecurity Compliance Engineer who has been maintaining regulatory frameworks that keep the company out of legal exposure.
These are not the same things — and the market does not pay them the same way.*
*Companies are paying for specialists, not generalists. Knowing Python is not a specialty. Knowing how to draw is not a specialty. Being a strong communicator is not a specialty. These are table stakes — expected, assumed, and not what anyone is searching for. Recruiters are not searching for "knows how to code" or "has design skills." They are searching for Kafka Infrastructure Engineers, Aerospace Systems Validation Engineers, Medical Device UX Researchers, and Financial Compliance 
*Architects. The more precisely you can name what you actually do, the more directly you land in the search results of the person trying to hire exactly you.*
*Breadth is valuable. But breadth without a clearly named core is how you become the candidate who is good at everything and gets hired for nothing specific — or worse, gets hired for the wrong thing at the wrong price.*
*The gap between what you think you are and what you actually are is often worth tens of thousands of dollars annually. The JDs you've accumulated over your career are the evidence that closes that gap.*
*This is where an LLM becomes genuinely useful. Take every job description from every role you've held — even the ones that felt routine — and feed them to Claude, GPT, or Gemini with a simple prompt: "Based on these job descriptions, what is my actual technical specialty and how should I position it in the market?" You will be surprised what comes back. Not because the AI knows something you don't — but because it can see the pattern across all your experience simultaneously in a way that's hard to do from inside your own career.*
The push button get banana instinct is real. Most people reduce their own experience to the most surface-level description of what they did every day. The JDs tell the fuller story. Use them.*

---

### Portfolio-Led

The Portfolio-Led category is for roles where an independent project, open-source contribution, or self-directed work product is your strongest differentiator — stronger than your employment history alone. This category exists because some audiences care more about what you have built independently than where you have worked. The resume assigned here leads with the project, frames employment history as supporting evidence, and treats the portfolio work as primary rather than supplementary.

Use this category when you have a project that directly evidences the core capability a target audience is hiring for. The project must be real, documented, and defensible under questioning. This is not a category for listing side projects — it is a category for leading with a work product that changes how your entire profile reads.

Example: an engineer who built an AI decision framework targeting AI evaluation roles. A developer who built and open-sourced a widely used tool targeting developer tools companies. A designer with a strong independent portfolio targeting product design roles.

---

### Regulated

The Regulated category is for roles in industries or environments where compliance, clearance, certification, or regulatory context is a primary hiring signal — not just a background check. This is your most immediately accessible lane if you already operate in a regulated environment, and your most inaccessible lane if you don't. The resume assigned here speaks the language of the regulated environment natively — it doesn't translate or soften the domain-specific vocabulary because the audience expects it.

*Note on security clearance: Some regulated environments — particularly defense, intelligence, and certain government-adjacent industries in the United States — require candidates to hold an active security clearance. Clearance levels in the US range from Confidential to Secret to Top Secret, with additional access designations beyond Top Secret for specific programs. Holding an active clearance is a significant hiring signal in these markets because obtaining one takes time, cost, and government sponsorship — a candidate who already holds one removes a major friction point for the hiring organization. If clearance is not relevant to your target market, remove all clearance references from this section and treat Regulated as applying to your industry's specific compliance or certification requirements instead — healthcare, finance, aviation, and other regulated industries have analogous credentialing signals that serve the same function. If none of your target roles exist in a regulated environment, delete this category entirely.*

Use this category when your target roles exist in an environment where regulatory context, clearance status, or compliance credentials are explicitly required or strongly preferred.

Example: a defense contractor targeting DoD prime contractor roles. A healthcare engineer targeting FDA-regulated medical device companies. A financial engineer targeting roles requiring FINRA licensing.

---

## The Portfolio & Independent Project

If you have an independent project, open-source contribution, or portfolio work on your resume — this section applies to you. If you don't, stop reading and go make one.

*(Just kidding. Sort of.)*

You can just delete this section and move on. But you will be leaving one of the highest-leverage differentiators on the table that this framework has to offer.

A portfolio or independent project cannot hurt a fit score in any category. It either adds value or scores zero. Never negative.

The weight it carries depends entirely on how directly it addresses the stated requirements of the category being evaluated. A project that evidences the core capability a target audience is hiring for scores at full weight as direct experience — it is not a side project, not a nice-to-have, not a differentiator. It is primary evidence. A project adjacent to the category scores as a bonus signal. A project tangentially related scores as a minor positive when it connects to a stated requirement.

For this to work, your project must be framed differently for each category it appears in. A project described in embedded signal processing language for a Technical Specialty application reads completely differently than the same project described in product reliability language for an Aspirational application targeting consumer hardware companies. The project doesn't change. The framing does. Each resume should already reflect this — if it doesn't, fix the resume before running JAF.

Your project does not need to be fully polished, production-ready, or feature-complete to earn interviews. It also doesn't need to be something the world has never seen before — especially as an engineer. The point is not novelty. The point is demonstrating that you have genuine interest outside of work hours and that you apply your skills to real problems on your own initiative. A framework you built to solve a recurring decision problem. A tool you wrote because the existing ones didn't work the way you needed. A system you designed because you were curious whether it could be done better. These are all legitimate. What matters is that it is real, documented well enough that someone can understand what you built and why, and something you can go deep on when asked. An interviewer who finds your project interesting will ask you to walk through it — the problem you identified, the architectural decisions you made, why you iterated the way you did, and what broke along the way. Depth of understanding matters more than polish of execution. Build it, document it, and be prepared to defend every line of it in the room.

---

## The Evidence Library

Your previous employer job descriptions are a gold mine of information that most candidates discard after accepting an offer. They contain the authoritative, employer-written description of the actual work you performed — often with more specificity, stronger framing, and more precise vocabulary than what ended up on your resume. When a gap analysis identifies a credential that may be partially addressed by work you performed but didn't fully capture on your resume, your evidence library is where you go to find out what you can truthfully claim and how to frame it.

The evidence library is not a license to inflate. It defines the ceiling of what can be claimed — not a floor to build from aspirationally. If the source document describes a responsibility you performed at a supporting level, frame accordingly. The library makes explicit what is already evidenced. It never adds what isn't.

Add the original job description for every role on your resume. Keep them on file permanently. A JD you accepted three years ago may contain framing language directly relevant to a role you are applying to today that your current resume bullet doesn't capture as precisely. This is one of the most underutilized assets in any job search — most people throw it away the day they sign the offer letter.

---

## Role Scope Preference

JAF treats role scope preference as a configurable baseline variable — not a fixed assumption. Set it to whatever reflects your actual goal and the framework enforces it accordingly throughout the analysis.

Three options:

**IC Only** — Individual contributor track. Any role requiring people management of engineers is a hard disqualifier regardless of all other fit factors. The framework will output DO NOT APPLY on management scope roles automatically.

**Management Track** — You are actively pursuing people management or leadership scope. IC-only roles that cap your growth are flagged as a Conflicts rating in trajectory impact.

**Agnostic** — Scope preference is not a constraint. The framework does not evaluate management vs IC as a factor in any section. Use this if you genuinely don't have a preference or if both tracks are acceptable.

Set your preference in the baseline variables before running any analysis. It applies across every category and every verdict.

---

## How To Use JAF

JAF ships with a reference profile for a fictional candidate — Brennan Okafor, Shreveport, LA, 3 years experience, Active Secret clearance. Every personal variable in the framework is a placeholder. Before running JAF on a real opportunity, replace all of Brennan's details with your own:

- Current base salary and compensation floors
- Current location and secondary market targets
- Clearance status — or remove clearance references entirely if not applicable
- Role scope preference — IC Only, Management Track, or Agnostic
- Category names and definitions — rename, delete, or add categories to match your actual target lanes
- Resume assignments — one resume per category, no exceptions
- Evidence Library — add your own employer JDs as canonical evidence sources

The framework logic does not change. Only the inputs do.

---

## Current Version

JAF 2.8. Active and in production. See the changelog at the bottom of JAF_2_8.md for the full version history and the failure mode that each version increment resolved.

---
