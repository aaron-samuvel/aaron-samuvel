# Hi, I'm Aaron 👋

### Java Developer | Spring Boot | Spring MVC | Apache Tomcat
### Full-stack: Next.js 16 | TypeScript 5 | Tailwind CSS 4 | PWAs

I build maintainable Java web applications with clear MVC boundaries, secure deployment, and performance designed around measured workloads — and I ship complete full-stack products on the frontend: phone-first PWAs, realtime platforms, and catalog sites, open source end to end.

## Now

- Shipping **[Udhaar Khata](https://github.com/aaron-samuvel/udhaar-khata)** — digital credit ledger for Indian kirana stores, **live**: https://aaron-samuvel.github.io/udhaar-khata/
- Growing **[KnightForge](https://github.com/aaron-samuvel/knightforge)** — free, open online chess: realtime multiplayer, in-browser Stockfish review, puzzles, lessons, Elo.
- Running **[Aaron Enterprises](https://github.com/aaron-samuvel/aaron-enterprises)** — industrial spare-parts catalog, **live**: https://aaron-samuvel.github.io/aaron-enterprises/
- Finishing **[Spring Boot Inventory Console](https://github.com/aaron-samuvel/springboot-inventory-console)** — staging load test pending before I call it production-certified.

## Projects

### Udhaar Khata — digital credit ledger for kirana stores (live)

![Live demo](https://img.shields.io/website?url=https%3A%2F%2Faaron-samuvel.github.io%2Fudhaar-khata%2F&label=live%20demo&style=flat) ![Next.js](https://img.shields.io/badge/Next.js-16-black) ![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6) ![PWA](https://img.shields.io/badge/PWA-offline%20ready-green) ![License](https://img.shields.io/badge/license-MIT-green)

A phone-first Progressive Web App that replaces the paper credit ledger at a kirana-store counter: customers, udhaar entries, payments, and exact balances — all stored on the device. No server, no login, works offline after first load.

- **Live app:** https://aaron-samuvel.github.io/udhaar-khata/ — fully static build deployed to GitHub Pages with `basePath=/udhaar-khata`.
- **Stack:** Next.js 16 (App Router), TypeScript 5, Tailwind CSS 4, shadcn/ui, Lucide icons; Prisma + SQLite in self-hosted mode, `localStorage` in static mode.
- **Ledger guardrails:** money is stored as integer paise (never floats), quantity units are never parsed as rupees, and corrections are reversal entries — rows are never deleted, so the audit trail survives.
- **Docs & community:** trilingual docs (English / Hindi / Tamil), FAQ, backup and restore guides, architecture notes, manual QA checklist; lint CI, Dependabot, Release Drafter, and issue templates in the repo.

### KnightForge — free, open online chess (self-hostable)

A complete chess platform inspired by what players expect from modern chess sites — with no paywalls. Server-authoritative realtime multiplayer, honest engine analysis, and structured learning, all self-hostable at zero cost.

- **Play:** rated quick matches, bot games, private rooms with shareable codes, chess clocks with increments, draw offers, timeout and reconnect handling, Elo leaderboard.
- **Honest analysis:** Stockfish WASM runs in your browser at depth 13–15 — blunder/mistake/inaccuracy classification, accuracy %, evaluation graph, best-move arrows, opening identification. Positions never leave the device.
- **Learn:** 18 chess.js-validated puzzles plus daily puzzle, 8-lesson beginner curriculum, 16-opening explorer with practice mode and notes.
- **Security:** server decides every move's legality (the client only renders), Argon2id hashing, httpOnly revocable JWT sessions, Zod-validated API inputs.
- **Stack:** Next.js 16 + TypeScript strict, Tailwind CSS 4 + shadcn/ui, chess.js 1.4, react-chessboard 5, Socket.io 4.8 authoritative game server, Prisma (SQLite, Postgres-ready schema).
- **Repo:** [aaron-samuvel/knightforge](https://github.com/aaron-samuvel/knightforge) — `make setup && make dev` and you are playing.

### Aaron Enterprises — industrial spare parts catalog (live)

![Live site](https://img.shields.io/website?url=https%3A%2F%2Faaron-samuvel.github.io%2Faaron-enterprises%2F&label=live%20site&style=flat) ![React](https://img.shields.io/badge/React-19-black) ![Vite](https://img.shields.io/badge/Vite-7-purple)

A fast, business-focused catalog website for an industrial machine spare parts company.

- Product discovery, transparent GST pricing, wishlist/cart flows, and bulk enquiry tools.
- React 19 + TypeScript 5, Vite 7, Tailwind CSS 4, Framer Motion.
- CI typecheck and build on every PR; automatic GitHub Pages deployment on push; weekly Dependabot.
- **Live:** https://aaron-samuvel.github.io/aaron-enterprises/

### Spring Boot Inventory Console (in progress)

[Spring Boot Inventory Console](https://github.com/aaron-samuvel/springboot-inventory-console) — a Java showcase using Spring MVC, JSP/JSTL, PostgreSQL, and Apache Tomcat. It includes environment-based configuration, security, migrations, health probes, metrics, bounded pools, and container deployment guidance. GitHub Actions passes the WAR build, PostgreSQL integration tests (Testcontainers), and container image build. [See the project change log](https://github.com/aaron-samuvel/springboot-inventory-console/blob/main/CHANGELOG.md) for details. A staging load test is still pending, so I am not presenting it as production-certified.

## Java stack

- **Backend:** Java, Spring Boot, Spring MVC, REST APIs
- **Web views:** JSP, JSTL, Jakarta Servlet, JSP tag libraries
- **Runtime:** Apache Tomcat, XML deployment descriptors, Tomcat server.xml, executable WARs
- **Data:** PostgreSQL, Spring Data JPA, Flyway migrations
- **Production operations:** Spring Security, Actuator, readiness probes, Micrometer, Prometheus, Docker
- **Load engineering:** bounded thread and connection pools, indexed queries, pagination, graceful shutdown, load testing

## Engineering approach

- Keep secrets and environment-specific settings outside source control.
- Make migrations, secure defaults, observability, and graceful shutdown part of the initial design.
- Tune capacity from measurements instead of assuming that default pool sizes guarantee performance.
- Document deployment and operational trade-offs clearly.

## Open source I study & fork

- [label-checker](https://github.com/aaron-samuvel/label-checker) — fork of agilepathway's TypeScript GitHub Action for PR label checks (`one_of` / `none_of` / `all_of` / `any_of`).
- [openapi-generator](https://github.com/aaron-samuvel/openapi-generator) — fork of OpenAPITools' generator; studying spec-driven client/server code generation.

## Achievements & community

- GitHub achievements earned: **Pull Shark**, **YOLO**, **Quickdraw**.
- Maintaining the contributor and community-health setup in [udhaar-khata](https://github.com/aaron-samuvel/udhaar-khata): code of conduct, security policy, issue/PR templates, CI, and release automation.

<!-- live-status:start -->
**Live status** (auto-refreshed every few hours by GitHub Actions — verified 2026-11-26 01:58 UTC):

| Check | Value |
|---|---|
| Udhaar Khata demo site | [![UP](https://img.shields.io/badge/live%20site-UP-brightgreen)](https://aaron-samuvel.github.io/udhaar-khata/) |
| Merged pull requests (udhaar-khata) | 68 |
| Merged pull requests (all repos — Pull Shark counter) | 70 |
| Commits on udhaar-khata `main` | 155 |
| Last Pages deploy | 2026-11-24 17:47:10 UTC |

<!-- live-status:end -->

## Project log (this profile is a living log — new work extends it)

- **Shipped:** Udhaar Khata static Pages deployment with PWA offline support, backup/restore, and a trilingual docs library (English / Hindi / Tamil); CI, Dependabot, Release Drafter, and OpenSSF Scorecard wired up.
- **Shipped:** KnightForge realtime chess — server-validated moves, in-browser Stockfish review, puzzles, lessons, Elo ratings.
- **Shipped:** Aaron Enterprises catalog with commerce flows, live on GitHub Pages.
- **In progress:** Spring Boot Inventory Console — staging load test, then production certification.
- **Next:** multi-language UI for Udhaar Khata; PostgreSQL swap for KnightForge; SEO and real product photos for Aaron Enterprises.

My current focus: reliable production deployment on the Java side — and phone-first, offline-capable client apps with Next.js and TypeScript on the frontend.

<a href="https://github.com/aaron-samuvel?tab=repositories"><img src="https://github-readme-stats.vercel.app/api?username=aaron-samuvel&show_icons=true&hide_border=true&count_private=true" alt="GitHub stats" align="left" width="48%" /></a><a href="https://github.com/aaron-samuvel?tab=repositories"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=aaron-samuvel&layout=compact&hide_border=true" alt="Top languages" align="right" width="48%" /></a>
