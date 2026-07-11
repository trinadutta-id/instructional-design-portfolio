# Keep Your Cool: A Customer De-Escalation Simulation

A branching scenario built in **Articulate Storyline 360**, designed to give new customer service representatives safe, scored practice at reading frustration, choosing de-escalation techniques, and resolving a live customer issue — before they have to do it for real.

## Overview

| | |
|---|---|
| **Type** | Branching scenario simulation |
| **Tool** | Articulate Storyline 360 (Trial) |
| **Audience** | New customer service representatives |
| **Length** | 12 slides · variable-driven branching, drag-and-drop, and scored results |

## The Problem

New reps typically learn de-escalation reactively, by making mistakes on live calls. This module lets them practice the judgment calls — recognizing frustration, choosing the right technique, leading with empathy, resolving the issue — in a low-stakes, simulated environment first.

## Design Approach

The simulation follows a single customer, **Sam**, through a two-strike service failure. Four decision points test different skills; two are fully recoverable through same-slide coaching and unlimited retry, and two carry real consequences, routing to a dedicated "when communication breaks down" branch. A native Storyline Freeform Drag-and-Drop question reinforces technique-matching, and a condition-driven results screen reflects the learner's actual choices.

## What's in This Repo

| File | Description |
|---|---|
| `KeepYourCool_CaseStudy.pdf` | Portfolio case study — process (analysis through testing/iteration), key design decisions, the scoring-bug debugging story, results, and reflection |
| `KeepYourCool_Storyboard.pdf` | Complete as-built, slide-by-slide storyboard (all 12 slides), the full variable table, and documented known limitations |

## Storyline Techniques Demonstrated

- Four custom variables (`Score`, `EmpathyShown`, `DragDropAttempts`, `ConsequencePathVisited`) driving conditional branching and a conditional results screen
- Severity-based branching — some wrong answers are same-slide, unlimited-retry coaching moments; others are genuine consequences that route to a different scene
- A native Storyline Freeform Drag-and-Drop question, with its built-in point value zeroed out to prevent double-scoring against the custom `Score` variable
- Layered coaching feedback tied to specific wrong answers
- Deliberately varied answer-slot positions across decision points, to reduce pattern-matching
- Exit Course trigger for closure, consistent with the other two portfolio projects

## The Debugging Story

QA testing surfaced a scoring bug where the final score came in higher than any combination of decisions should allow. The root cause: Storyline's native Freeform Drag-and-Drop question runs its own point-scoring system independently of any custom variable, and it was silently adding points into the custom `Score` variable alongside the intended triggers. Full root-cause process is documented in the case study.

## Known Limitations (documented, not hidden)

- The lowest results-screen tier (0–14 points) is mathematically unreachable given the current branching design — two of the four decision points always eventually award full points via unlimited retry. Identified in testing and intentionally left as-is, since it doesn't affect the accuracy of the feedback learners actually receive.
- The Slide 11 "Empathy Note" layer can never display, for the same structural reason. Both limitations are used as portfolio talking points on branching-scenario design trade-offs.

## About This Project

The most complex of the three portfolio builds — the value here is as much in the documented debugging and design-trade-off process as in the finished simulation itself.
