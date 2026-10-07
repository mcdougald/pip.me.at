# pip.me.at

How performance review actually works inside big tech.

pip.me.at is planned as a written course and blog on ratings, calibration, and improvement plans, plus a private workbook for someone who is in one. The workbook keeps plan terms, an append-only evidence journal, check-in prep, and an exit packet the user owns: yours alone, never your employer's. It describes how these systems work and never promises an outcome or gives legal advice. The product logic is built and tested, but the site is not public yet.

## Features

- **Append-only evidence journal**: entries carry a server timestamp and cannot be edited or deleted; corrections and retractions are appended as amendments that point at the original.
- **Check-in prep**: a per-meeting agenda computed from your own entries (what changed since the last check-in actually held, progress per goal, open questions), with no model involved.
- **Exit packet you own**: a timestamped archive of the whole record, rendered as text or HTML, with the full amendment trail shown and no verdicts or claims added.
- **Share links that fail closed**: every share has a mandatory expiry, and scope defaults to plan terms and goal status, with journal entries, check-ins and artifacts each opt-in.
- **Fenced AI assist**: deterministic pre-call fences (distress escalation first, then legal-advice referral, then a no-fabrication rule) stop a request before any model is called, and answers carry provenance.
- **Content-free analytics and no employer surface**: analytics events cannot carry record content, and there is structurally no employer-side view, integration, or report.
- **Course and blog structure**: a course catalog with outline, reading path, progress and related lessons, and a matching blog structure, ready for written content.

## Built with

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

See [LICENSE](LICENSE).
