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
