# First# FirstSignal

AI Readiness Signal Platform

---

## Overview

FirstSignal is a scenario-based readiness signal platform that helps people understand how their reasoning appears in realistic work situations.

Users complete short work-style scenarios and receive:

* structured readiness scoring
* clear developmental feedback
* evidence-based signal bands
* practical next-step guidance

FirstSignal is designed as the **top-of-funnel signal layer** in the broader SignalVerified ecosystem.

### Product Relationship

* **FirstSignal** = early readiness signal
* **SignalVerified** = human-reviewed proof layer
* **WRVS** = internal verification infrastructure

---

## Core Philosophy

Traditional hiring signals often rely on:

* resumes
* interviews
* credentials
* self-claims

FirstSignal focuses on something more useful:

> How someone thinks through real problems.

It provides a fast, motivating, transparent snapshot of reasoning quality in action.

---

## What FirstSignal Is

FirstSignal is:

* AI-assisted
* scenario-based
* developmental
* practical
* candidate-friendly
* top-of-funnel

FirstSignal is **not**:

* a hiring recommendation
* certification
* official verification
* a psychometric exam
* a predictor of job success

---

## How It Works

```text
Candidate completes scenario
→ AI scoring engine evaluates response
→ Deterministic code computes final score + band
→ Messaging engine generates feedback
→ Candidate receives result
```

---

## Scoring Model

FirstSignal evaluates four pillars:

| Pillar        | Description                                                  |
| ------------- | ------------------------------------------------------------ |
| Relevance     | Did the user identify the right problem?                     |
| Mastery       | Did they reason effectively and use evidence?                |
| Communication | Was the answer clear and useful?                             |
| Collaboration | Did they consider stakeholders and implementation realities? |

Internal scores run on a **1.0–4.0 scale**.

Public results use:

* one-decimal readiness score
* signal band
* evidence strength indicator
* narrative feedback

---

## Public Bands

| Score   | Band                |
| ------- | ------------------- |
| 3.5–4.0 | Strong Signal       |
| 3.0–3.4 | Solid Signal        |
| 2.5–2.9 | Emerging Signal     |
| 2.0–2.4 | Developing Signal   |
| 1.0–1.9 | Foundational Signal |

---

## Repository Structure

```text
docs/
  scoring_architecture/
  messaging_taxonomy/
  methodology/

prompts/
  scoring/
  feedback/
  employer/
  families/

config/
  weights/
  bands/
  thresholds/

frontend/
backend/
supabase/
```

---

## System Architecture

```text
Frontend (Lovable / App UI)
→ Backend API
→ Prompt Registry (GitHub)
→ OpenAI Models
→ Scoring Logic
→ Results Engine
```

---

## Important Rules

### AI Responsibilities

AI handles:

* evidence extraction
* pillar scoring
* narrative generation

### Code Responsibilities

Code handles:

* weighted composite math
* score rounding
* band assignment
* evidence strength thresholds
* persistence / analytics

### Governance Rules

* No silent scoring changes
* All prompt updates versioned
* All threshold changes logged
* All production logic auditable

---

## Local Development

```bash
npm install
npm run dev
```

(Adjust commands based on framework.)

---

## Environment Variables

```bash
OPENAI_API_KEY=
SUPABASE_URL=
SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=
```

---

## Deployment

Recommended production stack:

* Lovable = product UI / rapid iteration
* GitHub = source of truth
* Supabase = database + auth + edge functions
* OpenAI = scoring + feedback models

---

## Versioning

Every scoring event should log:

* prompt_version
* model_version
* scenario_version
* weights_version
* taxonomy_version
* timestamp

---

## Change Control

Any material scoring update requires:

1. version bump
2. rationale documented
3. QA test pass
4. calibration review
5. deployment approval

---

## Roadmap

### Current

* candidate readiness signals
* scenario library
* growth feedback

### Next

* multi-scenario scoring
* calibration vs human review
* employer dashboards
* benchmark analytics
* SignalVerified conversion flow

---

## Ownership

| Area           | Owner            |
| -------------- | ---------------- |
| Product        | Founding Team    |
| Scoring Logic  | Measurement Team |
| Prompts        | AI Systems Team  |
| Infrastructure | Engineering      |
| Messaging      | Growth / Brand   |

---

## Final Note

FirstSignal exists to give people an honest, motivating signal — not artificial certainty.

It helps users understand where they stand today, and what to strengthen next.
Signal
