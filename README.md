# BDM – Architecture

---

## 🇸🇰 Slovensky

### Čo je BDM
BDM (Building / Bytový Dom Management) je webová aplikácia
určená na správu komunikácie a procesov v bytových domoch.

Zameriava sa najmä na:
- oznamy a nástenku
- nahlasovanie a riešenie porúch (tikety)
- hlasovania a rozhodovanie
- transparentnú komunikáciu (komentáre, reakcie)
- voliteľnú AI pomoc (iba návrhy, nikdy automatické rozhodnutia)

### Architektonické ciele
- oddelený frontend a backend
- modulárny monolit (žiadne mikroservisy v MVP)
- multi-tenant od začiatku
- auditovateľná a deterministická logika
- AI ako voliteľný a vypínateľný doplnok

---

## 🇬🇧 English

### What is BDM
BDM (Building Management) is a web-first (mobile later) application
designed to manage communication and operational processes
within apartment buildings.

The system focuses on:
- notices and announcements
- issue reporting and workflows (tickets)
- voting and decision-making
- transparent communication (comments, reactions)
- optional AI assistance (suggestions only, never automatic decisions)

### Architectural goals
- clear separation of frontend and backend
- modular monolith backend (no microservices initially)
- multi-tenant architecture from day one
- deterministic and auditable business logic
- optional and fully toggleable AI assistance

---

## Scope of this repository
This repository contains:
- system context and container diagrams
- core business workflows
- data model overviews
- security and role concepts
- architecture decision records (ADR)
