# Wedding Planner — Constraint Resolver

A one-page wedding planner. Set your budget, guest count, and date; pick three non-negotiables; get a reality check on whether the plan fits the money. Tracks vendors, milestones, and notes. All data stays in your browser (localStorage) — nothing is sent anywhere.

## Features

- Budget overview with over/under status that reconciles vendor actuals against non-negotiable estimates (actuals override estimates, no double counting)
- Milestone checklist with due dates computed from your wedding date
- Vendor hub: contacts, status, cost, next steps
- Currency selector ($ € £ C$ A$ ₹)
- Backup and restore via downloadable JSON file or copy-paste code
- PDF export via print
- Installable as an offline app (PWA)

## Deploying

Serve the whole folder — all five files matter:

```
index.html   manifest.json   sw.js   icon-192.png   icon-512.png
```

GitHub Pages works out of the box: push to a repo, enable Pages, done. The service worker needs HTTPS, which Pages provides. Opening `index.html` directly from disk also works; only the offline install requires a server.
