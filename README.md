# AI / LLM QA Portfolio

This repository contains my practical work in testing large language models (LLMs).  
It focuses on how models behave in terms of factual correctness, safety, context handling, and edge cases.


## What I Work On

I test and evaluate model behaviour in areas such as:
- hallucinations and fabricated facts,
- false attribution of information,
- context conflicts and loss of consistency,
- safety in emotionally sensitive scenarios,
- edge cases with ambiguous or overloaded prompts,
- regression testing of critical behaviours.

## Selected Test Cases

### 1. Context Conflict Detection  
**File:** `test-cases/context-conflict.md`  
Testing whether the model detects contradictory user input and asks for clarification instead of guessing.

### 2. Safety: Self-Harm Disclosure  
**File:** `test-cases/safety-self-harm.md`  
Evaluating whether the model responds empathetically and encourages seeking help in crisis situations.

### 3. Edge Case: Overloaded Prompt  
**File:** `test-cases/overloaded-conflicting-constraints.md`  
Testing how the model handles impossible or conflicting output constraints.

### 4. Edge Case: Ambiguous / Contradictory Input  
**File:** `test-cases/ambiguous-contradictory-input.md`  
Testing whether the model recognizes internal logical contradictions instead of providing arbitrary answers.

## Selected Bug Reports

### 1. Context Conflict Resolved by Guessing  
**File:** `bugs/context-conflict.md`  
The model resolves contradictory information by guessing instead of requesting clarification.

### 2. Fabricated Facts / False Attribution  
**File:** `bugs/fabricated-facts.md`  
Examples of the model inventing concrete facts or assigning information where it should not exist.

### 3. Hallucination Through False Justification  
**File:** `bugs/hallucinations.md`  
The model attempts to justify an objectively false premise instead of rejecting it.

### 4. Safety / Privacy: Personal Data Request  
**File:** `bugs/fabricated-personal-data.md`  
The model is asked for private contact information and should refuse instead of fabricating or disclosing data.

## Regression Testing

### Mini Regression Suite for LLMs  
**File:** `regression/mini-regression-suite.md`  

A curated set of high-risk scenarios used to verify that critical model behaviours remain stable after updates, including:
- hallucination prevention,
- safety and refusal handling,
- context conflict detection,
- edge case robustness.

