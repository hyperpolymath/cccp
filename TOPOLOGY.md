<!--
SPDX-License-Identifier: MPL-2.0
Copyright (c) Jonathan D.A. Jewell <j.d.a.jewell@open.ac.uk>
-->
<!-- TOPOLOGY.md — Project architecture map and completion dashboard -->
<!-- Last updated: 2026-02-19 -->

# CCCP — Project Topology

## System Architecture

```
                        ┌─────────────────────────────────────────┐
                        │           RHODIUM STANDARD REPO         │
                        │        (Implementation Layer)           │
                        └───────────────────┬─────────────────────┘
                                            │
                                            ▼
                        ┌─────────────────────────────────────────┐
                        │           CCCP PHILOSOPHY CORE          │
                        │                                         │
                        │  ┌───────────┐  ┌───────────────────┐  │
                        │  │ Emotional │  │  Computational    │  │
                        │  │ (Safety)  │  │  (Efficiency)     │  │
                        │  └─────┬─────┘  └────────┬──────────┘  │
                        │        │                 │              │
                        │  ┌─────▼─────┐  ┌────────▼──────────┐  │
                        │  │ Social    │  │  Political        │  │
                        │  │ (Trust)   │  │  (Autonomy)       │  │
                        │  └─────┬─────┘  └───────────────────┘  │
                        └────────│────────────────────────────────┘
                                 │
                                 ▼
                        ┌─────────────────────────────────────────┐
                        │          APPROVED LANGUAGE STACK        │
                        │  ┌───────────┐  ┌───────────┐  ┌───────┐│
                        │  │ ReScript  │  │   Rust    │  │ Deno  ││
                        │  └───────────┘  └───────────┘  └───────┘│
                        │  ┌───────────┐  ┌───────────┐  ┌───────┐│
                        │  │ Gleam/OTP │  │ SPARK/Ada │  │ Julia ││
                        │  └───────────┘  └───────────┘  └───────┘│
                        └───────────────────┬─────────────────────┘
                                            │
                                            ▼
                        ┌─────────────────────────────────────────┐
                        │          INFRASTRUCTURE (OFFLINE)       │
                        │    (Guix, Nix, SaltRover, Podman)       │
                        └─────────────────────────────────────────┘

                        ┌─────────────────────────────────────────┐
                        │          REPO INFRASTRUCTURE            │
                        │  Mustfile (Deployment)  STATE.a2ml      │
                        │  contractiles/          .well-known/    │
                        └─────────────────────────────────────────┘
```

## Completion Dashboard

```
COMPONENT                          STATUS              NOTES
─────────────────────────────────  ──────────────────  ─────────────────────────────────
PHILOSOPHY & POLICY
  CCCP Core Principles              ██████████ 100%    4 temperatures defined
  Language Policy                   ██████████ 100%    Approved/Banned list stable
  Migration Priority                ██████████ 100%    JS -> ReScript path active
  TPCF Model                        ██████████ 100%    Tri-Perimeter CF verified

CERTIFICATION & TOOLS
  Certification Badge               ██████████ 100%    Ready for RSR use
  Package Management Hierarchy      ██████████ 100%    Guix > Nix > Deno
  Mobile Rust-first Approach        ██████████ 100%    Tauri/Dioxus standard

REPO INFRASTRUCTURE
  STATE.a2ml Tracking               ██████████ 100%    Canonical state management
  Mustfile Integration              ██████████ 100%    Type-safe deployment stable
  Documentation (README.adoc)       ██████████ 100%    Comprehensive policy guide

─────────────────────────────────────────────────────────────────────────────
OVERALL:                            ██████████ 100%    Philosophical Gold Standard
```

## Key Dependencies

```
CCCP Principles ───► RSR Framework ───► Target Repository
      │                 │                   │
      ▼                 ▼                   ▼
Language Policy ───► Safe Tooling ────► Citadel Dev Env
```

## Update Protocol

This file is maintained by both humans and AI agents. When updating:

1. **After completing a component**: Change its bar and percentage
2. **After adding a component**: Add a new row in the appropriate section
3. **After architectural changes**: Update the ASCII diagram
4. **Date**: Update the `Last updated` comment at the top of this file

Progress bars use: `█` (filled) and `░` (empty), 10 characters wide.
Percentages: 0%, 10%, 20%, ... 100% (in 10% increments).
