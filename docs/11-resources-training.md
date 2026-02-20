# Resources & Training Materials

## Introduction

This document consolidates all resources, training materials, and learning paths for Growisto's teams and merchant partners implementing Shopify AI features. Use this as a reference hub for onboarding, ongoing education, and troubleshooting.

## Official Shopify Resources

### Documentation & Guides

| **Resource** | **URL** | **Use Case** |
|-------------|---------|-------------|
| Shopify Help Center | help.shopify.com | General platform documentation |
| Shopify Plus Academy | academy.shopify.com | Structured learning for Plus merchants |
| Shopify Dev Docs | shopify.dev | API references, theme development |
| Shopify Changelog | changelog.shopify.com | New feature announcements |
| Shopify Engineering Blog | shopify.engineering | Technical deep dives |
| Shopify Partners Blog | shopify.com/partners/blog | Partner-focused updates |

### AI-Specific Documentation

| **Feature** | **Documentation** | **Key Topics** |
|------------|-------------------|---------------|
| Shopify Magic | Help Center > Shopify Magic | Content generation, image editing, SEO |
| Sidekick | Help Center > Sidekick | Admin assistant, analytics queries |
| Search & Discovery | Help Center > Search | Semantic search, filters, synonyms |
| Product Recommendations | Help Center > Recommendations | Algorithm types, widget placement |
| Shopify Audiences | Help Center > Audiences | Ad platform integration, audience types |
| Unified Customer Profile | Help Center > Customers | Identity resolution, segmentation |
| Shopify Flow | Help Center > Flow | Automation templates, custom workflows |
| B2B Features | Help Center > B2B | Wholesale, pricing, company management |

### Shopify Editions (Feature Launches)

Shopify releases major feature updates twice a year at "Editions" events:
- **Summer Edition** (typically June/July)
- **Winter Edition** (typically January/February)

Follow: editions.shopify.com for announcements

## Training Curriculum

### Track 1: Growisto Delivery Team Training

**Module 1: Shopify AI Fundamentals (4 hours)**
```
Topics:
1. Shopify's AI strategy and architecture (Doc 01)
2. Overview of all AI features and their business impact
3. How AI features interconnect (UCP → Personalization → Recommendations)
4. Competitive positioning vs Salesforce/Adobe/WooCommerce

Format: Self-paced reading + 1-hour team discussion
Assessment: Quiz on feature capabilities and positioning
```

**Module 2: Technical Implementation (8 hours)**
```
Topics:
1. UCP setup and configuration (Doc 03)
2. Shopify Magic configuration and brand voice (Doc 06)
3. Search & Discovery setup (Doc 04)
4. Recommendation engine configuration (Doc 05)
5. Shopify Flow automation (Doc 07)
6. Integration patterns (APIs, webhooks, middleware)

Format: Hands-on lab in Shopify Partner development store
Assessment: Set up all AI features in a test store
```

**Module 3: Analytics & Optimization (4 hours)**
```
Topics:
1. Setting up baseline metrics
2. Search analytics interpretation
3. Recommendation performance measurement
4. A/B testing methodologies
5. ROI calculation and reporting

Format: Case study analysis + dashboard setup exercise
Assessment: Create a performance report from sample data
```

**Module 4: India Market Specialization (4 hours)**
```
Topics:
1. India enterprise use cases (Doc 09)
2. Multilingual implementation best practices
3. Festival commerce strategies
4. Regional personalization patterns
5. Payment and logistics considerations
6. DPDP Act compliance for AI/data features

Format: Case studies from Indian merchants + role-play exercises
Assessment: Create an implementation plan for a sample Indian merchant
```

### Track 2: Merchant Team Training

**Session 1: AI for Business Leaders (1 hour)**
```
Audience: CEO, CMO, COO, CTO
Topics:
- Why AI matters for your business (with industry benchmarks)
- What Shopify AI can do (live demo)
- Expected ROI timeline
- What your team needs to do differently
- Key metrics to watch

Format: Presentation + live demo + Q&A
Deliverable: Executive summary one-pager
```

**Session 2: Content Team Workshop (2 hours)**
```
Audience: Content managers, copywriters, SEO specialists
Topics:
- Shopify Magic hands-on tutorial
- Product description generation workflow
- SEO metadata generation and optimization
- Multilingual content generation
- Image editing with AI
- Quality review process
- When to use AI vs write manually

Format: Hands-on workshop in merchant's Shopify Admin
Deliverable: Content production SOP with AI integration
```

**Session 3: Marketing Team Workshop (2 hours)**
```
Audience: Marketing managers, email marketers, ad managers
Topics:
- Shopify Audiences setup and campaign creation
- Email personalization with AI
- Customer segmentation for campaigns
- Recommendation-driven campaigns
- A/B testing with AI variations
- Measuring AI impact on marketing metrics

Format: Hands-on workshop + campaign planning exercise
Deliverable: Marketing playbook with AI-powered campaigns
```

**Session 4: Operations Team Workshop (2 hours)**
```
Audience: Store managers, operations team, customer service
Topics:
- Sidekick for daily operations
- Common Sidekick queries for your store
- Shopify Flow automations (monitoring, adjusting)
- Customer profile usage for service
- Inventory automation
- Troubleshooting common issues

Format: Hands-on workshop with real store scenarios
Deliverable: Operations handbook with Sidekick query library
```

## Sidekick Query Library

### Analytics Queries

```
"What were my top 10 best-selling products last month?"
"Show me revenue by channel for this quarter"
"What's my conversion rate trend for the last 90 days?"
"Which products have the highest return rate?"
"What are my top traffic sources this week?"
"Show me customer acquisition cost by channel"
"What's my average order value trend?"
"Which customer segments are growing fastest?"
"Show me sales by region for India"
"What products are trending up in the last 7 days?"
```

### Product Management Queries

```
"Set all summer collection products to 20% off"
"Which products are low in stock (less than 10 units)?"
"Add the tag 'festive' to all products in the Diwali collection"
"Show me products without descriptions"
"Which products haven't sold in the last 60 days?"
"Update the price of [product] to ₹2,999"
"Create a collection of products tagged 'new-arrival'"
"Which products have no images?"
"Show me products with less than 3 reviews"
"Unpublish all products with zero inventory"
```

### Customer Queries

```
"Show me customers who haven't ordered in 90 days"
"Who are my top 20 customers by lifetime value?"
"How many new customers did we acquire this month?"
"Show me customers from Mumbai with 3+ orders"
"What's the average order frequency for repeat customers?"
"Show customers who abandoned cart this week"
"Which customer segment has the highest AOV?"
"How many customers used UPI payment last month?"
"Show me VIP customers who haven't ordered recently"
"What percentage of customers are repeat buyers?"
```

### Operations Queries

```
"How many orders are pending fulfillment?"
"What's the average fulfillment time this week?"
"Show me orders flagged for fraud review"
"Which shipping zones have the most delays?"
"How many returns were processed this month?"
"What's our COD vs prepaid order ratio?"
"Show me orders above ₹10,000 from today"
"Which products were most returned this month?"
"How many discount codes were used this week?"
"Show me unfulfilled orders older than 48 hours"
```

## Shopify Flow Templates

### Essential Automations for Indian Enterprise

**Template 1: Low Stock Alert**
```yaml
Trigger: Inventory quantity changed
Condition: Inventory quantity < 10
Actions:
  - Send internal email to operations team
  - Add tag "low-stock" to product
  - Remove from "Best Sellers" collection (prevent overselling)
  - Send Slack notification to #inventory channel
```

**Template 2: VIP Customer Tagging**
```yaml
Trigger: Order created
Condition: Customer total orders >= 5 OR Customer total spent >= ₹25,000
Actions:
  - Add tag "vip" to customer
  - Add to "VIP Customers" segment
  - Send internal notification to CRM team
  - Trigger VIP welcome email sequence
```

**Template 3: High-Value Order Alert**
```yaml
Trigger: Order created
Condition: Order total >= ₹15,000
Actions:
  - Send internal notification to sales team
  - Add order tag "high-value"
  - Priority fulfillment queue
  - Send personalized thank you email
```

**Template 4: COD Risk Management**
```yaml
Trigger: Order created
Condition: Payment method = COD AND Order total > ₹5,000
Actions:
  - Send verification SMS to customer
  - Add tag "cod-verify" to order
  - Hold fulfillment for 2 hours (awaiting confirmation)
  - If no confirmation: Flag for manual review
```

**Template 5: Product Review Follow-Up**
```yaml
Trigger: Order fulfilled
Condition: 7 days after fulfillment
Actions:
  - Wait 7 days
  - Send review request email with product images
  - Include 10% off next purchase incentive
  - Add tag "review-requested" to order
```

**Template 6: Seasonal Collection Automation**
```yaml
Trigger: Scheduled (45 days before Diwali)
Actions:
  - Create "Diwali Collection" (if not exists)
  - Auto-populate with products tagged "festive" or "ethnic"
  - Feature on homepage
  - Trigger email campaign to all customers
  - Enable festival-specific discount codes
```

**Template 7: Win-Back Campaign Trigger**
```yaml
Trigger: Customer created (scheduled check every 7 days)
Condition: Last order > 90 days ago AND Customer total orders >= 2
Actions:
  - Add to "Win-Back" segment
  - Trigger win-back email sequence
  - Generate personalized discount code (15% off)
  - Add tag "win-back-eligible"
```

## Recommended Third-Party Tools

### Analytics & Reporting

| **Tool** | **Purpose** | **Integration** | **Pricing** |
|---------|-----------|----------------|------------|
| Google Analytics 4 | Web analytics | Native Shopify integration | Free |
| Lifetimely | Customer LTV analytics | Shopify app | From $34/month |
| Triple Whale | Attribution & analytics | Shopify app | From $100/month |
| Polar Analytics | D2C analytics dashboard | Shopify app | From $300/month |

### Email & Marketing

| **Tool** | **Purpose** | **Integration** | **Pricing** |
|---------|-----------|----------------|------------|
| Klaviyo | Email/SMS marketing | Deep Shopify integration | Free up to 250 contacts |
| Omnisend | Email/SMS/push | Shopify app | Free up to 250 contacts |
| WebEngage | Customer engagement (India-focused) | API integration | Custom pricing |
| MoEngage | Customer engagement (India-focused) | API integration | Custom pricing |

### Customer Support

| **Tool** | **Purpose** | **Integration** | **Pricing** |
|---------|-----------|----------------|------------|
| Gorgias | E-commerce helpdesk | Deep Shopify integration | From $10/month |
| Freshdesk | Support ticketing | Shopify app | Free tier available |
| Intercom | Live chat + AI bot | Shopify integration | From $39/month |
| Yellow.ai | AI chatbot (India-focused) | API integration | Custom pricing |

### Reviews & Social Proof

| **Tool** | **Purpose** | **Integration** | **Pricing** |
|---------|-----------|----------------|------------|
| Judge.me | Product reviews | Shopify app | Free tier available |
| Loox | Photo reviews | Shopify app | From $9.99/month |
| Stamped.io | Reviews + loyalty | Shopify app | Free tier available |

### India-Specific Tools

| **Tool** | **Purpose** | **Integration** | **Pricing** |
|---------|-----------|----------------|------------|
| Razorpay | Payment gateway | Shopify integration | Per-transaction |
| Shiprocket | Shipping aggregator | Shopify app | From ₹20/shipment |
| Unicommerce | Order/inventory management | API integration | Custom pricing |
| WhatsApp Business API | Customer communication | Via partners (Gupshup, Wati) | Per-message |
| Clevertap | Customer analytics | API integration | Custom pricing |

## Compliance & Legal Resources

### DPDP Act (Digital Personal Data Protection Act, 2023)

```
Key requirements for AI features:

1. Consent Management
   - Explicit consent for data collection
   - Clear purpose specification
   - Easy withdrawal mechanism
   
2. Data Localization
   - Certain data categories must stay in India
   - Shopify's India data residency options
   
3. Customer Rights
   - Right to access personal data
   - Right to correction
   - Right to erasure
   
4. AI Transparency
   - Disclose when AI is used for personalization
   - Allow opt-out of AI-driven recommendations
   - Explain automated decision-making when asked

Implementation:
- Privacy policy template (AI-specific clauses)
- Consent banner configuration
- Data access request workflow
- AI disclosure in terms of service
```

### E-commerce Regulations (India)

```
Key considerations:
- Consumer Protection (E-Commerce) Rules, 2020
- Legal Metrology (Packaged Commodities) Rules
- GST compliance for digital goods
- FDI regulations for marketplace vs inventory model
- MRP display requirements

Resources:
- Ministry of Consumer Affairs guidelines
- DPIIT e-commerce policy updates
- Industry associations (NASSCOM, CII, FICCI)
```

## Certification & Learning Paths

### Shopify Partner Academy

```
Recommended certifications:
1. Shopify Foundations Certification (prerequisite)
2. Shopify App Development Certification
3. Shopify Theme Development Certification
4. Shopify Plus Partner Certification (if available)

Time investment: 4-8 hours per certification
Value: Credibility with merchants, access to partner resources
```

### AI/ML Fundamentals (Optional but Recommended)

```
For team members wanting deeper AI understanding:

1. Google AI Essentials (Coursera) - 10 hours
   - AI fundamentals for business professionals
   
2. AI for Everyone (Andrew Ng, Coursera) - 6 hours
   - Non-technical AI strategy course
   
3. Commerce AI Applications (various platforms) - 8 hours
   - Recommendation systems basics
   - Personalization strategies
   - Search relevance optimization
```

## Community & Support

### Shopify Community Resources

| **Resource** | **URL** | **Best For** |
|-------------|---------|-------------|
| Shopify Community Forums | community.shopify.com | Peer support, best practices |
| Shopify Partners Slack | Via partner dashboard | Real-time partner discussions |
| Shopify Plus Facebook Group | Facebook Groups | Plus merchant networking |
| r/shopify (Reddit) | reddit.com/r/shopify | Community troubleshooting |
| Shopify Dev Discord | Via shopify.dev | Developer-focused discussions |

### India-Specific Communities

| **Resource** | **Platform** | **Focus** |
|-------------|------------|----------|
| D2C India | LinkedIn Group | Indian D2C ecosystem |
| Shopify India Partners | WhatsApp Group | India partner network |
| Indian E-commerce Leaders | LinkedIn Group | Enterprise e-commerce |
| YourStory D2C | Media | Indian D2C news and analysis |
| Inc42 E-commerce | Media | Indian startup/e-commerce coverage |

### Growisto Internal Resources

```
Knowledge base: [Internal wiki/Notion link]
Slack channels:
  #shopify-ai — AI feature discussions
  #client-implementations — Active project updates
  #tech-support — Technical troubleshooting
  #india-ecommerce — Market trends and insights

Weekly sync: Friday AI feature review (30 min)
Monthly: Client implementation retrospective
Quarterly: AI roadmap review with Shopify partner team
```

## Quick Reference Cards

### Shopify Magic Quick Reference

```
┌─────────────────────────────────────────────────┐
│            SHOPIFY MAGIC QUICK REF              │
├─────────────────────────────────────────────────┤
│                                                 │
│  PRODUCT DESCRIPTIONS                           │
│  Admin > Products > [Product] > Description     │
│  Click ✨ Magic icon > Select tone > Generate   │
│                                                 │
│  SEO METADATA                                   │
│  Admin > Products > [Product] > SEO             │
│  Click ✨ Magic icon > Generate title + desc    │
│                                                 │
│  EMAIL CONTENT                                  │
│  Admin > Marketing > Campaigns > Create         │
│  Click ✨ Magic icon > Generate subject + body  │
│                                                 │
│  IMAGE EDITING                                  │
│  Admin > Products > [Product] > Images          │
│  Click image > Edit > Remove background         │
│                                                 │
│  BLOG POSTS                                     │
│  Admin > Blog Posts > Create                    │
│  Click ✨ Magic icon > Generate from topic      │
│                                                 │
│  TIPS:                                          │
│  • Set brand voice FIRST (Settings > Magic)     │
│  • Review all AI content before publishing      │
│  • Use "Regenerate" for alternative versions    │
│  • Edit AI output to add brand-specific details │
│                                                 │
└─────────────────────────────────────────────────┘
```

### Sidekick Quick Reference

```
┌─────────────────────────────────────────────────┐
│            SIDEKICK QUICK REFERENCE             │
├─────────────────────────────────────────────────┤
│                                                 │
│  ACCESS: Click Sidekick icon in Admin header    │
│                                                 │
│  ANALYTICS:                                     │
│  "What were my sales today?"                    │
│  "Top products this week"                       │
│  "Compare this month to last month"             │
│                                                 │
│  PRODUCTS:                                      │
│  "Set [product] to ₹X"                          │
│  "Which products are out of stock?"             │
│  "Add tag 'sale' to summer collection"          │
│                                                 │
│  CUSTOMERS:                                     │
│  "How many new customers this month?"           │
│  "Show VIP customers"                           │
│  "Customers who haven't ordered in 90 days"     │
│                                                 │
│  ORDERS:                                        │
│  "Pending orders today"                         │
│  "Average order value this week"                │
│  "Orders from Mumbai"                           │
│                                                 │
│  TIPS:                                          │
│  • Be specific with time periods                │
│  • Use natural language (no special syntax)     │
│  • Ask follow-up questions for deeper insights  │
│  • Sidekick remembers context within session    │
│                                                 │
└─────────────────────────────────────────────────┘
```

## Key Takeaways

1. **Invest in training**—AI tools are only as effective as the people using them. Budget 2 days for merchant team training.

2. **Use official resources first**—Shopify's documentation is comprehensive and updated. Start there before third-party guides.

3. **India-specific tooling matters**—payment, shipping, and communication tools built for India are essential complements to Shopify AI.

4. **Compliance is non-negotiable**—DPDP Act compliance must be baked into every AI implementation from day one.

5. **Community accelerates learning**—join Shopify and India D2C communities for real-world insights and troubleshooting.

6. **Keep this document updated**—AI features evolve rapidly. Review and update resources quarterly.

---

**Document Version**: 1.0
**Last Updated**: February 2026
**Prepared for**: Growisto Partner Enablement
