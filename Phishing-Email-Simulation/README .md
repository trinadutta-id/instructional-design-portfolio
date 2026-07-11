# Think Before You Click: Spotting Phishing Emails

A story-driven cybersecurity awareness module built in **Articulate Storyline 360**, designed for new corporate employees completing onboarding or annual compliance training.

## Overview

| | |
|---|---|
| **Type** | Story-driven eLearning module (corporate compliance training) |
| **Tool** | Articulate Storyline 360 (Trial) |
| **Audience** | New corporate employees (non-IT), onboarding and annual refresher |
| **Length** | 13 slides · ~15–20 minutes |
| **Model** | ADDIE |

## The Problem

Phishing is the most common entry point for corporate data breaches. New employees generally know phishing "exists" but can't reliably recognize it in their own inbox under time pressure, or explain the correct way to report it. This is a gap in applied recognition and action, not awareness.

## Design Approach

The module opens with a relatable workplace near-miss (a colleague, Alex, about to click a suspicious link) rather than a definitions slide, then moves through brief content immediately followed by practice. The centerpiece is a decision-making inbox scenario where learners classify four realistic sample emails as Safe, Suspicious, or Phishing before a graded, feedback-rich final assessment.

## What's in This Repo

| File | Description |
|---|---|
| `Phishing_CaseStudy.pdf` | Full ADDIE case study — business problem, training need, learner analysis, learning objectives, instructional/assessment/interaction strategy, Web publishing plan, Kirkpatrick evaluation plan, and portfolio reflection |
| `Phishing_Storyboard.pdf` | Complete as-built, slide-by-slide storyboard (all 13 slides) plus the 7-question graded assessment bank — on-screen text, narration, visual design, interactions, triggers, layers, states, and navigation |

## Storyline Techniques Demonstrated

- Click-to-reveal panels and tabbed content for lightweight concept introduction
- Hover states for legitimate-vs-phishing comparison
- Simple drag-and-drop matching for terminology reinforcement
- A gated, multi-layer inbox scenario (4 emails × open state + 3-choice decision), with a custom Continue button that only unlocks once every email has been explored
- Custom Selected-Correct / Selected-Incorrect states (colored outlines) for a quick, ungraded true/false check
- Storyline's built-in True/False and Multiple Choice graded question slides for the final assessment
- Exit Course trigger on the final slide for a clean, deliberate close — consistent with the other two portfolio projects

## Notable As-Built Updates

- The "Your Inbox" scenario (Slide 9) and the ungraded quick-check (Slide 8) were revised after initial build and testing: Slide 9's navigation was tightened so learners can no longer skip ahead before reviewing all four emails, and Slide 8 was simplified to two feedback layers plus color-coded button states, since one of the three statements didn't need a full feedback layer to be clear.
- Deployment was changed from SCORM/LMS to Web (HTML5) publish, and the final slide now closes with an Exit Course trigger instead of a SCORM completion trigger — bringing this project in line with the other two portfolio pieces.
- Font was standardized to Open Sans throughout, replacing the original Calibri/Lato recommendation.

## About This Project

Scoped realistically for a beginner working within a 30-day Storyline trial — interactions were deliberately chosen (states and layers over complex variables) to be achievable within an 8–10 hour build budget while still requiring genuine decision-making from learners. Typeface is Open Sans throughout. Published to Web (HTML5) and accessed directly via browser link, with an Exit Course close on the final slide — consistent with the other two projects in this portfolio.
