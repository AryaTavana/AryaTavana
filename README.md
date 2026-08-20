<p align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1020,50:2563EB,100:06B6D4&height=220&section=header&text=Arya%20Tavana&fontSize=52&fontColor=FFFFFF&animation=fadeIn&fontAlignY=38&desc=Full-Stack%20Product%20Developer&descAlignY=58&descSize=20" alt="Arya Tavana — Full-Stack Product Developer">
</p>

<p align="center">
  <a href="https://neowavechart.com/"><img src="https://img.shields.io/badge/NEoWave%20Chart-Live%20Product-2563EB?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Visit NEoWave Chart"></a>
  <a href="https://thoughthub-aryatavana.alwaysdata.net/"><img src="https://img.shields.io/badge/ThoughtHub-Live%20App-06B6D4?style=for-the-badge&logo=react&logoColor=white" alt="Visit ThoughtHub"></a>
  <a href="./RESUME.md"><img src="https://img.shields.io/badge/Resume-Read-0B1020?style=for-the-badge&logo=readme&logoColor=white" alt="Read my resume"></a>
  <a href="mailto:aryatavana07@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email Arya Tavana"></a>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=20&duration=3200&pause=1000&color=2563EB&center=true&vCenter=true&repeat=true&width=800&lines=Building+production+Django+products;Shipping+React+and+TypeScript+experiences;Designing+reliable+systems+for+real+users" alt="Building production Django products; Shipping React and TypeScript experiences; Designing reliable systems for real users">
</p>

## About me

I am a full-stack developer in Tehran, focused on turning complex product requirements into reliable, maintainable web platforms.

- Developer of [NEoWave Chart](https://neowavechart.com/), a production education, analysis, community, and commerce platform for serious NEoWave analysts.
- Creator of [ThoughtHub](https://github.com/AryaTavana/ThoughtHub), a Django and React publishing community with authoring and moderation workflows.
- Maintainer of [discourse-topic-reply-limits](https://github.com/AryaTavana/discourse-topic-reply-limits), an open-source Discourse plugin for subscription-aware reply quotas.
- Interested in product engineering, secure commerce, background processing, deployment automation, performance, and accessible interfaces.

## Flagship product — NEoWave Chart

<p align="center">
  <a href="https://neowavechart.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://neowavechart.com/static/images/LogoVW.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://neowavechart.com/static/images/LogoVB.svg">
      <img src="https://neowavechart.com/static/images/LogoVB.svg" width="560" alt="NEoWave Chart">
    </picture>
  </a>
</p>

<p align="center">
  An independent educational and technology platform that makes Glenn Neely's NEoWave methodology more accessible through structured learning, market research, expert Q&amp;A, community access, and specialized analytical tools.
</p>

<p align="center">
  <a href="https://neowavechart.com/"><strong>Website</strong></a> ·
  <a href="https://neowavechart.com/shop/pricing/"><strong>Plans</strong></a> ·
  <a href="https://neowavechart.com/neowave-qanda/"><strong>NEoWave Q&amp;A</strong></a> ·
  <a href="https://neowavechart.com/blog/"><strong>Research &amp; blog</strong></a> ·
  <a href="https://neowavechart.com/about-us/"><strong>About</strong></a>
</p>

### Product at a glance

| 26+ | 18 | 5 | 367 |
| :---: | :---: | :---: | :---: |
| Active students | Cash Data timeframes | Active product plans | Repository commits |

The live platform combines a public learning and research experience with authenticated memberships, product access, payments, support, and an integrated Discourse community. Its private production codebase contains 369 test methods, 87 schema migrations, and 56 server-rendered templates as of August 2026.

### What I engineered

<details open>
<summary><strong>Commerce, subscriptions, and entitlements</strong></summary>

- Product catalogue with categories, media, included benefits, ordering, duration-based pricing, and unlimited-access options.
- Cart and checkout flows with quantities, coupons, gift subscriptions, purchase snapshots, and customer receipts.
- Wallet and cryptocurrency-payment workflows with provider verification, reconciliation, idempotent fulfilment, refund handling, and administrator review paths.
- Central subscription entitlements for forum tiers, trading-signal access, forecasts, downloadable products, and protected video delivery.

</details>

<details>
<summary><strong>Accounts and member experience</strong></summary>

- Registration, login, password recovery, email verification, secure email changes, profiles, and an account dashboard.
- Support tickets, in-app notifications, branded transactional email, subscription status, gifts, downloads, signals, forecasts, and video access.
- Customer badges, score rewards, wallet conversion, review rewards, and recent-activity presentation.
- Responsive account navigation and consistent communication patterns for payments, access, support, and security events.

</details>

<details>
<summary><strong>Community, content, and growth</strong></summary>

- Discourse SSO with automated subscription-tier group synchronization and reply-limit entitlement integration.
- SEO-focused blog and forecasts, favorite posts, buffered view counters, sitemaps, robots directives, metadata, and structured data.
- Product comparison tables, FAQs, Trustpilot/customer reviews, contact workflows, policies, and educational pages.
- Accessible popup campaigns with scheduling, targeting, priority, multiple triggers, frequency controls, calls to action, and aggregate performance metrics.

</details>

<details>
<summary><strong>Production engineering</strong></summary>

- Django and Gunicorn behind Nginx, backed by PostgreSQL, Redis caching, Celery workers, and scheduled Celery Beat tasks.
- Docker-based services with health checks, immutable commit-tagged images, GitHub Actions CI/CD, production deployment, and rollback support.
- Automated database/media backups, encrypted off-site retention, checksums, and scheduled restore verification.
- CSP nonces, HTML sanitization, private response policies, rate limiting, Cloudflare Turnstile, upload validation, and server-side authorization.
- Anonymous page caching, responsive WebP images, self-hosted variable fonts, structured request metrics, and liveness/readiness monitoring.

</details>

### Production architecture

```text
Browser
  └── Nginx
        └── Django + Gunicorn
              ├── PostgreSQL          accounts, content, commerce, entitlements
              ├── Redis               cache, counters, task broker/results
              ├── Celery workers      email, notifications, sync, reconciliation
              ├── Celery Beat         scheduled operational tasks
              ├── Discourse           SSO, groups, subscription community
              └── Payment providers   checkout, wallet funding, fulfilment

GitHub Actions ── tests ── container build ── production deploy ── health check
```

<p>
  <img src="https://img.shields.io/badge/Django-6.0-092E20?style=flat-square&logo=django&logoColor=white" alt="Django 6.0">
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python 3.12">
  <img src="https://img.shields.io/badge/PostgreSQL-15-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL 15">
  <img src="https://img.shields.io/badge/Redis-7-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis 7">
  <img src="https://img.shields.io/badge/Celery-5-37814A?style=flat-square&logo=celery&logoColor=white" alt="Celery 5">
  <img src="https://img.shields.io/badge/Docker-Production-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Nginx-Reverse%20Proxy-009639?style=flat-square&logo=nginx&logoColor=white" alt="Nginx">
  <img src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

> NEoWave Chart is an independent product based on the methodology developed by Glenn Neely. It does not provide financial or investment advice.

## Other featured work

| Project | What it demonstrates | Stack |
| --- | --- | --- |
| [ThoughtHub](https://github.com/AryaTavana/ThoughtHub) · [Live site](https://thoughthub-aryatavana.alwaysdata.net/) | Full-stack publishing, block-based authoring, search, moderation, notifications, saved posts, and automatic LTR/RTL content direction. | Django REST Framework, React, TypeScript, PostgreSQL, Docker |
| [Discourse Topic Reply Limits](https://github.com/AryaTavana/discourse-topic-reply-limits) | Per-topic group quotas, subscription-cycle carryover, concurrent server-side enforcement, admin reporting, and audit history. | Ruby, Rails, Ember/Glimmer, PostgreSQL, RSpec |
| [React Learning](https://github.com/AryaTavana/React-Learning) | Routing, validated forms, data fetching, TypeScript modeling, Jest, and Testing Library exercises. | React, TypeScript, Vite, Tailwind CSS |
| [Bus Ticket Reservation](https://github.com/AryaTavana/Bus-Ticket-Reservation) | Linked-list data modeling, reservations, identity checks, lookup, and cancellation in a command-line program. | C, CMake |
| [AI/ML/DL Learning](https://github.com/AryaTavana/AI-ML-DL-Learning) | Iris classification with a k-nearest-neighbors model. | Python, scikit-learn |

## Technical toolkit

**Product and backend**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/Django%20REST-A30000?style=for-the-badge&logo=django&logoColor=white)
![Ruby](https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white)

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Data, infrastructure, and quality**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)

## Connect

<p align="center">
  <a href="mailto:aryatavana07@gmail.com"><strong>Email</strong></a> ·
  <a href="https://stackoverflow.com/users/21219212"><strong>Stack Overflow</strong></a> ·
  <a href="./RESUME.md"><strong>Resume</strong></a> ·
  <a href="https://neowavechart.com/"><strong>NEoWave Chart</strong></a> ·
  <a href="https://thoughthub-aryatavana.alwaysdata.net/"><strong>ThoughtHub</strong></a>
</p>

<p align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,50:2563EB,100:0B1020&height=110&section=footer" alt="Decorative gradient footer">
</p>
