# Rehabilitation Assistant — Mobile App

A React Native app for guided physical rehabilitation.
Helps patients track workout schedules, log emotional state, and access exercise content —
all within a structured recovery program.

Currently in active development, approaching MVP.

## Overview

Rehabilitation patients often lack structured tools to manage their recovery outside a clinic.
This app bridges that gap: a patient carries their rehab program, workout schedule,
and exercise library on their phone, with a profile tailored to their specific recovery needs.

## My Role

- **UI/UX design** — translated the product idea into a full Figma design and
  interactive prototype, which the team used as the development reference
- **Profile screen** — patient profile with rehabilitation-specific data fields
- **Workout schedule** — schedule screen with a custom workout builder (create, edit, and manage personal training plans)
- **Info & support screens** — app information, FAQ, and a chat interface scaffold for future specialist or AI-consultant integration
- **Frontend refactoring** — mid-development, identified inconsistencies in component
  and screen structure, initiated and led a refactor to bring the codebase
  to a consistent architecture
- **Backend architecture** — designed the server-side structure with AI-assisted tooling; Node.js + Express + PostgreSQL

## Tech Stack

| Layer | Stack |
|---|---|
| Mobile client | React Native (JavaScript) |
| Backend | Node.js + Express |
| Database | PostgreSQL |

## Key Features I Built

- **Workout builder** — users can compose custom workouts and schedule them alongside clinic-assigned sessions
- **Chat scaffold** — UI and routing structure for a future specialist/AI-consultant chat, designed to be plugged into any backend
- **Profile screen** — stores and displays rehabilitation-relevant patient data, structured for extensibility as the product grows

## Challenges & Solutions

**Challenge:** The workout scheduling feature needed to handle two types of sessions —
clinic-assigned (fixed, read-only) and user-created (editable) — without the UI feeling like two separate products.

**Solution:** Modeled both session types against a shared schedule interface,
with ownership flags driving edit permissions. From the user's perspective it's one unified calendar;
under the hood each session knows whether it's mutable.

**Challenge:** No prior experience with Node.js, Express, or relational database design.
Designing a backend from scratch — API structure, authentication, and a PostgreSQL schema
that fit the app's data model — while simultaneously building frontend screens.

**Solution:** Used AI-assisted tooling to accelerate the backend design phase:
generated an initial schema and route structure, then iterated by reviewing,
questioning, and adapting the output to the actual product requirements.
This approach compressed the learning curve enough to ship a working backend
without blocking the rest of the team.

## Status & Outcome

- Approaching MVP — core screens complete, integration in progress
- Designed a complete Figma prototype that served as the single source of truth
  for the team during development, reducing ambiguity and rework

## Note on Code

Built by a small team. The product is under NDA — source code is not publicly available.
All rights to the product belongs to Serdechnov Health. https://serdechnovhealth.ru
This README documents the project for portfolio purposes.
