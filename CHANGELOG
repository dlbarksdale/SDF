Version History
SDF follows a deliberate versioning philosophy. Each version increment reflects a specific failure mode identified in the prior logic and the architectural fix introduced to address it. The version history is a regression record, not a feature log.

  v1.0 — Initial Architecture
Established the core four-stage structure: hard-gate classification, weighted scoring, risk tiering, human validation. First working implementation of constraint-first reasoning with AI as the structured reasoning layer.
Failure mode identified: Hard gates and preferences were not cleanly separated — high preference scores were partially compensating for borderline hard gate performance. The boundary between non-negotiable requirements and weighted preferences existed conceptually but was not enforced architecturally.

  v1.5 — Hard Gate Enforcement
Introduced strict binary enforcement of hard gates with zero tolerance for score compensation. Any input failing a hard gate is eliminated before entering the scoring phase regardless of projected preference performance.
Failure mode identified: Weight assignments were subjective and inconsistent across evaluations — the same preference carried different implicit weight depending on how the input was framed to the model.

  v2.0 — Explicit Weight Architecture
Formalized weight assignment as a human-defined input declared before the framework runs. Weights held constant across all inputs in a given evaluation set. The model no longer determines what matters — the human does, in advance.
Failure mode identified: Risk tiering was producing misleading confidence signals. High overall scores were masking significant weakness in specific categories.

  v2.1 — Risk Flag Surfacing
Introduced explicit risk flag identification at the category level. Weaknesses are surfaced in the output regardless of overall score, preventing high aggregate performance from obscuring material gaps.
Failure mode identified: Output documentation was inconsistent — rationale quality varied based on model behavior rather than following a defined structure.

  v2.2 — Structured Output Documentation
Standardized output format across all evaluations. All outputs now include hard gate results, category-level scores, risk flags, risk tier assignment, and recommendation rationale in a consistent structure regardless of model or decision domain.
Failure mode identified: Framework behavior varied across LLM configurations — output consistency was partially dependent on model characteristics rather than framework constraints alone.

  v2.3 — Model-Agnostic Validation
Validated framework behavior across Claude, GPT-4, and Gemini. Constraint architecture confirmed model-agnostic — consistent outputs regardless of underlying model. Where model behavior varied, the constraint layer absorbed the variance and produced consistent outputs.
Failure mode identified: Gap penalties were applied uniformly regardless of whether the gap was realistically closeable within the evaluation timeline. A gap closeable in three days was penalized identically to a gap requiring six months of sustained work.

  v2.4 — Gap Ramp Time Estimation
Introduced gap ramp time estimation as a required component of scoring analysis. Four tiers: Days, Weeks, Months, Different Domain. Gap score penalty calibrated to realistic closing timeline rather than binary presence or absence. Days and Weeks ramp gaps carry reduced penalty reflecting their closeability within a standard evaluation cycle. Months gaps carry standard penalty with a mandatory roadmap note. Different Domain gaps carry full hard gap penalty.
Failure mode identified: The preferred requirement rule was asymmetric — it correctly avoided penalizing absences but did not reward presence. Strong preferred matches were being undervalued and had no mechanism to add positive signal to the output.

  v2.5 — Two-Sided Preferred Scoring
Expanded preferred requirement scoring to two-sided. Absence remains at 0.25x weight maximum — no penalty. Presence now scores as a bonus of 0.25–0.5 per strong match, up to 1.0 maximum, added on top of the hard requirement baseline. Hard guardrail added: preferred bonuses cannot compensate for hard requirement failures.
Failure mode identified: All inputs were receiving the same depth of analytical investment regardless of their consequence magnitude or rarity — high-stakes inputs were being evaluated with the same effort as routine ones, producing unreliable outputs on decisions that mattered most.

  v2.6 — Investment Tier Classification & Evaluator Probability Statement
Introduced formal investment tier classification before analysis begins. Three tiers — Standard, Full, and Elite — calibrate analytical depth to the consequence magnitude and rarity of the input. Standard for common inputs. Full for high-value inputs. Elite for rare or high-consequence inputs where the output materially changes trajectory. Investment tier is documented before analysis begins, can be upgraded mid-analysis, and cannot be downgraded to skip uncomfortable gap analysis. Added Evaluator Probability Statement immediately following fit score — written from the evaluator's perspective assessing likelihood of a favorable result based on output match, competitive pool, visible differentiators, and visible gaps.
Failure mode identified: High-consequence inputs were receiving consistent analytical outputs but the framework had no mechanism to verify that the strongest relevant credentials were explicitly surfaced rather than implied — elite inputs were being submitted without confirming the output template was optimally positioned for the specific evaluation context.

  v2.7 — Within-Category Emphasis Check & Evidence Library
Added Within-Category Emphasis Check for Elite tier evaluations. Runs after investment classification and before scoring. Identifies the two to three signals the evaluator will look for first, determines whether those signals are explicitly present or only implied in the output template, and flags what needs surfacing through targeted addition or reorder. Added Evidence Library as a canonical reference that defines the ceiling of what can be claimed during evaluation. Source documents define actual scope of evidenced capability. Framing guidance derived from evidence sources must remain truthful to actual capability performed. Does not authorize adding unevidenced capabilities regardless of what scoring would reward.
Current stable version.
