Human-In-The-Loop Design
Philosophy
SDF is built on a specific belief about the role of AI in decision-making: AI should handle structured reasoning within constraints that humans define. Humans should own the rules, the evidence base, the investment decisions, and the final call.
This isn't a safety hedge — it's an architectural principle. The framework produces better outputs when human judgment defines the constraint space rather than leaving that judgment to the model. A framework where the model defines its own criteria, evaluates against them, and recommends an outcome has no mechanism to catch when the criteria themselves are wrong. That's not a decision framework — it's a rationalization engine with an AI voice.
SDF separates criteria definition from criteria evaluation permanently. The human defines what good looks like before evaluation begins. The model evaluates how well each option meets that definition. The human validates whether the evaluation makes sense and iterates the rules when it doesn't.

What the Human Does
Classifies investment tier before analysis begins — determines how much effort this decision justifies
Defines hard-gate classification rules before the framework runs — establishes what disqualifies immediately
Defines the evidence base — establishes the ceiling of what can be claimed during scoring
Assigns weights to preference categories — determines what matters and how much
Reviews output documentation in full
Validates or overrides the recommendation
Evaluates trajectory impact — determines whether the output serves longer-term positioning
Iterates classification rules, weights, and thresholds based on where prior outputs fell short
Owns the final decision — always

What the Model Does
Routes inputs through the three-tier classification logic
Evaluates inputs against hard-gate rules defined by the human
Scores inputs across weighted preference categories using weights defined by the human
Identifies risk signals and assigns risk tier
Estimates gap ramp time and evaluation survivability
Produces structured output documentation with full rationale
Does not define criteria
Does not determine what matters
Does not make the call

Why This Division
The failure mode of most AI-assisted decision tools is that they ask the model to do too much. Define the criteria, evaluate against them, recommend an outcome, and present it with enough confidence that the human accepts it without scrutiny. When the model owns all three — definition, evaluation, and recommendation — there is no external check on whether the criteria are right. The model becomes both the judge and the standard it's judging against.
SDF breaks this by separating definition from evaluation at the architectural level. The human defines the constraint space before the model sees the inputs. The model operates within that space. The human reviews the output and decides whether the space was defined correctly. If it wasn't, the human changes the rules — not the model.
This division also means the framework improves through human iteration, not model behavior. Every version of SDF exists because a human identified where the prior logic broke down and fixed the architecture. The model didn't evolve the framework. The human did. That's intentional.
