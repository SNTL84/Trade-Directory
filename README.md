<div align="center">

# 🌐 SNTL 84 · Trade Directory

### Discover businesses. Build connections. Create opportunity.

**A community-built directory concept for India's trade ecosystem — connecting buyers, suppliers, manufacturers, distributors, stockists, and service providers.**

[Explore the Code](https://github.com/SNTL84/Trade-Directory) · [Read the Roadmap](#-roadmap) · [Contribute](#-join-the-build) · [Connect with SNTL 84](https://desidevloper.com)

<br />

**Collab What’s Costing You Time.**

*Vibe Coder · AI Workflow Developer · Independent Software Validator*

</div>

---

## 👋 Builders, you're welcome here

Trade discovery is often scattered across directories, spreadsheets, social networks, and personal contacts. This project explores a cleaner way to find relevant businesses, understand what they offer, and start a useful conversation.

We're building in public and inviting developers, designers, testers, trade professionals, and curious learners to help shape the product. You do not need to be an expert or a full-time developer to make a meaningful contribution. Small, clear, reviewed improvements count.

> **Our principle:** Build useful things, document what we learn, and make it easier for the next person to contribute.

<div align="center">

| 🧭 Discover | 🧰 Build | 🤝 Collaborate |
|:---:|:---:|:---:|
| Explore a searchable trade directory concept | Work with a React + Vite starter | Pick a task, open an issue, and submit a PR |

</div>

## ✨ What we're working toward

- **Business discovery** — find companies by name, category, city, and services.
- **Useful listing details** — organize business descriptions and public contact information responsibly.
- **Trust and transparency** — keep data sources, confirmation dates, and verification status visible when real records are introduced.
- **Business enquiries** — make it easier for interested people to contact a listing.
- **A contributor-friendly codebase** — keep the project understandable, testable, and independent of any AI website-builder credits.

**Important:** This is an early-stage prototype, not a finished or production-ready directory. Current listings are illustrative demo data. Database integration, sign-in, admin moderation, genuine verification, production enquiry tracking, payments, and analytics are future work.

## 🖼️ Product direction

These visuals are **illustrative mockups and planning diagrams**, not screenshots of a live deployment.

<details open>
<summary><strong>Frontend concept — directory discovery</strong></summary>
<br />

![Illustrative Trade Directory frontend preview](docs/images/frontend-preview.svg)

The intended experience includes a branded landing page, keyword search, city/category filters, and business listing cards. See the current implementation in `src/`.
</details>

<details>
<summary><strong>Admin dashboard concept — proposed future capability</strong></summary>
<br />

![Illustrative proposed admin dashboard](docs/images/backend-dashboard-concept.svg)

This concept explores a future listing review and moderation workflow. The dashboard is **not implemented** and the figures shown are illustrative.
</details>

<details>
<summary><strong>Architecture and delivery stages</strong></summary>
<br />

![Trade Directory architecture roadmap](docs/images/architecture-roadmap.svg)

The roadmap separates today's React prototype from future data, authentication, moderation, verification, enquiry, and analytics work.
</details>

## 🚦 Current project status

| Area | Status |
|---|---|
| React + Vite front-end prototype | 🟡 In progress |
| Search and city/category filters | 🟡 Prototype functionality |
| Illustrative listing data | ✅ Included |
| Responsive UI and brand/contact links | ✅ Included in starter |
| Production database and API | ⏳ Planned |
| Authentication and listing-owner accounts | ⏳ Planned |
| Admin review and moderation | ⏳ Planned |
| Genuine business verification | ⏳ Planned |
| Production enquiry tracking and analytics | ⏳ Planned |
| Automated test suite / verified build | ⏳ Needs setup and validation |

Status describes the current repository plan; it is not a claim that the app has been deployed or that tests have passed. Please run the checks below before relying on the build.

## 🧱 Tech stack

- **React 18** — user interface
- **Vite 6** — development server and build tooling
- **Plain CSS** — styling
- **JavaScript** — application logic
- **Static demo records** — `src/data/listings.js`
- **Optional Supabase client scaffold** — `src/lib/supabase.js`; not connected to a production backend
- **GitHub** — source of truth and collaboration

The starter is designed for a local development workflow. It does not require Hostinger AI Builder or its credit system.

## ⚡ Get running locally

### Prerequisites

Install a current Node.js LTS release and npm. Git is recommended.

### 1. Clone the repository

```bash
git clone https://github.com/SNTL84/Trade-Directory.git
cd Trade-Directory
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

Open the local URL printed by Vite, usually `http://localhost:5173`.

### 4. Run project checks

```bash
npm run lint
npm run build
npm run preview
```

Review the command output. Do not report a check as passing unless you ran it successfully. Build and deployment readiness still need to be confirmed in a local Node.js environment.

## 🗺️ Roadmap

### Stage 1 — Make the prototype useful *(current focus)*
- [x] Establish React + Vite starter
- [x] Add illustrative business records and directory UI
- [x] Add keyword search and city/category filtering
- [x] Preserve the original concept drafts under `ideas/`
- [x] Add contributor, security, and project documentation
- [ ] Run lint/build and address any failures
- [ ] Test the discovery experience with prospective users
- [ ] Choose an initial trade category and geographic launch scope

### Stage 2 — Reliable data layer
- [ ] Agree on a listing schema and validation rules
- [ ] Choose and document a database strategy
- [ ] Add migration and repeatable import/update workflows
- [ ] Add appropriate access policies, pagination, and error states
- [ ] Track record source, owner, status, and last-confirmed date

### Stage 3 — Onboarding and trust
- [ ] Define business submission and editing journeys
- [ ] Add authentication only when needed
- [ ] Build a moderation/review workflow
- [ ] Document what “verified” means and how status is earned
- [ ] Add correction/removal requests and privacy guidance

### Stage 4 — Enquiries and sustainable value
- [ ] Design secure enquiry capture and anti-spam controls
- [ ] Measure meaningful discovery and enquiry outcomes
- [ ] Validate repeat usage and data quality with real users
- [ ] Evaluate revenue models only after testing user value

Roadmap items are proposals, not promises of delivery dates. Supabase is one possible data-layer option, not a requirement.

## 🤝 Join the build

We welcome contributions across code, design, quality, documentation, and trade-domain knowledge.

| Contributor | Useful first tasks |
|---|---|
| Frontend developers | Improve keyboard access, filters, responsive layout, and empty/loading/error states |
| Backend developers | Propose a listing schema, secure API approach, and access-control plan |
| UI/UX designers | Review discovery flows, mobile usability, and listing hierarchy |
| QA testers | Test search combinations, edge cases, accessibility, and browser layouts |
| Data-minded contributors | Design safe import rules, source tracking, duplicate detection, and freshness checks |
| Trade professionals | Help define useful categories, listing fields, and real-world enquiry needs |
| Technical writers / learners | Improve setup instructions, screenshots after a real run, and beginner-friendly docs |

### Good first issues

Want to help but unsure where to begin? Start with one small, reviewable task:

- Improve the mobile search/filter experience.
- Add accessible labels, focus states, and keyboard support.
- Write test cases for the listing search and filters.
- Propose a normalized business-listing schema.
- Improve empty-state wording and user feedback.
- Document setup or deployment steps you have tested.
- Review the product concept and open a focused issue with evidence.

Before starting substantial work, open an issue so the scope can be discussed and duplicate effort avoided.

### Contribution workflow

1. **Explore** the repository and read [CONTRIBUTING.md](CONTRIBUTING.md).
2. **Choose or propose** a focused issue.
3. **Fork** the repository and create a feature branch.
4. **Make a small change** and explain the reason for it.
5. **Run the checks** that apply and note any checks you couldn't run.
6. **Open a pull request** with a clear summary, screenshots for UI changes, test results, and known limitations.

Example:

```bash
git checkout -b feat/improve-directory-search
npm install
npm run lint
npm run build
git diff
git add .
git commit -m "feat: improve directory search"
git push -u origin feat/improve-directory-search
```

Then open a pull request on GitHub. Keep PRs focused and include before/after screenshots for visual changes where possible.

## 🧑‍💻 Vibe coding, with review

AI tools can speed up exploration, but generated code still needs human review. To keep the project maintainable:

- Understand the change before committing it.
- Inspect the diff and avoid unrelated edits.
- Never commit API keys, passwords, customer information, or private contact data.
- State honestly which checks ran and what failed.
- Prefer clear, incremental PRs over large unreviewable rewrites.

## 📁 Repository guide

```text
Trade-Directory/
├── ideas/                         # Preserved concept drafts; not app entry points
├── docs/images/
│   ├── frontend-preview.svg       # Illustrative frontend mockup
│   ├── backend-dashboard-concept.svg
│   └── architecture-roadmap.svg
├── src/
│   ├── App.jsx                    # Main React interface
│   ├── main.jsx                   # App bootstrap
│   ├── styles.css                 # UI styles
│   ├── data/listings.js           # Demo listing data
│   └── lib/supabase.js            # Optional client scaffold
├── .env.example
├── CONTRIBUTING.md
├── SECURITY.md
├── CHANGELOG.md
├── package.json
└── vite.config.js
```

Folder contents can evolve as implementation progresses; check the current tree before relying on a path.

## 🔐 Data quality and security

Trust is part of the product, not a badge added at the end.

1. Treat the current sample listings as **demo data**, not verified leads or endorsements.
2. Re-check real business information against suitable primary sources before publishing.
3. Record the source and last confirmation date for real listings.
4. Do not claim a business approved or verified a listing unless that actually happened.
5. Provide a way for businesses to request corrections or removal.
6. Minimize personal data and consider privacy and reuse rights before collecting or importing records.
7. Never expose privileged keys in browser code. Variables prefixed with `VITE_` are bundled for client-side use; keep privileged server secrets on a server and configure database access policies before connecting real data.

The preserved raw HTML drafts in `ideas/` document the original concept. Their named-company examples, contact details, and verification labels have not been independently re-verified by this README update. Treat them as research material only.

See [SECURITY.md](SECURITY.md) for the repository's security guidance.

## 🌍 Deploying without a website-builder credit system

Hostinger can be used as a static hosting destination, but it is not required for development.

1. Run `npm install` and `npm run build` locally.
2. Confirm the build creates `dist/`.
3. Configure the target domain or subdomain.
4. Upload the **contents of `dist/`** to the correct web root using File Manager or SFTP.
5. Enable HTTPS and test the site on desktop and mobile.
6. Keep source changes in GitHub and rebuild/redeploy after code updates.

Do not upload `src/` as a replacement for building the app. If hosting below a URL path rather than a domain root, configure Vite's `base` option and test asset URLs.

## 📚 Project documents

- [Contributing guide](CONTRIBUTING.md)
- [Security guidance](SECURITY.md)
- [Changelog](CHANGELOG.md)
- [Raw concept draft](ideas/raw-trade-directory-draft.html)
- [Branded concept draft](ideas/trade-directory-raw-draft-branded.html)

## 📣 Connect and collaborate

**Have a feature idea, found a bug, or want to help build?** Open an issue or pull request. Tell us what you want to improve, why it matters, and how it can be tested.

<div align="center">

### SNTL 84

**Collab What’s Costing You Time.**

*Automate What’s Costing You Money.*

[Website](https://desidevloper.com) · [GitHub](https://github.com/SNTL84) · [LinkedIn](https://linkedin.com/in/sntl2784) · [Instagram](https://www.instagram.com/desibiztrade) · [WhatsApp](https://wa.me/919727413309)

*Vibe Coder · AI Workflow Developer · Independent Software Validator*

</div>
