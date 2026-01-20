# Architecture TOC

## 🇸🇰 SK
Tento dokument je mapa architektúry. Obsahuje zoznam tém, ktoré musia byť pokryté,
aby bol systém navrhnutý profesionálne a udržateľne.

Legenda:
- ✅ hotové
- 🔜 plánované

---

## 🇬🇧 EN
This document is the architecture map. It lists the topics that must be covered
to design a professional and maintainable system.

Legend:
- ✅ done
- 🔜 planned

---

## 1) Context & scope
- ✅ `docs/system-context.md` – system purpose + context diagram
- 🔜 `docs/scope/in-scope.md` – in-scope / out-of-scope
- 🔜 `docs/stakeholders/stakeholders.md` – stakeholders + responsibilities

---

## 2) Containers (high-level architecture)
- 🔜 `docs/containers/overview.md` – FE / BE / DB / storage / AI
- 🔜 `docs/containers/deployment.md` – environments (dev/stage/prod) (minimal)

---

## 3) Domain model
- 🔜 `docs/domain/entities.md` – core entities overview
- 🔜 `docs/domain/relationships.md` – relationships + invariants
- 🔜 `docs/data/er-mvp.md` – MVP ER diagram
- 🔜 `docs/domain/units-and-membership.md` – unit + membership rules

---

## 4) Workflows (behaviour)
- ✅ `docs/registration/overview.md` – registration + approval (MVP)
- ✅ `docs/tickets/workflow.md` – ticket lifecycle (MVP)
- 🔜 `docs/voting/workflow.md` – voting lifecycle + snapshot weights
- 🔜 `docs/social/comments-and-reactions.md` – comments + likes
- 🔜 `docs/notifications/overview.md` – in-app notifications (MVP)

---

## 5) Security
- 🔜 `docs/security/roles-and-voting.md` – roles + voting rights (weights)
- 🔜 `docs/security/authentication.md` – login, password reset (MVP)
- 🔜 `docs/security/authorization.md` – RBAC + tenant scoping rules
- 🔜 `docs/security/permissions-matrix.md` – who can do what (table)

---

## 6) API Contract (DTO lives here)
- 🔜 `docs/api/overview.md` – API principles + versioning
- 🔜 `docs/api/auth.md` – register/login/me DTOs
- 🔜 `docs/api/tickets.md` – tickets DTOs
- 🔜 `docs/api/posts.md` – notices DTOs
- 🔜 `docs/api/voting.md` – voting DTOs
- 🔜 `docs/api/social.md` – comments/likes DTOs
- 🔜 `docs/api/errors.md` – standard error format

---

## 7) Realtime & events
- 🔜 `docs/realtime/overview.md` – WebSocket/SSE approach (MVP)
- 🔜 `docs/realtime/events.md` – list of emitted events (table)

---

## 8) AI (optional)
- 🔜 `docs/ai/overview.md` – AI as assistant (what it does / does not do)
- 🔜 `docs/ai/feature-flags.md` – toggle rules (global + tenant + feature)
- 🔜 `docs/ai/suggestions.md` – suggestion data model + audit

---

## 9) Non-functional requirements (minimal)
- 🔜 `docs/nfr/auditability.md`
- 🔜 `docs/nfr/performance.md`
- 🔜 `docs/nfr/backups-and-retention.md`
- 🔜 `docs/nfr/observability.md` – logs/metrics (minimal)

---

## 10) ADR (Architecture Decision Records)
- 🔜 `docs/adr/README.md` – how we write ADRs
- 🔜 `docs/adr/ADR-001-backend-language.md`
- 🔜 `docs/adr/ADR-002-ai-assistant.md`
- 🔜 `docs/adr/ADR-003-multi-tenant-model.md`
- 🔜 `docs/adr/ADR-004-voting-weight-snapshot.md`
