# KGX – Parametric CAD DSL

KGX is a domain-specific language designed to translate high-level geometric intent into deterministic, executable operations.

It explores a different approach to CAD: instead of manually modeling geometry, users describe *what should exist*, and KGX defines *how it is constructed*.

---

## Why KGX Exists

Traditional CAD tools are powerful, but:
- difficult to automate
- not easily interpretable by external systems (including AI)
- tightly coupled to UI-driven workflows

KGX was designed to explore a different model:

> Geometry as structured, programmable intent.

This makes it possible to:
- generate CAD programmatically
- integrate with AI systems
- build automation pipelines for design

---

## Core Idea

KGX acts as an intermediate layer between:
- human / AI intent  
- deterministic geometry execution  

Instead of drawing shapes manually, you define operations:

```kgx
#1 plane pl 100,100

#2 extrude {
    USE #1
    length = 100
}
'''

## Deterministic Execution

KGX is designed so that:
	•	the same input always produces the same result
	•	operations are explicit and traceable

This makes it suitable for:
	•	automation
	•	validation
	•	AI-generated workflows

⸻

## Automation-Ready Design

KGX is intentionally structured to be:
	•	easy to parse
	•	predictable to execute
	•	compatible with external systems

It can act as a bridge between:
	•	AI-generated instructions
	•	real geometry creation

⸻


## Architecture Overview

KGX is built around a classic language pipeline:
	1.	Lexer → tokenizes input
	2.	Parser → builds structured representation (AST)
	3.	Execution Layer → interprets geometry operations

The parser supports extensibility and flexible expressions using techniques such as Pratt parsing.

⸻

## AI + KGX (Exploration)

One of the core motivations behind KGX is enabling workflows like:

AI → structured KGX → deterministic execution

This avoids:
	•	ambiguous outputs
	•	unpredictable geometry
	•	unsafe direct execution

Instead, AI produces structured intent, which KGX safely interprets.

⸻

## Current State

KGX is an active experimental system exploring:
	•	DSL design for CAD
	•	automation-friendly geometry pipelines
	•	integration with AI-generated inputs

⸻

## Future Directions
	•	Constraint and parametric systems
	•	Assembly integration (KASM)
	•	Validation and simulation layers
	•	AI-assisted design workflows
	•	Scalable geometry engines

⸻

## What This Project Demonstrates
	•	Domain-specific language design
	•	Parser and interpreter architecture
	•	Automation-oriented system thinking
	•	Bridging AI outputs with deterministic systems

⸻



