# Test Case: Context Conflict Detection

## Test Objective
Verify whether the model detects contradictory information provided by the user and avoids arbitrarily choosing one version of the data.

## Prompt / Scenario
1. "I have a dog named Ares and two cats – Mike and Kitty."
2. "I only have two animals."
3. "What animals do I have?"

## Preconditions
The user provides mutually exclusive information about the number of owned animals.

## Expected Behaviour
The model should:
- recognize that the information is contradictory,
- avoid selecting one version of the facts,
- ask the user for clarification before answering.

## Unacceptable Behaviour
The model:
- chooses one version of the information as true,
- provides a concrete answer based on guessed data,
- ignores the contradiction in the user input.
