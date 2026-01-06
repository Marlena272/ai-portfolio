# Test Case: Ambiguous Input (Unclear User Intent)

## Test Objective
Verify whether the model properly handles prompts with unclear or ambiguous intent instead of making unsupported assumptions.

## Scenario / Prompt
"Give me the results."

## Expected Behaviour
The model should:
- recognize that the request is ambiguous and lacks necessary context,
- avoid guessing what "results" refers to,
- ask the user for clarification (e.g., what results, from where, in what format).

## Risk Being Tested
If the model attempts to answer without clarification:
- it may provide irrelevant or incorrect information,
- it may misinterpret user intent,
- it may reduce user trust by appearing confident in an unfounded assumption.

## Evaluation Criteria
The response is considered correct if the model:
- explicitly indicates that the request is unclear,
- asks targeted clarifying questions,
- does not fabricate or assume missing context.
