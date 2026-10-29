# Hi, I'm Khalil 👋

**Full Stack Developer — Laravel / Vue.js** · Sousse, Tunisia · Open to remote and relocation

I build SaaS platforms end to end: REST APIs, Vue 3 frontends, payments, real-time features and media pipelines. 4 years in production, from system design to deployment.

---

## 🎬 Subscription platform for content creators — Project Lead & Lead Developer

Led from scratch to production: product design, architecture, development and deployment. **100,000+ active users.**

**Architecture: 3 isolated services**
- **Laravel API + Vue 3 / TypeScript SPA**: 232 API routes, 279 Vue components, Pinia, Vite
- **Node.js real-time server**: Express, Socket.IO with Redis adapter (multi-instance), Bull queues, PM2
- **Node.js video microservice**: Express, BullMQ, FFmpeg, AWS SDK, with a callback to Laravel when a video is ready

**Real-time chat**
- Messages and files, reactions, typing indicator, read receipts, online presence, catch-up after a disconnection
- Reliable delivery: Socket.IO acknowledgements with retry, HTTP fallback, idempotency keys against duplicates
- Message sending cut from **34 to 12 database queries** (1.4 s → 0.69 s); conversation list at 50,000 conversations from **4.1 s to 9 ms**
- AI auto-replies with OpenAI GPT-4o, scheduled follow-ups and per-creator settings

**Media on AWS**
- Direct browser-to-**S3** uploads with pre-signed URLs, and resumable chunked uploads for large files
- **CloudFront** CDN with time-limited signed URLs for private content and targeted cache invalidation
- Replaced **AWS MediaConvert** with an in-house transcoding pipeline: adaptive **HLS** (360p to 1080p), previews, thumbnails; 1080p encoding **101 s → 76 s**
- Responsive WebP images (srcset), BlurHash placeholders, shared hls.js player with device-based quality

**Payments**
- **Stripe, Viva Wallet, Segpay and CCBill**: subscriptions, pay-per-media, paid chat media, tips, 6 currencies, per-country VAT
- Two live provider migrations (Stripe → Viva Wallet → CCBill) without interrupting running subscriptions
- Signed payment references and double-credit protection; creator balances and payouts with double validation

**Back-office, trust & safety**
- Admin rebuilt in 8 batches (134 routes, 27 screens): roles and permissions, audit log, dashboard
- Moderation queue with automated image moderation (Sightengine), reports and sanctions
- Identity verification (KYC) with interchangeable providers, age verification, security hardening (SQL injection tests, CSP)

**Also**
- Firebase push notifications with anti-spam rules, e-mail campaigns, creator statistics, scheduled posts, reels
- Technical SEO (server pre-rendering, 301 redirects, sitemaps) and 6 languages
- Docker, Nginx, Redis, Supervisor (5 priority queues), GitHub Actions CI/CD, Cloudflare, Telescope monitoring
- **1,369 PHPUnit tests** and 67 Cypress / Puppeteer scenarios

---

## 🖥️ HostStronger — hosting platform (VPS, domains, web hosting)

Worked on HostStronger, a hosting platform built by a 5-developer team: automated VPS provisioning on Proxmox, Stripe subscription billing, domains, web hosting and website-building workflows, with real-time status updates (Laravel 10, Vue 3 / TypeScript).

**My contributions**
- **Domains**: registration, availability checks and domain management on a third-party registrar API
- **DNS**: end-to-end zone management (create, list, update, reset, delete), synchronised with the local database
- **Domain contacts**: detailed model, repository, validation, registrar sync and a typed Vue 3 / TypeScript page
- **Websites**: SitePro site backup, restore and publishing; domains linked to sites hosted on CyberPanel
- **Customer area**: about 10 customer pages, Sanctum login, admin "log in as customer", PDF invoice download
- **Forms**: international phone input with country-filtered dial codes and libphonenumber validation

---

## 🤖 AI proof of concept

Immigration document classification with OpenAI GPT-4o behind a self-hosted n8n layer (Laravel 12, Vue 3, PostgreSQL 16), delivered in 2.5 weeks, with a 6-language interface including right-to-left scripts.

---

### Tech stack
**Backend:** PHP 8, Laravel, Node.js, Express, REST APIs, Redis queues
**Frontend:** Vue 3, TypeScript, Pinia, Vite, Tailwind CSS, PrimeVue
**Real-time & media:** Socket.IO, BullMQ, FFmpeg, HLS
**Data:** PostgreSQL, MySQL, Redis, MongoDB
**Cloud / DevOps:** AWS (S3, CloudFront), Docker, Nginx, Cloudflare, GitHub Actions
**AI:** OpenAI API, n8n, AI-assisted development with Claude Code

### Contact
[LinkedIn](https://www.linkedin.com/in/khalil-bouhdida-301587219) · khalil.bh130@gmail.com

> Most of my work lives in private repositories. Happy to walk you through the architecture and code in an interview.
