# ❇️ NumiBright

[Numibright.com]([https://numibright.com/]) NumiBright.com is a web app for people who feel anxious about money and do not know where to begin. Numibright helps users intsantly discover that "oh, *that's* where my money goes" moment and set up personalized plan in under five minutes. No bank login, no forced sign in, and no dozens of new tools to learn.

---

### Core Capabilities
 
- **Monthly Income** — quickly understand your monthly income.
- **Monthly Budgets** — divvy up your monthly income into 3 buckets: Needs, Savings, and Wants.
- **Paycheck Split** — each paycheck, users know exactly where their money should go.
- **Savings Goals** — quickly get users set up on the right track and identify how fast they can reach their financial goals.

---

## Infrastructure & Tech Stack

NumiBright is a React single-page web app built on the Memoir design system, with a new backend layer added for the MVP: Firebase for auth, MongoDB for user data, Stripe for premium payments, and PostHog for analytics. Onboarding survey calculations run client-side until the upgrade modal hits. The data model stores amounts with a currency code from day one, so future locales drop in as days of work rather than weeks.

### Frontend

| Layer | Technology |
|-------|-----------|
| Framework | React |
| Styling | Tailwind CSS |
| UI components | custom shadcn/ui |
| Onboarding logic | Client-side calculations (pre-upgrade) |

### Backend & Platform

| Layer | Technology |
|-------|-----------|
| Auth | Firebase (sign-up, login, account state) |
| User data | MongoDB (persisted budget numbers) |
| Payments | Stripe (premium upgrade) |
| Analytics | PostHog (event tracking, iteration-loop instrumentation) |
| Compliance | Privacy policy + data-collection compliance (live before any account, payment, or analytics event) |

---

## Screenshots

> Drop images into `docs/screenshots/` using the filenames below and they'll render automatically.

### Homepage
![NumiBright Homepage](docs/numibright.jpg)
