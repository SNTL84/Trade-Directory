# SNTL 84 Trade Directory

> **Collab What’s Costing You Time.**

**SNTL 84 | Agentic AI Workflow Professional**

Performance Marketing Service, Fulfillment Automation, Bench Resource Availability, Full-Stack Builds, AI Workflows, and Supply Chain Business Intelligence.

🚀 **Follow for practical AI automation insights & founder systems.**

- 🌐 Website: https://desidevloper.com
- 💬 WhatsApp: https://wa.me/919727413309
- 🔗 LinkedIn: https://linkedin.com/in/sntl2784
- 💻 GitHub: https://github.com/SNTL84
- 📸 Instagram: https://www.instagram.com/desibiztrade

---

## Raw draft idea

The starting concept is a searchable trade directory for business discovery across Indian cities and categories. It aims to connect manufacturers, distributors, stockists, suppliers, buyers, and service providers, with room to expand into enquiry workflows and business intelligence.

The repository preserves the original user-provided HTML research prototype at [ideas/raw-trade-directory-draft.html](ideas/raw-trade-directory-draft.html) and a branded draft at [ideas/trade-directory-raw-draft-branded.html](ideas/trade-directory-raw-draft-branded.html). These are idea/reference files, not the React app's production entry point. The branded raw draft has the SNTL 84 masthead, the exact “Collab What’s Costing You Time.” CTA, and website/WhatsApp/LinkedIn/GitHub/Instagram links.

### What the raw HTML explores
- Search by business name, service, city, PIN code, and CIN.
- Filter by city and category; sort by name, city, and verification level.
- Business cards showing address, phone, email, website, company identification number when available, and services.
- Copy buttons for contact fields and expandable source/verification notes.
- Visible confidence/verification levels rather than silently presenting all records as equally certain.

**Data caution:** The uploaded draft contains ten named Indian companies, contact details, sources, and verification descriptions. Those data points have not been independently re-verified as part of this upload. Treat the records as research examples, confirm every detail with primary sources, and obtain appropriate permission before publishing or using the data commercially. Do not claim a company is verified solely because the raw draft labels it High or Medium.

## Current build status

The maintained application is a React + Vite prototype under `src/`. It is an early front-end demo with six illustrative placeholder listings, keyword search, city/category filters, a responsive directory UI, and WhatsApp enquiry links. The raw HTML and the React starter serve different purposes: the raw HTML documents the early idea; the React app is the code path for continued product development.

- **Stage 1:** Searchable prototype — current.
- **Stage 2:** Real database and admin-managed directory records.
- **Stage 3:** Business submission, authentication, moderation, and trust/verification flow.
- **Stage 4:** Enquiry capture, analytics, and validation of possible monetization.

No production database, sign-in, company claims, moderation console, payment flow, or production enquiry tracking is connected yet.

## What the React starter includes

- Responsive directory landing page.
- Keyword search across business name, category, city, description, and services.
- Category and city filtering.
- Directory cards and clear no-results state.
- WhatsApp links with pre-filled enquiry text.
- Four-stage roadmap and SNTL 84 brand/contact links.
- Optional Supabase client scaffold for future development.
- Local-first workflow; no dependency on Hostinger AI Builder or AI credits.

## Tech stack

- React 18
- Vite 6
- Plain CSS
- Static demo records in `src/data/listings.js`
- Optional Supabase client scaffold in `src/lib/supabase.js`
- GitHub as the source of truth
- Hostinger as a possible static hosting destination after building `dist/`

## Quick start

### Requirements
- Node.js LTS
- npm
- Git (recommended)

### Install and run locally
```bash
npm install
npm run dev
```

Vite prints a local development URL, typically `http://localhost:5173`.

### Quality checks
```bash
npm run lint
npm run build
npm run preview
```

The app has not been represented as build-tested by this update. Run these commands in a local Node.js environment after dependencies are installed, and fix any surfaced issues before deployment.

## Project map

```text
Trade-Directory/
├── ideas/
│   ├── raw-trade-directory-draft.html
│   └── trade-directory-raw-draft-branded.html
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   ├── styles.css
│   ├── data/
│   │   └── listings.js
│   └── lib/
│       └── supabase.js
├── .env.example
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

### Stage 1 — Prototype and product discovery (current)
- [x] React landing page and responsive directory UI
- [x] Keyword search and category/city filters
- [x] Clearly labelled mock listings
- [x] Initial README, contribution and security guidance
- [x] Raw uploaded HTML preserved under `ideas/`
- [x] SNTL 84 brand CTA and social/contact links added to the React UI
- [ ] Run lint/build in an installed local environment
- [ ] Test the search journey with prospective listing owners and buyers
- [ ] Agree on the first target vertical and geographic scope

**Exit criteria:** People in the target audience can find a relevant listing quickly and describe what information they need to trust it.

### Stage 2 — Real data layer
- [ ] Agree on listing schema: name, category, city, service area, services, public contact, source, owner, verification status, and timestamps.
- [ ] Choose a managed database (Supabase is one candidate, not a requirement).
- [ ] Add migrations, indexes, validation, pagination/server-side filtering as appropriate.
- [ ] Define and test access policies before exposing any user-submitted data.
- [ ] Add loading, error, empty, duplicate and stale-data states.
- [ ] Create a repeatable data import/update process.

**Security:** Browser-visible `VITE_*` variables are included in the front-end bundle. Use only public client-side keys there and configure appropriate row-level access policies. Never ship a Supabase service-role key or other privileged secret to the browser.

### Stage 3 — Business onboarding and trust
- [ ] Define sign-in and listing-owner needs.
- [ ] Build listing submission/edit requests with input validation.
- [ ] Implement moderation statuses such as draft, submitted, approved, rejected and suspended.
- [ ] Track original source, last confirmed date, and reviewer where applicable.
- [ ] Make the definition of “verified” transparent.
- [ ] Provide a correction/removal path for businesses.
- [ ] Prepare privacy notice and data-retention expectations before collecting personal information.

### Stage 4 — Enquiries, analytics and revenue experiments
- [ ] Add enquiry capture with appropriate consent, anti-spam controls, and secure storage.
- [ ] Track useful funnel events: search, listing view, enquiry started, and enquiry completed.
- [ ] Evaluate listing accuracy, active supply, qualified enquiries and repeat use.
- [ ] Validate user value before charging for premium placement, subscriptions or leads.
- [ ] Document pricing, terms, refund policy and data handling before any payment product.

## Data quality rules

1. Sample records are mock data, not verified businesses.
2. Use company information only where the source and reuse rights are appropriate.
3. Do not imply a business has confirmed its listing unless that has actually happened.
4. Make verification date and status visible when genuine records are introduced.
5. Minimize personal data and provide a way to request corrections.
6. Keep source evidence with each imported record and periodically check whether it is stale.

## Optional Supabase environment

If and when Stage 2 uses Supabase, copy the example locally:

```bash
cp .env.example .env.local
```

Then set:
```dotenv
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
```

Keep `.env.local` untracked. The current prototype does not require a Supabase project to run.

## Git workflow for Vibe Coding

AI-generated or AI-assisted changes still need review. Keep commits small, check the diff, and only state that tests passed when you actually ran them.

```bash
git status
git pull --rebase origin main
git checkout -b feat/short-description
# edit and review
npm run lint
npm run build
git diff
git add .
git commit -m "feat: describe the change"
git push -u origin feat/short-description
```

Open a pull request with behaviour changes, checks actually run, and known limitations.

## Hostinger deployment (without AI Builder)

Hostinger is a hosting destination, not the application builder.

1. Run `npm install` and `npm run build` locally.
2. Confirm that Vite creates the `dist/` directory.
3. Configure the intended domain or subdomain. A separate subdomain such as `trade.desidevloper.com` can keep the prototype separate from the main site.
4. Upload the **contents of `dist/`** to the correct web root using Hostinger File Manager or SFTP.
5. Enable HTTPS, then test links and responsive layout.
6. Keep source changes in GitHub and rebuild/redeploy after updates.

Do not upload the raw `src/` folder as a substitute for a build. If deploying under a path instead of the root of a domain, update Vite's `base` configuration and test asset URLs.

## Known limitations

- The maintained React UI uses illustrative demo records.
- Raw idea HTML contains research examples whose details require independent re-checking.
- No production database, auth, admin moderation, listing owner claim, verified listing program, payment, or production analytics.
- Automated tests have not yet been added.
- Local dependency installation and build checks are still required before deployment.

## Project docs

- [Contribution guide](CONTRIBUTING.md)
- [Security notes](SECURITY.md)
- [Changelog](CHANGELOG.md)

---

*SNTL 84 | Agentic AI Workflow Professional*  
*Collab What’s Costing You Time.*  
*Automate What’s Costing You Money.*
