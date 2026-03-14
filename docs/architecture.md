SDF Architecture
SDF is a constraint architecture with a pre-stage gate and four sequential evaluation stages. Each stage gates the next. No stage can be bypassed. No stage can be reordered.

INPUT
  ↓
[PRE-STAGE: INVESTMENT CLASSIFICATION]
  → Standard: Full analysis, no supplementary preparation
  → Full: Complete analysis with tactical output guidance
  → Elite: Maximum investment, custom output preparation
  ↓
  
[STAGE 1: HARD-GATE CLASSIFICATION]
  → Three-tier routing: Hard Rules → Signal Routing → Content Evaluation
  → FAIL: Eliminated from consideration immediately
  → PASS: Evaluation lens bound to classification category
  ↓
  
[STAGE 2: WEIGHTED SCORING]
  → Evidence ceiling defined — scoring cannot exceed evidenced capability
  → Hard requirements scored at full weight
  → Preferred requirements scored two-sided — absence minimal penalty, presence adds bonus
  → Gaps evaluated against ramp time tier: Days / Weeks / Months / Different Domain
  → Preferred bonuses cannot compensate for hard requirement failures
  ↓
  
[STAGE 3: RISK TIERING]
  → Inputs classified: Low / Medium / High
  → Category-level risk flags surfaced explicitly
  → Each pressure point includes evaluation survivability call
  → Scope realism rule applied — evaluate requirements described, not label
  ↓
  
[STAGE 4: HUMAN VALIDATION & OUTPUT OWNERSHIP]
  → Trajectory impact evaluated across all dimensions
  → Anchoring applied on strong-fit inputs
  → Documented output presented for human review
  → Human owns final decision
  → Human iterates classification rules, weights, and thresholds
OUTPUT: Single recommendation with full rationale and documented failure mode record



Key Architectural Decisions
  Why investment classification before analysis? Not every decision justifies the same depth of evaluation. Spending maximum effort on a low-stakes input wastes resources. 
  Spending minimum effort on a high-stakes input produces unreliable outputs. Classifying investment before analysis begins ensures effort is proportional to consequence magnitude — and documents that classification so it cannot be downgraded mid-analysis to skip uncomfortable findings.

  Why hard gates first? Placing binary elimination before scoring prevents the most common failure mode in weighted decision systems: a high aggregate score masking a failed requirement. 
  Hard requirements and preferences operate in different stages and never interact. A failed hard requirement cannot be rescued by preference performance regardless of how the rest of the evaluation scores.

  Why evidence ceiling in scoring? Scoring without a defined evidence ceiling produces inflation — the framework rewards projected or aspirational capability rather than verified capability. 
  The evidence ceiling is defined before scoring begins and held constant. The framework evaluates what exists. It cannot reward what doesn't.

  Why gap ramp time in scoring? Binary gap treatment — present or absent — penalizes closeable gaps at the same level as fundamental domain mismatches. 
  A gap closeable in three days before first contact is not the same as a gap requiring six months of sustained work. Ramp time tiering calibrates penalty to realistic closing timeline, producing more accurate risk assessment and more defensible output.

  Why human-defined weights? Allowing the model to implicitly weight preferences produces inconsistent results across runs and models. 
  Explicit, human-defined weights are declared before the framework runs and held constant across all inputs in a given evaluation set. Reproducibility is a property of the weight architecture, not the model.

  Why trajectory impact before final output? A decision that scores well on immediate fit but conflicts with longer-term positioning is not a good decision — it's a technically passable one. 
  Evaluating trajectory impact before finalizing output surfaces these cases and forces an explicit acknowledgment of the conflict rather than letting them pass through on score alone.

  Why document every output? Traceability is a core design requirement, not a feature. A decision framework that can't show its work isn't a framework — it's a suggestion engine. 
  Every output includes which hard gates were applied, how each input scored, what risk tier was assigned, and why the top recommendation was selected.

  Why HITL at the end? The model handles what it's good at — structured reasoning within defined constraints. The human handles what requires judgment — whether the rules are right, whether the output makes sense, and whether the framework needs to evolve. 
  These responsibilities are separated deliberately. The model executes. The human owns.
