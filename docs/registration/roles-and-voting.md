# Roles & Voting Rights (MVP)

## 🇸🇰 SK

### Prehľad rolí
Systém rozlišuje viacero rolí používateľov v rámci bytového domu.
Rola určuje:
- oprávnenia v systéme
- spôsob zapojenia do rozhodovania
- hlasovaciu váhu pri písomných hlasovaniach

---

### Definované roly

#### SPRÁVCA (ADMIN)
- správa systému a nastavení domu
- schvaľovanie registrácií
- správa tiketov a workflow
- zakladanie hlasovaní
- finálne uzatváranie procesov

Správca **nemusí mať hlasovaciu váhu**, pokiaľ nie je zároveň vlastník.

---

#### ČLEN RADY
- reprezentuje vlastníkov
- môže zakladať oznamy a návrhy
- môže iniciovať hlasovania (ak je povolené)
- nemá automaticky vyššiu hlasovaciu váhu než vlastník

Hlasovacia váha člena rady je daná **jeho vlastníckym podielom**, nie funkciou.

---

#### VLASTNÍK
- vlastní bytovú jednotku alebo jej časť
- má hlasovacie práva
- hlasovacia váha je odvodená od **podielu na dome**

Príklady hlasovacej váhy:
- 1/1 – plný vlastník
- 1/2 – polovičný vlastník
- 1/3 – tretinový vlastník

---

#### PODNÁJOMNÍK
- býva v byte na základe nájomného vzťahu
- môže:
  - čítať oznamy
  - nahlasovať poruchy
  - komunikovať (komentáre)

❗ **Nemá hlasovacie práva pri písomných hlasovaniach**  
Hlasovacia váha: **0**

---

### Hlasovacie princípy

- hlasovacia váha je viazaná na **vlastnícky podiel**
- rola sama o sebe neurčuje váhu hlasu
- podnájomník má vždy hlasovaciu váhu 0
- systém musí podporovať zlomkové váhy hlasov

---

### Príklady
- vlastník s podielom 1/2 → hlas = 0.5
- dvaja spoluvlastníci 1/2 + 1/2 → spolu 1 hlas
- podnájomník → hlas = 0

---

### Architektonické pravidlá
- hlasovacia váha sa ukladá ako **numerická hodnota**
- váha sa používa len pri písomných hlasovaniach
- zmena vlastníckych podielov je auditovaná
- hlasovanie vždy pracuje so **snapshotom váh** v čase hlasovania

---

## 🇬🇧 EN

### Roles overview
The system defines multiple user roles within a building.
A role determines:
- system permissions
- participation in decision-making
- voting weight in written voting

---

### Defined roles

#### ADMIN (BUILDING MANAGER)
- manages system and building settings
- approves registrations
- manages ticket workflows
- creates votes
- closes processes

Admin does not automatically have voting rights
unless also registered as an owner.

---

#### BOARD MEMBER
- represents owners
- may publish announcements and proposals
- may initiate votes (if allowed)

Voting weight is defined by ownership share,
not by board membership.

---

#### OWNER
- owns a full or partial share of a unit
- has voting rights
- voting weight is based on ownership share

Examples:
- 1/1 – full owner
- 1/2 – partial owner
- 1/3 – partial owner

---

#### TENANT
- lives in the unit under a rental agreement
- can read notices, report issues, and communicate

❗ **Has no voting rights in written voting**  
Voting weight: **0**

---

### Voting principles
- voting weight is based on ownership share
- role alone does not define voting power
- tenants always have zero voting weight
- fractional voting weights must be supported

---

### Architectural rules
- voting weight is stored as a numeric value
- weights apply only to written voting
- ownership changes are audited
- votes use a snapshot of weights at voting time
