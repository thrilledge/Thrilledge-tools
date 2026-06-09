# Thrilledge-tools

# AI Freelance Toolkit

A collection of AI-powered tools to help freelancers win more clients — from proposals to cold outreach. Built with a generous free tier and a simple upgrade path.

## 🛠️ Tools

| Tool | Description | Free Limit |
|------|-------------|-------------|
| **AI Upwork Proposal Writer** | Takes job description + your skills/experience → generates persuasive proposal | 5/month |
| **Cold Email Generator** | Takes prospect info + your service → generates personalized cold email | 10/month |
| **Cold Calling Script Generator** | Takes prospect persona + offering → generates script with hooks | 5/month |
| **Freelance Rate Calculator** (bonus) | Calculates hourly/project rates based on expenses & profit margin | Unlimited |

## 💰 Subscription Model

| Tier | Price | Limits |
|------|-------|--------|
| **Free** | $0 | 5 proposals + 10 emails + 5 scripts / month |
| **Unlimited** | $9.99/mo or $99/yr | All tools unlimited |

## ⚙️ Implementation Details

### Auth-less Approach (IP-based + optional email)

- **Free tier tracking**: IP + localStorage + optional Upstash Redis fallback
- **Upgrade flow**: Simple payment link (Stripe / LemonSqueezy) → set cookie or Redis flag
- No complex auth system needed initially

### AI Generation (GROQ)

Each tool uses a tailored system prompt specific to its purpose:

> *Example — Proposal Writer prompt:*  
> *"You are an expert Upwork proposal writer. Hook the client in the first line..."*

### State Management

- **Zustand** store for current tab, form inputs, and generated results
- **LocalStorage** for free usage tracking (with Redis as fallback)

---

## 🚀 Getting Started

*(Add setup instructions here once available)*

## 📄 License

*(Add license info here)*
