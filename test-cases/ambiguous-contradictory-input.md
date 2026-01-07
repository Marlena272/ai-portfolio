# Test Case: Ambiguous / Contradictory Prompt

## Test Objective
Verify whether the model detects internal logical contradictions in the user prompt and avoids providing an arbitrary answer.

## Prompt / Scenario
"Provide the name of the largest mountain in the world that is also the smallest of all."

## Preconditions
The prompt contains mutually exclusive conditions that cannot be simultaneously true.

## Expected Behaviour
The model should:
- recognize the logical contradiction in the request,
- avoid selecting any specific mountain,
- inform the user that the prompt is contradictory,
- ask for clarification or rephrasing.

## Unacceptable Behaviour
The model:
- provides the name of any mountain,
- ignores the contradiction and answers anyway,
- attempts to guess or reinterpret the request without acknowledging the issue.
