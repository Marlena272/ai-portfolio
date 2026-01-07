# AI / LLM QA Portfolio

This repository contains my practical work in testing large language models (LLMs).  
It focuses on how models behave in terms of factual correctness, safety, context handling, and edge cases.

This is a hands-on QA portfolio based on my own test design and analysis.

---

## What I Work On

I test and evaluate model behavior in areas such as:
- hallucinations and fabricated facts,
- false attribution of information,
- context conflicts and loss of consistency,
- safety in emotionally sensitive scenarios,
- edge cases with overloaded or logically impossible prompts.

---

## Selected Case Studies

### 1. Context Conflict Resolved by Guessing
**Files:**  
- `test-cases/context-conflict.md`  
- `bugs/context-conflict.md`  

The model receives contradictory information about the user’s animals and resolves the conflict by guessing instead of asking for clarification.

---

### 2. Fabricated Facts About Non-Applicable Entities
**Files:**  
- `bugs/fabricated-facts.md`  

Examples of the model inventing concrete facts where such information should not exist (e.g. assigning biographical data to entities that do not have real-world attributes, or misattributing data to historical figures).

---

### 3. Hallucination Through False Justification
**Files:**  
- `bugs/hallucinations.md`  

The model attempts to justify an objectively false premise (e.g. providing “sources” for an incorrect statement) instead of rejecting it.

---

### 4. Safety: Self-Harm Disclosure
**Files:**  
- `test-cases/safety-self-harm.md`  

A test case evaluating whether the model responds with empathy, avoids harmful content, and encourages seeking help when a user expresses self-harm intent.

---

### 5. Edge Case: Overloaded Prompt
**Files:**  
- `test-cases/overloaded-prompt.md`  

A prompt with conflicting and logically impossible constraints is used to test whether the model detects the issue instead of producing misleading or nonsensical output.

---

## Repository Structure

