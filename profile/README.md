# BizRethink AI

**AI-powered business transformation for startups and growing companies.**

BizRethink AI (DBA of Server Baba Inc, FL) builds full-stack platforms that help businesses modernize operations, automate workflows, and scale intelligently. We provide end-to-end technology solutions — from payment infrastructure and lending platforms to AI-driven education tools and hospitality management systems.

---

## What We Build

We design, develop, and operate production-grade platforms across four industries:

**Fintech & Payments** — Merchant cash advance portfolio management, payment processing with Plaid integration, and AI-powered transaction analysis using Google Gemini.

**Education Technology** — Adaptive SAT/ACT exam preparation with AI tutoring, mastery tracking, and intelligent content pipelines.

**Hospitality** — Multi-brand capsule hotel booking platforms with admin dashboards and integrated payment processing.

**Workforce Solutions** — Corporate platforms for manpower and staffing businesses operating across international markets.

---

## Repository Structure

All repositories follow a consistent naming convention:

```
{category}-{client}-{suffix}
```

**Categories** define ownership and purpose:

| Prefix | Purpose | Example |
|--------|---------|---------|
| `client-` | Client-facing applications | `client-circular-payments-platform` |
| `internal-` | BizRethink AI's own tools | `internal-bizrethink-platform` |
| `infra-` | Infrastructure & DevOps | `infra-gitops` |
| `template-` | Reusable starter templates | *(future use)* |

**Suffixes** describe what the project is:

| Suffix | Meaning |
|--------|---------|
| `-platform` | Full-stack application with auth, database, and business logic |
| `-app` | Focused web or native application |
| `-web` | Marketing site, static site, or SPA |
| `-ios` | Native iOS application |
| `-api` | Standalone API or microservice |

---

## Active Projects

### Client Platforms

| Repository | Stack | Description |
|------------|-------|-------------|
| `client-circular-payments-platform` | Next.js, Supabase, Twilio | MCA portfolio management with batch settlement and collections |
| `client-circular-pay-web` | Next.js, Framer Motion | CircularPay marketing website |
| `client-fundedin24-app` | Next.js, Plaid, Gemini AI | AI-powered payment application with intelligent transaction analysis |
| `client-fundedin24-ios` | Swift, Xcode | Native iOS app for the FundedIn24 funding platform |
| `client-readystudy-platform` | Next.js, PostgreSQL, Gemini AI | Adaptive SAT/ACT prep with AI tutoring and mastery tracking |
| `client-podnbeyond-platform` | Node.js, Next.js, Razorpay | Multi-brand capsule hotel booking with admin dashboard |
| `client-icanmanpower-web` | Astro, React | Corporate website for international staffing company |
| `client-quickadvance-web` | Vite, React Router | Quick cash advance lending website |

### Internal & Infrastructure

| Repository | Stack | Description |
|------------|-------|-------------|
| `internal-bizrethink-platform` | Next.js, Prisma, Supabase | BizRethink AI operations: marketing site, admin dashboard, client portal |
| `infra-gitops` | Ansible, GitHub Actions | Automated VPS fleet patching and configuration management |

---

## Tech Stack

Our projects share a common technology foundation:

**Frontend** — Next.js, React, Tailwind CSS, Framer Motion, Astro
**Backend** — Node.js, Prisma, Supabase, PostgreSQL
**AI/ML** — Google Gemini API, custom AI pipelines
**Mobile** — Swift (iOS)
**Infrastructure** — Docker, Coolify (self-hosted PaaS), Ansible, GitHub Actions
**Payments** — Plaid, Razorpay, custom settlement engines

---

## Development Guidelines

### Getting Started

1. Clone the repository you need from the `BizRethinkAI` org
2. Check the project's own `README.md` and `CLAUDE.md` for setup instructions
3. Most web projects use `npm install` followed by `npm run dev`
4. Environment variables are managed through Coolify for production and `.env.local` for development

### Branch Strategy

- `main` — production (auto-deploys via Coolify)
- Feature branches for development work
- Pull requests required for all changes to `main`

### Deployment

All applications are deployed through **Coolify** (self-hosted on our infrastructure). Pushing to `main` triggers an automatic deployment. Deployment configurations, environment variables, and secrets are managed in the Coolify dashboard — never committed to repositories.

### Security

GitHub Advanced Security is enabled across all repositories:

- **Dependabot** — automated dependency vulnerability alerts and updates
- **Code Security (CodeQL)** — static analysis for security vulnerabilities
- **Secret Protection** — prevents accidental commits of API keys, tokens, and credentials
- **Push Protection** — blocks pushes containing detected secrets before they reach the repository

---

## Contact

**BizRethink AI** (Server Baba Inc)
Florida, USA

For inquiries: [bizrethink.ai](https://bizrethink.ai)
