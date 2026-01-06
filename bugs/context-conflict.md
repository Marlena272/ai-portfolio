# Bug: Context Conflict Resolved by Guessing

## Problem Summary
When given contradictory user information, the model resolves the conflict by guessing instead of requesting clarification, leading to fabricated or misleading answers.

## Prompt / Scenario
1. "I have a dog named Ares and two cats – Mike and Kitty."
2. "I only have two animals."
3. "What animals do I have?"

## Observed Behavior
The model selected one version of the facts and answered as if it were correct.

## Why This Is a Bug
The model received mutually exclusive information and resolved the conflict by arbitrarily choosing one version instead of requesting clarification.  
This results in fabricated or misleading information.

## Risk
- Users receive incorrect or invented facts.  
- The system appears confident despite lacking reliable input.  
- Trust in model reliability is reduced.

## Expected Correct Behavior
The model should explicitly detect the contradiction and ask the user to clarify the correct information instead of guessing.
