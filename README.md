<h1 align="center">pip.me.at</h1>

<p align="center"><strong>How performance review actually works inside big tech.</strong></p>

<p align="center">
  <img src="https://img.shields.io/badge/status-parked-171717?style=flat-square" alt="Status: parked">
  <img src="https://img.shields.io/badge/license-source--available-404040?style=flat-square" alt="License: source-available">
  <img src="https://img.shields.io/badge/part%20of-me.at-737373?style=flat-square" alt="Part of me.at">
</p>

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#built-with">Built with</a>
</p>

When you are put on a performance improvement plan, the record of what happened usually lives on your employer's systems, in their words. I am building pip.me.at to explain how ratings, calibration and improvement plans really work, and to give someone in one a private workbook: plan terms, an append-only evidence journal, check-in prep, and an exit packet that is yours alone, never your employer's. It describes how these systems work and never promises an outcome or gives legal advice.

> **Status:** the product logic is built and tested, but the site is not public yet.

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/overview-dark.svg">
    <img src=".github/assets/overview.svg" alt="pip.me.at at a glance: evidence you cannot edit, prep from your own notes, an exit packet you own, no employer surface" width="880">
  </picture>
</p>

## Why pip.me.at

| The usual record of a plan | pip.me.at |
| --- | --- |
| Notes in a document anyone can quietly edit | An append-only journal with server timestamps and visible amendments |
| Kept on the employer's systems | No employer view, integration or report, by design |
| Meeting prep from memory | An agenda computed from your own entries, with no model involved |
| Shared in full, forever | Share links that expire, with each part of the record opt-in |

## Features

- **Append-only evidence journal**: entries carry a server timestamp and cannot be edited or deleted. Corrections and retractions are appended as amendments that point at the original.
- **Check-in prep**: a per-meeting agenda computed from your own entries (what changed since the last check-in actually held, progress per goal, open questions), with no model involved.
- **Exit packet you own**: a timestamped archive of the whole record, rendered as text or HTML, with the full amendment trail shown and no verdicts or claims added.
- **Share links that fail closed**: every share has a mandatory expiry, and scope defaults to plan terms and goal status, with journal entries, check-ins and artifacts each opt-in.
- **Fenced AI assist**: deterministic pre-call fences (distress escalation first, then legal-advice referral, then a no-fabrication rule) stop a request before any model is called, and answers carry provenance.
- **Content-free analytics and no employer surface**: analytics events cannot carry record content, and there is structurally no employer-side view, integration, or report.
- **Course and blog structure**: a course catalog with outline, reading path, progress and related lessons, and a matching blog structure, ready for written content.

## How it works

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/flow-dark.svg">
    <img src=".github/assets/flow.svg" alt="How pip.me.at works: set terms, journal, prepare, share, export" width="880">
  </picture>
</p>

You start by recording the plan's terms and goals, then keep an evidence journal whose entries are timestamped by the server and can only be amended, never rewritten. Before each check-in, an agenda is computed from those entries. You can share a scoped, expiring view of the record, and at any point export the whole thing as an exit packet you keep.

## Built with

<p>
  <img src="https://img.shields.io/badge/Next.js-16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js 16">
  <img src="https://img.shields.io/badge/React-19-171717?style=flat-square&logo=react&logoColor=white" alt="React 19">
  <img src="https://img.shields.io/badge/TypeScript-5-262626?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-4-404040?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS 4">
  <img src="https://img.shields.io/badge/Drizzle-Postgres-525252?style=flat-square&logo=drizzle&logoColor=white" alt="Drizzle ORM and Postgres">
</p>

- Next.js 16 (App Router), React 19, TypeScript
- Tailwind CSS 4
- Drizzle ORM + Postgres
- Better Auth
- oRPC
- A provider-agnostic AI layer (Anthropic or a configurable driver) behind pre-call guards
- The shared me.at content pipeline for course and blog posts

## Part of the me.at family

pip.me.at is one of my [`*.me.at`](https://me.at) apps. They share one design system, account, and app shell. Development happens in a private monorepo; this repository is the project's public-facing home.

## License

Source-available. See [LICENSE](LICENSE).
