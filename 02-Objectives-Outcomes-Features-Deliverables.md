# Vetobase AI: Project Description (Part 2 of 4)
## Objectives & Expected Outcomes, Key Features / Deliverables

---

## 1. Objectives

### 1.1 Overall goal
Make high-quality, AI-assisted customer service and messaging commerce **affordable and simple for small and medium online businesses**, so a small team can serve customers instantly across every channel and grow sales without proportionally growing headcount.

### 1.2 Specific objectives (next 12 months)

| # | Objective | How we will measure it |
|---|---|---|
| O1 | **Launch publicly** on the Shopify App Store and through self-serve sign-up on vetobase.com | App approved and listed; self-serve sign-up and onboarding live |
| O2 | **Let customers onboard themselves** to WhatsApp, Instagram, Messenger and Shopify without our team's help | Share of new workspaces fully connected without assistance; time from sign-up to first automated reply |
| O3 | **Automate the majority of routine conversations** for each customer | Share of inbound conversations resolved by AI or workflows without human handling (tracked per workspace) |
| O4 | **Cut first-response time to seconds** on all connected channels | Median first-response time before vs after onboarding |
| O5 | **Generate measurable revenue for customers** through order confirmations, cart recovery and campaigns | Attributed orders and revenue per workspace (campaign tracking and cart recovery) |
| O6 | **Build a sustainable recurring-revenue business** with international customers | Number of paying workspaces, monthly recurring revenue (MRR), churn |
| O7 | **Meet platform and data-protection requirements** (Meta, Shopify, GDPR-style privacy) | App approvals obtained; compliance webhooks, audit logging, encrypted backups and incident policy in place |

### 1.3 Targets (12-month horizon, to be validated during the programme)
These are **targets**, not current results:

- **Paying workspaces:** a first cohort of paying businesses from the Shopify App Store, direct sales and partners. 50+ paying installs would also make us eligible for Shopify's "Built for Shopify" quality programme.
- **Automation rate:** majority of routine questions (order status, product information, FAQs, confirmations) handled automatically for active customers.
- **First response:** under 1 minute for automated replies, 24/7.
- **Customer outcomes:** fewer unconfirmed or fake cash-on-delivery orders through WhatsApp confirmation, and recovered abandoned carts.

---

## 2. Expected Outcomes

### 2.1 For customer businesses
- **Time saved:** staff no longer copy-paste answers to repetitive questions; they focus on sales, exceptions and relationships.
- **Faster, 24/7 replies** on the channels customers already use, which means fewer lost sales.
- **More revenue:**
  - abandoned-cart recovery
  - instant product answers with buying links
  - WhatsApp campaigns with measurable conversion
- **Fewer failed deliveries and returns:** order confirmation before dispatch and proactive delivery updates.
- **Visibility:** what customers ask (intents), how the team performs, and which campaign earned how much.
- **One tool instead of several:** inbox, chatbot, automation, CRM, helpdesk, campaigns and analytics in one subscription.

### 2.2 For end customers
Instant, accurate answers (order status, availability, price, delivery time) on WhatsApp, Instagram, Messenger or the website, and a real person when it matters.

### 2.3 For the company and the ecosystem
- A **Pakistan-based software export** serving international customers (IT export revenue).
- **Skilled technical jobs** in AI, full-stack development, customer success and digital marketing.
- An **official integration partner** of major platforms: Meta (WhatsApp Business Platform tech provider) and Shopify (App Store partner).

---

## 3. Key Features / Deliverables

Status legend: ✅ **Built & live**, 🧪 **Built, in testing / pre-launch**, 🛠️ **Planned in this project period**

### 3.1 Channels and unified inbox
| Feature | Status | Description |
|---|---|---|
| WhatsApp Business (Cloud API) | ✅ | Two-way messaging, media, templates, multiple numbers per workspace |
| Instagram DMs | ✅ | Direct messages in the same inbox |
| Instagram post comments | ✅ | View, reply to, hide and delete comments on posts and reels from one screen |
| Facebook Messenger | ✅ | Page messages in the same inbox |
| Website chat widget | ✅ | Embeddable widget for any website, plus a Shopify theme app embed (one-click enable) |
| Unified real-time inbox | ✅ | Live updates, unread counts, filters by channel and intent, team presence |
| WhatsApp 24-hour window handling | ✅ | Shows the session window, sends reminders before expiry, uses templates outside the window |
| Multi-connection workspaces | ✅ | Several WhatsApp numbers, Instagram accounts or stores per workspace, within plan limits |
| Self-serve WhatsApp onboarding (Meta Embedded Signup) | 🛠️ | Customer connects their own number in a Meta popup; no manual setup |

### 3.2 AI layer
| Feature | Status | Description |
|---|---|---|
| Intent detection and smart labels | ✅ | Every message classified (order status, refund, product inquiry, complaint, bulk order and so on); labels are configurable per workspace |
| AI agents | ✅ | Create agents in natural language; each has its own instructions, knowledge base and outputs (for example order number, reason). Examples: Order Support, Sales & Recommendations, Returns & Refunds, FAQ & Store Info, Abandoned Cart Recovery |
| Store-aware answers | ✅ | Agents use order, product and tracking data to answer "where is my order", "is it in stock", "how much" |
| Sentiment analysis | ✅ | Every message is tagged positive, neutral or negative alongside its intent; sentiment is tracked in analytics, and complaint-intent messages can trigger escalation flows |
| Human handoff | ✅ | AI hands the chat to the team with a ticket, a notification and full context |
| Product recognition from images | 🛠️ | Customer sends a product photo; the AI identifies it and replies with price, availability and a buying link |
| Multilingual replies (for example Urdu, Arabic) | 🛠️ | Answers in the customer's language |
| AI quality evaluation suite | 🛠️ | Automated tests on real conversation samples to monitor answer accuracy before changes ship |

### 3.3 Visual automation builder (no-code workflows)
| Feature | Status | Description |
|---|---|---|
| Visual flow editor | ✅ | Drag-and-connect builder with branching, per channel (WhatsApp, Instagram, Messenger, Website) |
| Triggers | ✅ | AI-detected intent; store events (new order, abandoned checkout); customer inactivity; chat-expiry reminder |
| Messaging blocks | ✅ | Custom message, WhatsApp template, message with reply buttons |
| Query-resolution blocks | ✅ | "Query resolved?" yes/no branches, inactivity control (restart/stop intervals) |
| Flow & AI blocks | ✅ | AI condition (branch on intent), AI agent step, confirmation agent |
| Support blocks | ✅ | System notification, support ticket, notify human, ticket routing |
| Commerce blocks | ✅ | Shopify order lookup (filter + branch), courier tracking (PostEx), confirm order and cancel order (Shopify tags) |
| Ready-made flows | ✅ | Order confirmation, abandoned-cart recovery, delivery delay → priority ticket, return & refund assistant, negative-sentiment escalation, welcome menu, inactivity nudge, 24h window reminder, bulk/wholesale lead routing |
| Flow analytics | ✅ | Automation run history per flow |

### 3.4 Commerce integrations
| Feature | Status | Description |
|---|---|---|
| Shopify (direct connection) | ✅ | Orders, products and checkouts synchronised in real time with webhooks; abandoned-checkout detection; order tagging from workflows |
| Shopify App Store app | 🧪 | Embedded app installed from the Shopify App Store: secure token-exchange install with automatically refreshing access tokens, automatic workspace creation, Shopify billing, storefront chat widget (theme app embed), mandatory privacy (GDPR) webhooks, link to an existing Vetobase workspace. Built and tested end-to-end on a Shopify development store; submission pending |
| PostEx courier (Pakistan) | ✅ | Tracking sync every 15 minutes; delivery status available to agents and workflows |
| WooCommerce | 🛠️ | Same order, product and abandoned-cart features for WooCommerce stores |
| Additional couriers / carriers | 🛠️ | Pluggable tracking providers for international markets |

### 3.5 CRM, operations and team
| Feature | Status | Description |
|---|---|---|
| Customer CRM | ✅ | Customer profiles with order history, spend, refunds and conversations |
| Orders view | ✅ | Orders, analytics and abandoned checkouts in one place |
| Order-tracking boards | ✅ | Configurable orders, production and stock boards with ideal timelines (built for made-to-order fashion) |
| Tickets | ✅ | Support tickets with status, assignee, priority and soft-delete audit |
| Notifications | ✅ | Priority-levelled notifications from AI and workflows |
| Team & roles | ✅ | Admin/member roles with page-level permissions; read-only demo or test memberships |
| Multi-workspace platform admin | ✅ | Platform-level administration of workspaces and limits |

### 3.6 Marketing and analytics
| Feature | Status | Description |
|---|---|---|
| WhatsApp marketing campaigns | ✅ | Template campaigns with per-recipient tracking: sent → delivered → read → link clicked → order placed |
| Revenue attribution | ✅ | Orders matched to campaign recipients within a tracking window; revenue and conversion rate per campaign |
| Analytics dashboard | ✅ | Customer sentiment, chat volume by channel, top intents, automation runs, AI agent reply volume, team performance |
| Campaign segmentation & A/B testing | 🛠️ | Target by tags, purchase history and intent; compare template variants |

### 3.7 Security, privacy and compliance
| Feature | Status | Description |
|---|---|---|
| Workspace isolation and role-based access | ✅ | Every API request scoped to the caller's workspace; page-level permissions |
| Encryption | ✅ | HTTPS everywhere; integration tokens and secrets encrypted at rest (AES-256-GCM) |
| Webhook verification | ✅ | HMAC signature verification on store webhooks; invalid requests rejected |
| Privacy (GDPR) request handling | ✅ | Automated data export and erasure for customer and shop redaction requests, with an audit trail |
| Data-access audit log | ✅ | Logs who accessed customer data, when, and through which endpoint |
| Encrypted daily backups | ✅ | Nightly AES-256 encrypted database backups with 14-day retention; restore tested |
| Incident response policy | ✅ | Documented detection, containment and notification process |

### 3.8 Go-to-market deliverables
| Deliverable | Status |
|---|---|
| Marketing website with pricing, terms, privacy and refund policies | ✅ |
| 13 use-case landing pages and 12 SEO blog articles (WhatsApp automation, Instagram DM automation, Shopify support, AI agents, CRM and so on) | ✅ |
| Animated product demo film (landscape) and vertical Instagram Reel cut | ✅ |
| Fully populated demo workspace for sales demos and reviewers | ✅ |
| Shopify App Store listing (texts, screenshots, screencast) | 🧪 |
| International payment processing for direct subscriptions | 🛠️ |
| Self-serve sign-up, onboarding wizard and in-app guides | 🛠️ |

*(Continued in Part 3: Implementation Plan & Timeline, Resources or Requirements.)*
