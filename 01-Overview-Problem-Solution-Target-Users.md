# Vetobase AI: Project Description (Part 1 of 4)
## Project Overview, Problem Statement, Proposed Solution and Target Users

| | |
|---|---|
| **Project** | Vetobase AI, an AI customer-support and automation platform for online businesses |
| **Organisation** | Vetobase SMC Private Limited (registered in Pakistan) |
| **Website** | https://www.vetobase.com |
| **Product (live)** | https://app.vetobase.com |
| **Product demo film** | https://www.vetobase.com/watch/ |
| **Stage** | Product built and live in production with partner brands; preparing for public launch (Shopify App Store, self-serve onboarding, international billing) |
| **Development started** | March 2026 |

### Contents of this 4-part submission
1. **Part 1 (this file):** Project Overview & Problem Statement, Proposed Solution, Target Users
2. **Part 2:** Objectives & Expected Outcomes, Key Features / Deliverables
3. **Part 3:** Implementation Plan & Timeline, Resources or Requirements
4. **Part 4:** Potential Challenges or Risks, Business Model, Additional Details

---

## 1. Project Overview

Vetobase AI is a software-as-a-service (SaaS) platform that gives online businesses one place to handle every customer conversation, with AI doing most of the repetitive work.

It connects a business's **WhatsApp Business**, **Instagram** (DMs and post comments), **Facebook Messenger** and **website chat** into a single shared team inbox. It also connects the business's **online store** (Shopify today) and its **courier** (PostEx today). Once connected:

- **AI reads every incoming message.** It detects the customer's intent (order status, refund, product question, complaint, bulk order and so on) and applies labels automatically.
- **AI agents reply on the business's behalf.** Each agent is created by describing it in plain language and has its own instructions and knowledge base. Agents answer order-status questions from live store data, recommend products, collect leads and resolve routine issues 24/7.
- **A visual automation builder** lets the business design customer flows without code. Examples:
  - order confirmations on WhatsApp
  - abandoned-cart recovery
  - delivery-delay escalation
  - return and refund handling
  - negative-sentiment escalation
  - inactivity nudges
  - reminders before WhatsApp's 24-hour messaging window closes
- **People step in only when needed.** The AI hands complex cases to a team member with full context, and creates a ticket and a notification.
- **Behind the scenes** it provides:
  - a CRM (customers, orders, chats, tickets)
  - team roles and permissions
  - WhatsApp marketing campaigns with click, order and revenue attribution
  - an analytics dashboard (sentiment, chat volume, top intents, team performance)

Our positioning is **"The AI system that runs your business with you."** Vetobase AI does not replace the team. It removes the repetitive work so a small team can serve many more customers, faster, across every channel.

---

## 2. Problem Statement

### 2.1 The situation
Online businesses, especially direct-to-consumer (D2C) and e-commerce brands, now sell and support customers through **messaging apps** rather than email or phone. WhatsApp, Instagram DMs and Messenger are where customers ask:

- *"Where is my order?"*
- *"Is this available in medium?"*
- *"How much is this?"*
- *"I want to return this."*
- *"My parcel arrived damaged."*

Most of these questions are **repetitive**, **time-sensitive**, and **answerable from data the business already has** (its store, orders and courier tracking).

### 2.2 The problems

| # | Problem | Impact on the business |
|---|---|---|
| 1 | **Conversations are scattered** across WhatsApp, Instagram, Messenger and the website, often on separate phones and logins | Missed messages, slow replies, no shared view of a customer, no accountability |
| 2 | **Most questions are repetitive** (order status, sizes, prices, delivery times, return policy) | Staff spend most of their day copy-pasting answers instead of selling or solving real problems |
| 3 | **Support doesn't scale** without hiring | Every growth spike, sale or campaign means more agents, more cost and longer response times |
| 4 | **Response time loses sales** | Customers who don't get a fast answer on WhatsApp or Instagram buy elsewhere; abandoned carts are rarely followed up |
| 5 | **Messaging and store data are disconnected** | Agents switch between the inbox, Shopify admin and the courier portal to answer one question |
| 6 | **Messaging-platform rules are complex** (WhatsApp's 24-hour window, template approval, opt-in) | Businesses break rules unknowingly or miss the window and lose the conversation |
| 7 | **No visibility** into what customers are asking, which campaigns convert, or how the team performs | Decisions are based on guesswork |
| 8 | **Existing tools are fragmented or expensive** | A shared inbox, a chatbot builder, a broadcast tool, a CRM and a helpdesk are usually separate subscriptions that don't share context |

### 2.3 Why now
- **Customers prefer messaging apps.** WhatsApp and Instagram have become primary customer-service channels for e-commerce, especially in South Asia, the Middle East, the UK and Europe.
- **AI is now good enough and cheap enough to answer real customer questions** reliably when it is grounded in the business's own data and constrained by clear instructions.
- **Platform APIs are open to software providers.** Meta's WhatsApp Cloud API, the Instagram Messaging API and the Shopify Admin API now allow third parties to build compliant, official integrations.

---

## 3. Proposed Solution

### 3.1 The solution in one sentence
**One AI-powered workspace that connects every customer channel to the business's store and courier, answers routine questions automatically with AI agents and no-code workflows, and gives the team a clean inbox for everything else, with analytics and campaigns built in.**

### 3.2 How it works (end to end)

```
Customer messages on WhatsApp / Instagram / Messenger / Website chat
          │
          ▼
┌───────────────────────────────────────────────────────────────┐
│  Vetobase AI unified inbox (real-time, per-workspace)          │
│                                                               │
│  1. Intent AI      → reads the message, applies smart labels   │
│  2. Workflows      → no-code flows triggered by intent or      │
│                      store events (new order, abandoned cart)  │
│  3. AI agents      → answer using store/order/courier data and │
│                      the business's own instructions           │
│  4. Human handoff  → ticket + notification + full context      │
└───────────────────────────────────────────────────────────────┘
          │                         │
          ▼                         ▼
 Store & courier data       CRM · tickets · campaigns · analytics
 (Shopify orders, products,  (customers, orders, chats, team roles,
  checkouts; PostEx tracking) funnels, revenue attribution)
```

### 3.3 What makes the solution different

| Differentiator | Why it matters |
|---|---|
| **All channels + store + courier in one place** | The AI and the team answer from real order and tracking data, not guesses, without switching tools |
| **AI agents created in plain language** | A business owner types *"Create a refund agent that checks the order, applies our 30-day policy and reports to admin"*; no prompt engineering or code needed |
| **Visual automation builder with AI blocks** | Flows mix fixed steps (templates, buttons, order confirmation, tickets) with AI steps (AI condition, AI agent, confirmation agent) |
| **Built around messaging-platform rules** | It tracks WhatsApp's 24-hour window, reminds before it expires, and uses approved templates outside it |
| **Commerce-aware from day one** | Order confirmations, abandoned-cart recovery, delivery updates, order tagging (confirm/cancel), and per-customer order history inside the chat |
| **Campaigns with real attribution** | Every recipient's journey is tracked: sent, delivered, read, link clicked, order placed. Each campaign shows its conversion rate and the revenue it generated |
| **Human-first handoff** | The AI escalates complex or emotional cases (for example negative sentiment) with full context, so customers aren't stuck with a bot |
| **Designed for small teams** | One affordable workspace replaces several separate tools |

### 3.4 Current status of the solution
The core platform is **built and running in production** at app.vetobase.com:
- It is used by partner brands, including a fashion brand running **two live Shopify stores** connected to WhatsApp, with live order synchronisation.
- A **Shopify App Store version** (embedded app with secure token-based install, Shopify billing and a storefront chat widget) has been **built and tested** on a development store and is being prepared for submission.
- A complete **demo workspace** exists for presentations and reviewers.

Details are in Parts 2 and 3.

---

## 4. Target Users

### 4.1 Primary target segment
**Small and medium online businesses (roughly 1–50 support or sales staff) that sell to consumers and receive customer questions through messaging apps.**

| Segment | Typical profile | Main pain we solve |
|---|---|---|
| **D2C fashion and apparel brands** | Instagram-led brands with WhatsApp ordering, frequent size, price and availability questions, high return and exchange volume | Product questions, size/availability, order status, returns, abandoned carts |
| **Shopify merchants (any vertical)** | Stores on Shopify with growing order volume and a small support team | Store-aware AI answers, order confirmations, delivery updates, cart recovery |
| **Cash-on-delivery (COD) heavy markets** | Pakistan, the Middle East, South Asia; high fake or unconfirmed order rates | WhatsApp order confirmation before dispatch, courier tracking updates |
| **Service and booking businesses** | Salons, clinics, studios, tutors and agencies taking bookings on WhatsApp/Instagram | Booking support, FAQs, lead capture, reminders |
| **Growing brands running promotions** | Brands launching collections and sales via WhatsApp broadcasts | Campaigns with click, order and revenue tracking |

### 4.2 Geographic focus
- **Initial:** international English-speaking markets (United States, United Kingdom, Europe) through the Shopify App Store and direct sales, plus Pakistan, where our partner brands operate.
- **Next:** the Gulf region (UAE, Saudi Arabia) and wider South Asia, where WhatsApp commerce is dominant.

### 4.3 User roles inside a customer business

| Role | What they do in Vetobase AI |
|---|---|
| **Business owner / admin** | Connects channels and the store, creates AI agents and workflows, manages the team and permissions, reviews analytics and campaign revenue |
| **Support / sales agent** | Works the unified inbox, handles escalated chats and tickets, replies with full customer and order context |
| **Operations / fulfilment staff** | Tracks orders, confirmations, delivery status and production/stock boards |
| **Marketing** | Runs WhatsApp campaigns and measures opens, clicks, orders and revenue |
| **End customers (indirect users)** | Get instant, accurate answers on the channel they already use, 24/7 |

### 4.4 Example user story
> *A fashion brand gets 300+ messages a day across WhatsApp and Instagram during a sale. Before Vetobase AI, three staff answered "where is my order?" and "is this available in M?" by hand, while abandoned carts went unanswered.*
>
> *With Vetobase AI, every message lands in one inbox and is labelled automatically. Order-status questions are answered instantly from Shopify and courier data. Product questions get the price, availability and a buying link. New orders get a WhatsApp confirmation, and abandoned carts get a reminder. The team handles only the escalated cases, such as damaged parcels and custom requests, and arrives with the customer's full history in front of them.*

*(Continued in Part 2: Objectives & Expected Outcomes, Key Features / Deliverables.)*
