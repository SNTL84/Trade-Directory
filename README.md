# SNTL 84 Trade Directory

**Collab What's Costing You Time.**  
A search-first B2B discovery directory concept for manufacturers, distributors, stockists, suppliers, service providers and buyers.

> **Status:** Stage 1 prototype. Listings are illustrative demo data, not real or verified business records. No production database, authentication, listing submission or real enquiry management is connected yet.

## Brand & contact

- **Project owner:** SNTL 84 — Agentic AI Workflow Professional
- **Website:** https://desidevloper.com
- **WhatsApp:** https://wa.me/919727413309
- **LinkedIn:** https://linkedin.com/in/sntl2784
- **GitHub:** https://github.com/SNTL84
- **Instagram:** https://www.instagram.com/desibiztrade
- **Related capabilities:** Performance Marketing Service, Fulfillment Automation, Bench Resource Availability, Full-Stack Builds, AI Workflows, and Supply Chain Business Intelligence.
- **Social line:** 🚀 Follow for practical AI automation insights & founder systems.

## What this starter does

- Responsive landing page with a directory discovery experience.
- Keyword search across business name, category, city, description and services.
- Category and city filters.
- Listing cards, clear empty state, and WhatsApp enquiry links (pre-filled messages are illustrative).
- Four-stage roadmap that keeps the product direction visible.
- SNTL 84 links and transparent demo-data labelling.
- Optional Supabase client scaffold for a future data layer.
- Local-first workflow; no dependency on Hostinger AI Builder or AI credits.

## Current architecture

- **React 18** for UI.
- **Vite 6** for local development and static production builds.
- **CSS** for responsive styling.
- **Demo records** in `src/data/listings.js`.
- **Optional Supabase scaffold** in `src/lib/supabase.js`, only used after configuring local environment variables.
- **Hostinger** can be used for static hosting once `dist/` has been built.
- **GitHub** remains the source of truth.

No live database integration has been enabled. Do not enter private customer details in this prototype.

## Quick start

### Requirements
- Node.js LTS (use a currently supported LTS release)
- npm
- Git (recommended)

### Install and run
```bash
npm install
npm run dev
```

Vite will print a local URL, typically `http://localhost:5173`.

### Quality checks
```bash
npm run lint
npm run build
npm run preview
```

A build check was not run as part of the initial project authoring. Run the checks above after installing dependencies in your environment.

## Project map

```text
Trade-Directory/
├── public/                 # Static assets (add as needed)
├── src/
│   ├── App.jsx              # Main directory page and filter state
│   ├── main.jsx             # React entry point
│   ├── styles.css           # Responsive visual system
│   ├── data/
│   │   └── listings.js      # Clearly labelled demo records
│   └── lib/
│       └── supabase.js      # Optional Stage 2 client scaffold
├── .env.example             # Names of optional client-side env vars (no secrets)
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── eslint.config.js
├── index.html
├── package.json
└── vite.config.js
```

## Delivery roadmap

### Stage 1 — Searchable prototype (current)
**Goal:** Validate that business discovery, categories and location filters are understandable before spending time on infrastructure.

- [x] Responsive front-end shell
- [x] Demo listings clearly marked as illustrative
- [x] Keyword search
- [x] Category and city filters
- [x] Enquiry CTA demo (WhatsApp message link)
- [x] Initial brand and project documentation
- [ ] Review real target segments and user journeys
- [ ] Replace demo records only when authentic, permitted business details are available
- [ ] Run lint/build checks after installing dependencies

**Exit criteria:** A few target users can find a relevant sample listing quickly and explain what information they expect to see.

### Stage 2 — Real directory data
**Goal:** Add a reliable, maintainable data source only after field requirements and data ownership are clear.

- [ ] Agree on listing schema: business name, category, city, coverage, services, description, public contact, status, owner and timestamps.
- [ ] Select a managed database (Supabase is a candidate, not a hard requirement).
- [ ] Create schema, indexes and migration notes.
- [ ] Define access policies before connecting a public client.
- [ ] Add loading, error and empty states.
- [ ] Add pagination or server-side filtering when the dataset grows.
- [ ] Establish an import/update process and duplicate handling.

**Security:** Any browser-visible Supabase anon/publishable key must be protected by correctly configured Row Level Security. Never put a service-role key or other privileged secret into a `VITE_*` variable.

### Stage 3 — Business registration and trust
**Goal:** Let businesses request changes while keeping public information accountable.

- [ ] Define registration and sign-in requirements.
- [ ] Add submission/edit forms with validation.
- [ ] Add moderation states: draft, submitted, approved, rejected and suspended.
- [ ] Track source and last-confirmed date for business details.
- [ ] Make verification status clear; never imply verification without evidence.
- [ ] Add spam/rate limits and a safe admin review workflow.
- [ ] Publish a privacy notice and retention rules before collecting personal information.

### Stage 4 — Enquiries, analytics and monetization
**Goal:** Prove useful trade demand and conversion before charging.

- [ ] Add enquiry capture with consent and anti-spam protections.
- [ ] Track useful events: search performed, listing opened, enquiry started and completed.
- [ ] Measure listing accuracy, active businesses, qualified enquiries and repeat usage.
- [ ] Test free listings before introducing premium placement.
- [ ] Evaluate paid lead products or subscriptions only after value is demonstrated.
- [ ] Document pricing, refund policy, terms and data handling before taking payments.

## Data and trust rules

1. Sample records are mock data. Do not represent them as active/verified businesses.
2. Use business information only when supplied with permission or obtained from a lawful, appropriate source.
3. Make the date and status of verification visible when real listings are introduced.
4. Provide a correction/removal channel for business owners.
5. Minimize personal information and keep access rules tight.

## Environment configuration (optional)

For Stage 2, create a local `.env.local` from the example:

```bash
cp .env.example .env.local
```

Then fill the project-specific values:

```dotenv
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
```

Do not commit `.env.local`. Vite variables prefixed with `VITE_` are exposed to the browser bundle; they must never contain server secrets. The current prototype does not need these variables.

## Git workflow for a Vibe Coder

Keep changes small, visible and reversible. AI-assisted code still needs review.

```bash
git status
git pull --rebase origin main
git checkout -b feat/short-description
# make and inspect the changes
npm run lint
npm run build
git diff
git add .
git commit -m "feat: describe the change"
git push -u origin feat/short-description
```

Open a pull request, describe behaviour changed, list tests actually run, and disclose known limitations. Avoid claiming checks passed if they were not executed.

## Deployment to Hostinger (without AI Builder)

Hostinger is used here as a hosting destination, not as the application builder.

1. Run `npm install` and `npm run build` locally.
2. Confirm the build generated `dist/`.
3. In Hostinger, configure the intended domain/subdomain (suggested separate subdomain: `trade.desidevloper.com`) to point to the correct web root.
4. Upload the **contents of `dist/`** to that web root using File Manager or SFTP. Do not upload `src/` as a substitute for a build.
5. Enable HTTPS and test the site on desktop and mobile.
6. Keep source code and future changes in GitHub; rebuild and redeploy after changes.

If deploying under a path instead of a domain root, adjust Vite's `base` setting and verify routing/assets. This starter currently uses `base: '/'`.

## Known limitations

- Demo listings only; they are not verified company leads.
- No database, authentication, admin console, listing claim flow, pagination, payments or production analytics.
- No automated tests are included yet.
- Dependencies require installation before lint/build checks can run.
- A real deployment requires building and testing the `dist/` output.

## Contributing and security

See [CONTRIBUTING.md](CONTRIBUTING.md) and [SECURITY.md](SECURITY.md). Report problems through the SNTL 84 GitHub profile rather than publishing private business or customer data in an issue.

---

*Automate What's Costing You Money.*  
*SNTL 84 — Agentic AI Workflow Professional.*
