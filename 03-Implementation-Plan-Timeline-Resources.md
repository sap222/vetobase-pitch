# Vetobase AI: Project Description (Part 3 of 4)
## Implementation Plan & Timeline, Resources or Requirements

---

## 1. Implementation Approach

We work in **short, shippable increments**. Each feature is built, tested against real conversations from partner brands, deployed to production, and then generalised for all customers. The core platform is already built and live, so this project period focuses on:

1. **Launch readiness:** marketplace approvals, self-serve onboarding, international billing.
2. **Product depth:** AI accuracy, new integrations (WooCommerce, more couriers), multilingual support, image recognition.
3. **Growth:** Shopify App Store distribution, content and SEO, agency partnerships, a customer-success process.
4. **Scale and trust:** reliability, monitoring, security and privacy controls that meet marketplace and enterprise expectations.

---

## 2. Technical Architecture (current)

| Layer | Technology | Notes |
|---|---|---|
| Frontend (customer app) | React single-page app | Unified inbox, flow builder, CRM, analytics; real-time updates over WebSockets |
| Backend API | Node.js + Express | REST API, webhook receivers (Meta, Shopify), workflow engine, schedulers (Shopify poller, courier sync, chat lifecycle) |
| Real-time | Socket.IO | Per-workspace rooms for live messages, orders, presence |
| AI services | Anthropic Claude models; Python LangChain service for AI agents | Intent + sentiment classification per message; AI agents with per-agent instructions, knowledge and structured outputs |
| Database | MongoDB | Multi-tenant data model: every record scoped to a workspace |
| Integrations | Meta WhatsApp Cloud API, Instagram Messaging API, Messenger Platform; Shopify Admin GraphQL API; PostEx courier API | Official APIs only |
| Shopify App Store app | Embedded app (App Bridge) + theme app extension | Token-exchange install with expiring, auto-refreshing tokens; Shopify billing; mandatory privacy webhooks |
| Hosting | Linux cloud server (VPS) behind Nginx with HTTPS; process manager for services | Static frontend; isolated services; nightly encrypted backups |
| Marketing site | React site with static SEO pages (use cases, blog), sitemap, robots and llms.txt | Hosted separately; auto-deploys from source control |

```
            ┌──────────── Customers' channels ────────────┐
            WhatsApp    Instagram    Messenger    Website widget
                 │           │           │              │
                 ▼           ▼           ▼              ▼
          ┌─────────────────────────────────────────────────┐
          │  Backend API (Node/Express) + webhook receivers  │
          │  • workflow engine   • schedulers & pollers      │
          │  • campaigns & tracking • privacy webhooks       │
          └───────┬───────────────┬───────────────┬─────────┘
                  │               │               │
          AI services        MongoDB          Store & courier
   (Claude intent/sentiment, (multi-tenant,    (Shopify GraphQL,
    LangChain AI agents)      encrypted        PostEx; WooCommerce
                              secrets)         planned)
                  │
                  ▼
     React app (unified inbox, flows, CRM, analytics) via Socket.IO
```

---

## 3. Work Completed to Date (March – September 2026)

| Period | Milestone (completed) |
|---|---|
| Mar–Apr 2026 | Core platform: multi-tenant workspaces, authentication, real-time inbox. WhatsApp Cloud API and Instagram channels. Shopify connection (orders, checkouts, webhooks). Intent detection with AI labels. First versions of the workflow engine and AI agents. Tickets, notifications, website chat widget, team presence |
| May–Jun 2026 | Visual automation builder and AI agents expanded. Facebook Messenger channel. PostEx courier tracking. Team management. WhatsApp templates. Order confirmation and abandoned-cart flows |
| Jul 2026 | Instagram comment moderation (reply/hide/delete). Order-handling improvements |
| Aug 2026 | Roles and page-level permissions. WhatsApp campaigns with click/order/revenue attribution. Order-tracking boards (orders/production/stock). Analytics expansion. Ticket and notification audit (soft delete) |
| Sep 2026 | Complete UI redesign. Demo workspaces. Marketing website with pricing, legal pages, use-case pages and blog. Product demo film. **Shopify App Store app built and tested end-to-end:** embedded install, expiring tokens, Shopify billing, theme app embed chat widget, privacy webhooks, abandoned carts via GraphQL. **Security hardening:** cross-workspace access fix, data-access audit log, encrypted nightly backups, incident response policy |

The platform has been **in production use with partner brands**, including a fashion brand with two live Shopify stores. Real conversations and orders from these brands shaped the AI labels, agents and workflows.

---

## 4. Implementation Plan & Timeline (12 months: October 2026 – September 2027)

### Phase 1: Launch readiness (Months 1–2, Oct–Nov 2026)
| Workstream | Deliverables | Exit criteria |
|---|---|---|
| Shopify App Store | Submit the built app with listing, screenshots and screencast; respond to review feedback | App approved and publicly listed |
| International billing | Set up a merchant-of-record payment provider (Paddle / Polar / 2Checkout) for direct subscriptions, with tax handling; Shopify billing for App Store merchants | Live checkout for direct customers; first international payment received |
| WhatsApp self-onboarding | Meta Embedded Signup so each customer connects their own WhatsApp Business number in a popup | A new workspace connects its own number without our help |
| Website positioning | Final pricing, onboarding pages, demo film, legal pages | Ready for paid traffic and review teams |

### Phase 2: Self-serve product and depth (Months 3–5, Dec 2026 – Feb 2027)
| Workstream | Deliverables | Exit criteria |
|---|---|---|
| Self-serve onboarding | Sign-up, guided setup wizard (channels → store → AI agent → first workflow), in-app checklists and templates | New customers reach a first automated reply within the first session |
| WooCommerce integration | Orders, products, abandoned carts and order actions for WooCommerce stores | Feature parity with Shopify for core flows |
| AI quality | Evaluation suite on anonymised conversation samples; guardrails; confidence-based handoff tuning | Measured accuracy tracked release by release |
| Multilingual AI | Replies in the customer's language (starting with English, Urdu and Arabic) | Language detected and handled in agents and templates |
| Campaign upgrades | Segmentation (tags, purchase history, intent), scheduling, A/B template tests | Campaigns targetable by segment, with variant reporting |

### Phase 3: Growth (Months 6–8, Mar – May 2027)
| Workstream | Deliverables | Exit criteria |
|---|---|---|
| Distribution | Shopify App Store optimisation (reviews, listing tests); content/SEO programme; partnerships with Shopify and Meta agencies | Steady weekly install and trial flow |
| Customer success | Onboarding calls, help centre, response-time SLAs, churn monitoring | Retention and activation tracked per cohort |
| Image recognition | Customer sends a product photo → AI identifies the catalogue item and replies with price, availability and link | Live for Shopify and WooCommerce catalogues |
| More couriers | Pluggable tracking providers for target markets | At least two additional international carriers |

### Phase 4: Scale and trust (Months 9–12, Jun – Sep 2027)
| Workstream | Deliverables | Exit criteria |
|---|---|---|
| Infrastructure | Managed database with replicas, horizontal scaling of the API and AI services, uptime monitoring and alerting, staging environment | High-availability setup; monitored uptime target |
| Security & compliance | Data-retention controls, data processing agreement (DPA) for customers, access reviews, penetration test; Shopify "Built for Shopify" requirements | Marketplace and enterprise security questionnaires answerable |
| New channels and features | Additional channels (for example Telegram and email) where customers ask for them; mobile-friendly agent experience | Shipped based on customer demand |
| Regional expansion | GCC (UAE/Saudi Arabia) go-to-market with Arabic support | First customers in the region |

### Timeline at a glance

```
2026            Oct   Nov   Dec   2027 Jan   Feb   Mar   Apr   May   Jun   Jul   Aug   Sep
Phase 1 Launch  ████████████
Phase 2 Depth               ██████████████████
Phase 3 Growth                                 ██████████████████
Phase 4 Scale                                                    ████████████████████████
Milestones      ▲App Store   ▲Billing    ▲Self-serve  ▲WooCommerce  ▲Image AI     ▲HA infra
                 submission   live        onboarding   live          live          & DPA
```

---

## 5. Resources or Requirements

### 5.1 Team

| Role | Current | Needed during the project | Responsibility |
|---|---|---|---|
| Founder / product & engineering lead (Omar Faiz) | ✅ | — | Product direction, architecture, AI, partner relationships |
| Full-stack engineer(s) | Partly covered by the founder | +1–2 | Integrations (WooCommerce, couriers), onboarding, campaigns, scaling |
| AI / ML engineer | Covered by the founder | +1 (part-time to start) | Agent quality, evaluation suite, multilingual and image recognition |
| Customer success & onboarding | — | +1 | Onboarding, support, help centre, feedback loop |
| Growth / digital marketing | — | +1 | Shopify App Store optimisation, content/SEO, paid acquisition, partnerships |
| Design (part-time / contract) | — | As needed | UX for onboarding, marketing assets |

### 5.2 Technology and services

| Requirement | Purpose | Cost behaviour |
|---|---|---|
| Cloud hosting (application servers, managed database, backups, monitoring) | Run the platform reliably as customer numbers grow | Grows with customers; moves from a single server to a high-availability setup in Phase 4 |
| AI model usage (Anthropic Claude) | Intent, sentiment, AI agents, image recognition | Usage-based; grows with message volume. Controlled by model choice, caching and short prompts |
| Meta WhatsApp Business Platform | WhatsApp messaging for customers | Conversation fees are paid by each customer on their own WhatsApp Business account; no platform fee for us |
| Shopify Partner programme | App Store distribution and billing | No listing fee; revenue share applies to App Store subscriptions |
| Payment provider (merchant of record) | International subscriptions with tax handling | Percentage fee per transaction |
| Domains, email, design and analytics tools | Operations and marketing | Small fixed monthly costs |
| Security testing | Penetration test and security review (Phase 4) | One-off |

### 5.3 Non-financial support that would accelerate the project
- **Mentorship and introductions** to e-commerce brands, Shopify and Meta agencies, and international customers (UK, US, GCC).
- **Guidance on international payments, IT-export registration (PSEB) and export-proceeds compliance** for a Pakistan-registered SaaS company.
- **Legal support** for international terms of service, data processing agreements and privacy compliance.
- **Cloud and AI credits** to fund hosting and AI usage during the growth phase.
- **Visibility:** demo days, investor and partner introductions, media.

### 5.4 Existing assets we bring
- A working, production-tested product with live integrations (WhatsApp, Instagram, Messenger, website, Shopify, courier).
- A Shopify App Store app built and tested end-to-end, with billing and privacy compliance.
- A registered company (Vetobase SMC Private Limited) with business verification on Meta's platform.
- Partner brands using the product, providing real-world feedback.
- A marketing website, SEO content library, demo workspace and product films ready for launch.

*(Continued in Part 4: Potential Challenges or Risks, Business Model, Additional Details.)*
