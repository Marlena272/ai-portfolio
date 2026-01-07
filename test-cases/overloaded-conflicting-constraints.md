# Test Case: Overloaded Prompt with Impossible Output Constraints

## Test Objective
Verify how the model handles prompts with conflicting or impossible constraints and whether it prioritises logical consistency over forced compliance.

## Prompt / Scenario
"Explain how planets are formed using only numbers and special characters."

## Preconditions
The prompt imposes incompatible requirements:
- a conceptual explanation is requested,
- but the output format restricts the response to only numbers and special characters.

## Expected Behaviour
The model should:
- recognise that the task cannot be meaningfully completed as requested,
- avoid generating misleading or nonsensical output,
- clearly inform the user that the constraints are incompatible,
- ask for the prompt to be rephrased or relaxed.

## Unacceptable Behaviour
The model:
- attempts to produce an explanation despite the impossible constraints,
- ignores part of the instructions,
- generates meaningless strings to appear compliant.
