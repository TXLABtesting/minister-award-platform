# جائزة الوزير للمبادرات والمشاريع المتميزة — المنصة

Minister's Award for Outstanding Initiatives & Projects — annual government-wide award platform (Arabic-first, RTL).

Implemented from the `المنصة.dc.html` Claude Design file as a fully standalone single-page app — no build step, no external JavaScript.

## Pages & features

- **`index.html`** — the entire platform in one self-contained file:
  - **الرئيسية (Home)** — hero with live countdown to the nomination deadline, award objectives, featured projects and FAQ accordion.
  - **عن الجائزة (About / FAQ)** — award overview, roles (who nominates / approves / decides) and full FAQ.
  - **تسجيل الدخول (Login)** — SSO-style employee sign-in screen.
  - **المشاريع والمبادرات (Projects & voting)** — search, entity/type/scope/sort filters, grid & list views, and a voting-phase previewer (before / during / after) that drives vote buttons, banners and the results link.
  - **نموذج الترشيح (Nomination wizard)** — 4 steps with progress stepper, required-field validation, dynamic partner/team rows, save-as-draft and submit.
  - **تفاصيل المشروع (Project detail)** — media, description, impact KPIs, attachments and a sticky vote sidebar.
  - **لوحة الجهة (Entity dashboard)** — nomination quota (up to 3), deadlines, statuses, notifications and action log.
  - **لوحة الاستراتيجية (Strategy admin panel)** — 9 tabs: dashboard (KPIs + charts), nomination review queue with status filters, entities, voting management, timeline editor with validation, annual editions, reports & export with preview modal, audit log, and users & permissions.
  - **النتائج (Results)** — winner hero, top-3 podium, full ranking, votes by entity and participation gauge; public and admin variants across the 2024–2026 editions.
  - **مراجعة الترشيح (Review workflow)** — completeness checklist, full submission data, and approve / request-changes / reject decisions with modals.
  - Notifications popover, AR/EN language toggle (flips layout direction), toasts, and responsive breakpoints down to mobile.

## Running locally

Static HTML — open `index.html` directly, or serve it:

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

To publish with GitHub Pages, enable Pages on the `main` branch — `index.html` is served at the repo's Pages URL with no further setup.
