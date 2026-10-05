# Vetobase AI: Project Description (Part 4 of 4)
## Potential Challenges or Risks, Business Model, Additional Details

---

## 1. Potential Challenges or Risks

Each risk is rated for **likelihood (L)** and **impact (I)** as High / Medium / Low, with the mitigation in place or planned.

### 1.1 Platform and partner dependency

| Risk | L | I | Mitigation |
|---|---|---|---|
| **Meta policy or API changes** (WhatsApp, Instagram, Messenger) affect messaging features or pricing | M | H | We use only official APIs and follow messaging rules: 24-hour window handling, approved templates, opt-in. Business verification on Meta's platform is complete. A channel-adapter architecture limits the impact of API changes to one module |
| **Meta approval steps** for self-serve onboarding (Embedded Signup / tech-provider requirements) take longer than planned | M | M | Business and tech-provider verification are already done. Until self-serve onboarding is live, we onboard customers' WhatsApp numbers with assisted setup |
| **Shopify App Store review** requests changes or rejects the app (billing, permissions, UX) | M | M | The app was built to the published App Store requirements: embedded install via token exchange, expiring tokens, Shopify billing, minimal permissions, theme app extension instead of theme edits, mandatory privacy webhooks, HMAC verification. We respond quickly to each review item |
| **Shopify API version changes** | M | L | Pinned API versions with a scheduled upgrade each release cycle; GraphQL-first client |

### 1.2 Commercial and market

| Risk | L | I | Mitigation |
|---|---|---|---|
| **International payment collection from Pakistan** (some providers do not onboard Pakistan-registered companies; one provider already declined us) | H | H | Apply to several merchant-of-record providers in parallel (Paddle, Polar, 2Checkout). Use Shopify billing for App Store merchants, which pays out to our bank. Register as an IT exporter (PSEB) and receive proceeds through an export account |
| **Competition** from established inbox, chatbot and helpdesk tools (Gorgias, Tidio, Zendesk, ManyChat, WATI, Interakt and others) | H | M | Differentiate on **all channels + store + courier + AI agents + campaigns with revenue attribution in one affordable product**, especially for WhatsApp-first and cash-on-delivery markets. Win specific niches (fashion D2C, COD markets) with ready-made flows |
| **Customer acquisition cost** higher than planned | M | M | Lean on organic channels: Shopify App Store search, SEO content (13 use-case pages, 12 articles already published), the product films, partner referrals and agency partnerships. Measure activation before scaling paid ads |
| **Concentration on a few early customers** | M | M | Broaden the base through public launch and self-serve onboarding; productise features first built for partners |
| **Pricing too high for small merchants in some markets** | M | M | A lower entry plan on the Shopify App Store alongside the full plan; usage-based plan options under evaluation |

### 1.3 Technical and AI

| Risk | L | I | Mitigation |
|---|---|---|---|
| **AI gives a wrong or made-up answer** | M | H | Answers are grounded in the business's own data (orders, products, tracking) and instructions. Agents are constrained to their task. Low-confidence intent results are not acted on automatically, and complaint-intent messages escalate to the team. An evaluation suite on anonymised samples is planned (Phase 2). Businesses can turn the AI off per flow or channel |
| **AI usage costs grow with volume** | M | M | Use the smallest suitable model per task (fast models for classification, larger only where needed), keep prompts short, cache repeated data, and set per-plan fair-use limits |
| **Scaling and reliability** (single-server setup today) | M | H | Nightly encrypted backups with tested restore. The Phase 4 move to a managed database with replicas, horizontally scaled services, monitoring and alerting, and a staging environment |
| **Third-party outages** (AI provider, Meta, Shopify) | M | M | Webhooks are acknowledged immediately and processed idempotently (records upserted by ID), and the platforms retry failed deliveries. Messages still reach the inbox when the AI service is unavailable. Durable job queues are planned with the Phase 4 infrastructure work |
| **Security breach or data leak** | L | H | Workspace isolation on every request, role-based permissions, encrypted secrets (AES-256-GCM), HMAC-verified webhooks, data-access audit logging, encrypted backups and a written incident response policy. External penetration test planned (Phase 4) |

### 1.4 Legal, privacy and regulatory

| Risk | L | I | Mitigation |
|---|---|---|---|
| **Data-protection obligations** (GDPR for EU/UK customers, platform data rules such as Shopify's protected customer data) | M | H | Privacy policy and terms published. Automated handling of data export and erasure requests, with an audit trail. Data minimisation. Retention controls and a data processing agreement planned (Phase 4) |
| **Messaging consent and anti-spam rules** for campaigns | M | M | WhatsApp template approval, opt-in requirements, opt-out handling; campaigns positioned for opted-in customers only |
| **Export-proceeds and tax compliance in Pakistan** | M | M | Bank-channel receipts tagged as IT exports; PSEB registration; professional tax advice |

### 1.5 Team and execution

| Risk | L | I | Mitigation |
|---|---|---|---|
| **Key-person dependency** (small founding team) | H | H | Documentation of architecture, deployment and security procedures. Planned hires in engineering, customer success and growth (see Part 3). Code under version control with automated tests for critical paths |
| **Scope creep** from custom partner requests | M | M | Productise only features useful to many customers; keep a public roadmap and a phased plan |

---

## 2. Business Model

### 2.1 Revenue streams
| Stream | Description |
|---|---|
| **Direct subscription** | Monthly per-workspace subscription sold on vetobase.com. **Business plan: USD 100 per month**, covering all channels, AI agents, the automation builder, CRM, tickets, campaigns and analytics |
| **Shopify App Store subscription** | Plan billed through Shopify for merchants who install from the App Store. **Introductory price: USD 20 per month** with a free trial. Prices can be adjusted as the product matures |
| **Future add-ons** (under evaluation) | Extra channels/numbers or stores beyond plan limits, higher AI usage tiers, onboarding and setup services for larger brands |

### 2.2 Unit economics (drivers)
- **Main variable costs:** AI model usage per message, hosting, and payment or marketplace fees.
- **WhatsApp conversation fees** are paid by each customer on their own WhatsApp Business account, not by Vetobase.
- **Revenue grows per workspace** with additional channels, stores and AI usage, while infrastructure is shared across all workspaces.

### 2.3 Go-to-market
1. **Shopify App Store:** organic discovery by merchants searching for WhatsApp, chat and AI support apps.
2. **Content and SEO:** use-case pages and articles targeting searches such as "WhatsApp automation", "Instagram DM automation", "Shopify customer support" and "AI agents for business" (already published).
3. **Product films and social media:** a landscape demo film on the website and a vertical cut for Instagram Reels.
4. **Partnerships:** Shopify and Meta agencies, e-commerce consultants, and partner brands as references.
5. **Direct sales and demos:** a fully populated demo workspace shows every feature in minutes.

---

## 3. Additional Details

### 3.1 Company
| | |
|---|---|
| Legal name | Vetobase SMC Private Limited |
| Country of registration | Pakistan |
| Website / product | https://www.vetobase.com · https://app.vetobase.com |
| Demo film | https://www.vetobase.com/watch/ |
| Platform verifications | Business verification on Meta's platform completed |
| Contact | support@vetobase.com |

### 3.2 Team
| Name | Role | Background |
|---|---|---|
| Omar Faiz | Founder & CEO (product, engineering, AI) | Designed and built the Vetobase AI platform end to end: the multi-channel messaging integrations, AI agents and intent engine, automation builder, Shopify App Store app and security controls. Leads product, engineering and partner relationships |

### 3.3 Traction and validation
- **Built and live in production** since spring 2026, used by partner brands in fashion and retail.
- **Live store integration:** a partner fashion brand runs two Shopify stores connected to WhatsApp, with real-time order and status synchronisation.
- **Real-world tuning:** intent labels, AI agents and workflows (order confirmation, delivery updates, returns, abandoned carts) were shaped by real customer conversations.
- **Shopify App Store app** installed, connected, billed (test charge) and the storefront chat widget enabled on a Shopify development store.
- **Launch assets ready:** website, pricing, legal pages, SEO content, demo workspace and product films.

*(Add specific metrics where available: number of active workspaces, messages handled, automated-reply share, orders confirmed, campaign revenue attributed.)*

### 3.4 Data protection and security summary
- HTTPS everywhere; integration tokens and secrets encrypted at rest (AES-256-GCM).
- Strict workspace isolation; role- and page-level permissions; read-only demo or test memberships.
- HMAC verification for store webhooks; invalid requests rejected.
- Automated privacy request handling (customer data export, customer and shop erasure) with an audit trail.
- Data-access audit log (who accessed customer data, when, from where).
- Nightly AES-256 encrypted database backups, 14-day retention, restore verified.
- Documented security incident response policy, with notification to affected merchants and platforms within 72 hours of a confirmed breach.

### 3.5 Social and economic impact
- **Software exports:** a Pakistan-based SaaS earning recurring revenue from international customers.
- **Skilled jobs:** engineering, AI, customer success and digital marketing roles.
- **Small-business enablement:** small brands get enterprise-grade, AI-assisted customer service at an affordable price, so they can compete with larger retailers.
- **Better customer experience:** fast, accurate answers on the channels people already use.

### 3.6 Why we will succeed
1. **The product already exists and works in production.** This project period is about launch and scale, not about proving the idea from scratch.
2. **It's built on real problems** from real brands, especially WhatsApp-first and cash-on-delivery commerce.
3. **It's broad but focused:** channels, store, courier, AI agents, automation, CRM, campaigns and analytics in one tool aimed at small and medium online businesses.
4. **It's compliance-ready:** built to the Meta and Shopify platform requirements, with privacy and security controls already in place.
5. **It has a clear, phased plan** with measurable milestones over 12 months (see Part 3).

---

*End of the 4-part project description.*
