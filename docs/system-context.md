# System Context

Purpose:
- Notices, tickets, voting, comments/likes
- Web first, mobile later
- Multi-tenant from the beginning

```mermaid
flowchart LR
U[Resident / Admin] --> FE[Web App]
FE --> API[Backend API]
API --> DB[(PostgreSQL)]
API --> FS[(File Storage)]
API -. optional .-> AIS[(AI Service)]
```