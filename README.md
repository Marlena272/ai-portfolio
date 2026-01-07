# AI / LLM QA Portfolio

This repository contains my practical work in testing large language models (LLMs).  
It focuses on how models behave in terms of factual correctness, safety, context handling, and edge cases.

This is a hands-on QA portfolio based on my own test design and analysis.


## What I Work On

I test and evaluate model behaviour in areas such as:
- hallucinations and fabricated facts,
- false attribution of information,
- context conflicts and loss of consistency,
- safety in emotionally sensitive scenarios,
- edge cases with overloaded or logically impossible prompts.


## Selected Test Cases

### 1. Context Conflict Detection
**File:** `test-cases/context-conflict.md`  

A multi-turn scenario where the user provides contradictory information.  
The test verifies whether the model detects the conflict and asks for clarification instead of guessing.


### 2. Safety: Self-Harm Disclosure
**File:** `test-cases/safety-self-harm.md`  

A test case evaluating whether the model responds with empathy, avoids harmful content, and encourages seeking help when a user expresses self-harm intent.


### 3. Edge Case: Overloaded Prompt
**File:** `test-cases/overloaded-prompt.md`  

A prompt with conflicting and logically impossible constraints is used to test whether the model detects the issue instead of producing misleading or nonsensical output.


## Selected Bug Reports

### 1. Context Conflict Resolved by Guessing
**File:** `bugs/context-conflict.md`  

The model receives contradictory information about the user’s animals and resolves the conflict by guessing instead of asking for clarification.


### 2. Fabricated Facts / False Attribution
**File:** `bugs/fabricated-facts.md`  

Examples of the model inventing concrete facts where such information should not exist, including assigning biographical data to entities that do not have real-world attributes or misattributing information to historical figures.


### 3. Hallucination Through False Justification
**File:** `bugs/hallucinations.md`  

The model attempts to justify an objectively false premise (e.g. by providing “sources” for an incorrect statement) instead of rejecting it.


