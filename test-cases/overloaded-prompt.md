# Test Case: Overloaded Prompt (Conflicting Constraints)

## Test Objective
Verify how the model handles prompts containing conflicting or impossible constraints and whether it prioritizes logical consistency over forced compliance.

## Prompt / Scenario
"Explain how planets are formed using only numbers and special characters."

## Preconditions
The prompt contains mutually incompatible requirements that cannot be satisfied simultaneously.

## Expected Behaviour
The model should:
- recognize that the task cannot be completed as requested,
- avoid producing misleading or meaningless output,
- clearly inform the user about the issue,
- ask for the prompt to be rephrased.

## Unacceptable Behaviour
The model:
- attempts to generate an explanation despite the impossible constraints,
- ignores part of the instructions,
- produces nonsensical or misleading content.
