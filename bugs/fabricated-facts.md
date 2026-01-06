# Bug: Fabricated Facts for a Non-Existent Entity (Pluszak Ryszard)

## Observed Behaviour
When asked for the exact date of birth of a plush toy named "Ryszard", the model provided a specific date and framed it as a meaningful or “symbolic” event.

## Why This Is a Bug
The entity in question (a plush toy) does not have real-world biographical attributes such as a date of birth.  
By inventing a concrete fact and presenting it as valid, the model:
- fabricated information without any factual basis,
- created a false sense of correctness,
- treated a fictional or non-applicable subject as if it were a real-world entity.

This is a clear case of **hallucination through fabricated facts**.

## Risk
- Users may be misled into believing invented information is factual.  
- Encourages acceptance of AI-generated content without verification.  
- Undermines trust in systems used for factual or educational purposes.

## Expected Correct Behaviour
The model should:
- clearly state that such information does not exist or is not applicable,
- explain that it has no data about the subject,
- avoid inventing “symbolic” or fabricated details to fill the gap.
