# Ticket workflow (MVP)

States:
- REPORTED
- TRIAGED
- IN_PROGRESS
- DONE
- CLOSED
- REJECTED

```mermaid
    [] --> REPORTED
    REPORTED --> TRIAGED : admin
    TRIAGED --> IN_PROGRESS : admin
    IN_PROGRESS --> DONE : admin/tech
    DONE --> CLOSED : admin
    REPORTED --> REJECTED : admin
    REJECTED --> []
    CLOSED --> [*]
```

Transitions:
| From | To | Who | Notes |
|---|---|---|---|
| REPORTED | TRIAGED | ADMIN | validate ticket |
| TRIAGED | IN_PROGRESS | ADMIN | work started |
| IN_PROGRESS | DONE | ADMIN/TECH | fix completed |
| DONE | CLOSED | ADMIN | final closure |
| REPORTED | REJECTED | ADMIN | reason required |
