# Appendix: Glossary, API References, Links & Troubleshooting

## Glossary of AI & Shopify Terms

### A

| **Term** | **Definition** |
|---------|---------------|
| **A/B Testing** | Comparing two versions of a page, email, or feature to determine which performs better. Shopify supports AI-automated A/B testing for themes and content. |
| **Admin API** | Shopify's primary API for managing store data (products, orders, customers). Available in REST and GraphQL. |
| **AOV (Average Order Value)** | Total revenue divided by number of orders. AI recommendations aim to increase AOV through cross-sell and upsell. |
| **API (Application Programming Interface)** | A set of protocols allowing software applications to communicate. Shopify provides multiple APIs for store management and customization. |
| **Audiences (Shopify Audiences)** | AI-powered feature that generates high-intent customer lists for advertising platforms (Meta, Google, TikTok, etc.) using Shopify's aggregated, anonymized commerce data. Plus-exclusive. |

### B

| **Term** | **Definition** |
|---------|---------------|
| **B2B (Business-to-Business)** | Commerce between businesses. Shopify Plus supports B2B with company profiles, custom pricing, and AI-powered catalog management. |
| **Boosting (Search)** | Manually or algorithmically prioritizing certain products in search results. AI search uses signals like conversion rate, margin, and inventory levels. |
| **Brand Voice** | The configured personality and tone settings for Shopify Magic's content generation. Set in Admin → Settings → Shopify AI. |

### C

| **Term** | **Definition** |
|---------|---------------|
| **CAC (Customer Acquisition Cost)** | Total marketing spend divided by number of new customers acquired. Shopify Audiences aims to reduce CAC. |
| **Churn Risk** | AI-predicted probability that a customer will stop purchasing. Part of the Unified Customer Profile's predictive analytics. |
| **COD (Cash on Delivery)** | Payment method where customers pay upon delivery. Dominant in India; AI can analyze COD vs prepaid behavior patterns. |
| **Collections (Smart)** | Shopify collections that automatically include products based on AI-defined conditions and categorization. |
| **Conversational Commerce** | Using chat interfaces (WhatsApp, Inbox, Sidekick) to facilitate purchases. AI enables automated, personalized conversations. |

### D

| **Term** | **Definition** |
|---------|---------------|
| **D2C (Direct-to-Consumer)** | Brands selling directly to end consumers without intermediaries. India's D2C ecosystem is a primary focus for Growisto. |
| **DPDP Act** | Digital Personal Data Protection Act 2023 (India). Governs collection, storage, and processing of personal data. Relevant to AI features using customer data. |

### E-F

| **Term** | **Definition** |
|---------|---------------|
| **Embeddings** | Vector representations of text/images used by AI to understand semantic meaning. Powers Shopify's semantic search. |
| **Flow (Shopify Flow)** | Visual automation platform for creating workflows without code. AI-enhanced triggers and conditions enable intelligent automation. Plus-exclusive. |
| **FSSAI** | Food Safety and Standards Authority of India. Compliance requirement for food/beverage merchants. |

### G-H

| **Term** | **Definition** |
|---------|---------------|
| **GraphQL** | Query language for APIs. Shopify's preferred API format, offering more efficient data retrieval than REST. |
| **Headless Commerce** | Architecture separating the frontend (storefront) from the backend (Shopify). Shopify supports this via Hydrogen/Oxygen and the Storefront API. |
| **Hydrogen** | Shopify's React-based framework for building custom storefronts. Works with Oxygen hosting. |

### I-L

| **Term** | **Definition** |
|---------|---------------|
| **Inbox (Shopify Inbox)** | Customer messaging tool with AI-powered instant answers, product recommendations, and conversation management. |
| **LLM (Large Language Model)** | AI model trained on vast text data to understand and generate human language. Powers Sidekick, Magic, and other Shopify AI features. |
| **Liquid** | Shopify's template language for customizing storefronts. Used in themes to render dynamic content. |
| **LTV (Lifetime Value)** | Predicted total revenue a customer will generate. Shopify's AI calculates predictive LTV in the Unified Customer Profile. |
| **Lookalike Audience** | An advertising audience modeled after existing high-value customers. Shopify Audiences generates these using commerce signals. |

### M-O

| **Term** | **Definition** |
|---------|---------------|
| **Magic (Shopify Magic)** | Brand name for Shopify's suite of AI-powered content generation tools — product descriptions, email content, image editing, blog posts, and more. |
| **Metafields** | Custom data fields attached to Shopify resources (products, customers, orders). AI features can read/write metafields for enriched personalization. |
| **NLP (Natural Language Processing)** | AI technology for understanding human language. Powers Sidekick's conversational interface and semantic search. |
| **ONDC** | Open Network for Digital Commerce. India's government-backed open e-commerce protocol. |

### P-R

| **Term** | **Definition** |
|---------|---------------|
| **Plus (Shopify Plus)** | Enterprise tier of Shopify with advanced features including AI capabilities, Shopify Flow, Audiences, B2B, and dedicated support. |
| **Predictive Analytics** | Using AI/ML to forecast future outcomes (customer churn, demand, LTV) based on historical data. |
| **Product Recommendations** | AI-generated product suggestions based on browsing behavior, purchase history, and collaborative filtering. |
| **ROAS (Return on Ad Spend)** | Revenue generated per rupee spent on advertising. AI-powered Audiences aims to improve ROAS. |

### S

| **Term** | **Definition** |
|---------|---------------|
| **Semantic Search** | AI-powered search that understands the meaning and intent behind queries, not just keyword matching. "Blue party dress" returns relevant results even without exact keyword matches. |
| **Sidekick** | Shopify's conversational AI assistant in the admin. Helps merchants with analytics, store management, and decision-making via natural language. |
| **Shopify Functions** | Server-side logic for customizing Shopify's backend (discounts, shipping, payments). Runs in a WebAssembly sandbox. |
| **Storefront API** | Public API for building custom shopping experiences. Powers headless commerce and mobile apps. |

### T-U

| **Term** | **Definition** |
|---------|---------------|
| **Theme** | The frontend template that controls how a Shopify store looks. AI features integrate with themes via sections and Liquid. |
| **Unified Customer Profile** | AI-enhanced 360° view of each customer, aggregating data from all channels. Includes predictive LTV, churn risk, and behavioral insights. Plus feature. |
| **UPI (Unified Payments Interface)** | India's real-time payment system. Major payment method for Indian e-commerce; transaction data feeds into AI analytics. |

### V-Z

| **Term** | **Definition** |
|---------|---------------|
| **Visual Search** | AI feature allowing customers to search by uploading an image. The system identifies similar products in the catalog. |
| **Webhook** | Automated notification sent from Shopify to an external URL when specific events occur. Used to trigger external AI workflows. |
| **Zero-Result Rate** | Percentage of searches that return no results. AI search aims to minimize this through semantic understanding and suggestions. |

---

## API Quick Reference

### Key Shopify APIs for AI Features

| **API** | **Endpoint Base** | **Auth** | **Primary Use** |
|---------|-------------------|----------|-----------------|
| Admin REST API | `https://{store}.myshopify.com/admin/api/2025-01/` | Access token | Store management |
| Admin GraphQL API | `https://{store}.myshopify.com/admin/api/2025-01/graphql.json` | Access token | Efficient queries |
| Storefront API | `https://{store}.myshopify.com/api/2025-01/graphql.json` | Storefront token | Customer-facing |
| Shopify Flow API | Via Admin API | Access token | Automation triggers |
| Customer Account API | `https://shopify.com/{store}/account/` | Customer token | Account management |

### Useful GraphQL Queries

#### Fetch Products with AI-Generated Content
```graphql
query {
  products(first: 10) {
    edges {
      node {
        id
        title
        descriptionHtml
        seo {
          title
          description
        }
        metafields(first: 5, namespace: "shopify-ai") {
          edges {
            node {
              key
              value
            }
          }
        }
      }
    }
  }
}
```

#### Fetch Customer with Predictive Data
```graphql
query {
  customer(id: "gid://shopify/Customer/123456") {
    firstName
    lastName
    email
    predictedSpendTier
    numberOfOrders
    amountSpent {
      amount
      currencyCode
    }
    tags
    metafields(first: 10) {
      edges {
        node {
          namespace
          key
          value
        }
      }
    }
  }
}
```

#### Search Products (Storefront API)
```graphql
query {
  search(query: "blue kurta", types: PRODUCT, first: 10) {
    edges {
      node {
        ... on Product {
          id
          title
          description
          priceRange {
            minVariantPrice {
              amount
              currencyCode
            }
          }
          images(first: 1) {
            edges {
              node {
                url
              }
            }
          }
        }
      }
    }
  }
}
```

### Webhook Events for AI Workflows

| **Event** | **Trigger** | **AI Use Case** |
|----------|------------|-----------------|
| `orders/create` | New order placed | Trigger post-purchase AI recommendations |
| `customers/create` | New customer registered | Initialize Unified Customer Profile |
| `products/update` | Product modified | Re-trigger AI content generation |
| `carts/update` | Cart modified | Trigger AI cart abandonment prediction |
| `inventory_levels/update` | Stock changed | Trigger AI restock forecasting |
| `customer_tags/update` | Customer tags changed | Update AI segments |

### API Rate Limits

| **Plan** | **REST** | **GraphQL** |
|----------|---------|-------------|
| Shopify Plus | 20 requests/second | 2,000 cost points/second |
| Standard | 2 requests/second | 1,000 cost points/second |

> **Note**: AI-heavy integrations (bulk content generation, customer sync) should use GraphQL bulk operations to stay within rate limits.

---

## Useful Links by Category

### Shopify Platform
| **Link** | **URL** |
|---------|---------|
| Shopify Admin | https://admin.shopify.com |
| Shopify Help Center | https://help.shopify.com |
| Shopify Status | https://www.shopifystatus.com |
| Shopify Changelog | https://changelog.shopify.com |
| Shopify App Store | https://apps.shopify.com |
| Shopify Theme Store | https://themes.shopify.com |

### Development
| **Link** | **URL** |
|---------|---------|
| Shopify Dev Docs | https://shopify.dev |
| API Versioning | https://shopify.dev/docs/api/usage/versioning |
| Shopify CLI | https://shopify.dev/docs/apps/tools/cli |
| Polaris Design System | https://polaris.shopify.com |
| Shopify GitHub | https://github.com/Shopify |

### Community & Support
| **Link** | **URL** |
|---------|---------|
| Shopify Community Forums | https://community.shopify.com |
| Shopify Partners Slack | Via Partner Dashboard |
| Stack Overflow (Shopify) | https://stackoverflow.com/questions/tagged/shopify |
| Shopify Plus Support | https://help.shopify.com/en/support/plus |

---

## Troubleshooting Guide

### Sidekick Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Sidekick not appearing in admin | Feature not enabled for staff account | Admin → Settings → Users → Edit staff permissions |
| Sidekick gives incorrect analytics | Date range mismatch or data sync delay | Verify date range; wait 24h for data sync |
| Sidekick responses in wrong language | Language settings misconfigured | Admin → Settings → Languages → Set primary language |
| "I can't help with that" responses | Query outside Sidekick's capabilities | Rephrase the question; check supported features in docs |
| Slow Sidekick responses | High platform load or complex query | Retry; break complex queries into smaller ones |

### Shopify Magic Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Generated descriptions are generic | Brand voice not configured | Set up brand voice: Admin → Settings → Shopify AI |
| Content in wrong language | Language preference mismatch | Set target language before generating |
| Generated content doesn't save | Browser/session timeout | Refresh admin; copy content before navigating away |
| Image background removal artifacts | Complex product image (hair, transparency) | Use a simpler background; try re-uploading at higher resolution |
| Bulk generation fails mid-batch | Rate limiting or timeout | Process in smaller batches (50 products at a time) |

### Search & Discovery Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Semantic search not returning relevant results | Insufficient product data | Enrich product titles, descriptions, and tags |
| Search results not including new products | Search index not updated | Wait 15-30 min for indexing; force reindex via app |
| Recommendations showing out-of-stock items | Inventory filter not enabled | Search & Discovery app → Settings → Exclude out-of-stock |
| Zero results for Hindi queries | Hindi not supported in search config | Add Hindi synonyms manually; verify multilingual settings |

### Shopify Flow Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Flow not triggering | Trigger conditions too narrow | Review and widen trigger conditions |
| Flow actions failing | API permissions insufficient | Check app permissions for the action's integration |
| Duplicate flow executions | Multiple overlapping triggers | Add conditions to prevent re-entry |
| Flow runs but no visible result | Action target misconfigured | Verify email addresses, tags, or webhook URLs |

### Shopify Audiences Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Audiences not generating | Insufficient order volume | Requires meaningful order history; check minimum thresholds |
| Audiences not syncing to Meta/Google | Ad account not connected | Reconnect ad platform in Settings → Apps → Audiences |
| Small audience size | Narrow store data | Expand product catalog and marketing reach first |
| Attribution data missing | Pixel/CAPI not configured | Verify Meta Pixel and Conversions API setup |

### India-Specific Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| UPI payment data not in analytics | Payment gateway integration gap | Verify Razorpay/PayU Shopify app is latest version |
| COD orders skewing AI predictions | COD returns not tracked properly | Ensure return/cancellation data flows back to Shopify |
| Regional language content quality poor | Limited training data for Indic languages | Use AI as first draft; have native speakers review and edit |
| Slow admin load times | Geographic latency to Shopify servers | Use CDN; consider Shopify's infrastructure region settings |
| GST calculations conflicting with AI pricing | Tax rules not configured correctly | Verify GST settings in Admin → Settings → Taxes |

### General Performance Issues

| **Problem** | **Possible Cause** | **Solution** |
|------------|-------------------|-------------|
| Store slow after enabling AI features | Heavy theme + multiple AI widgets | Audit theme performance; lazy-load recommendation widgets |
| API rate limit exceeded | Too many concurrent AI-driven API calls | Implement request queuing; use bulk operations |
| Data discrepancies between Shopify and GA4 | Tracking code issues or attribution differences | Audit tracking setup; accept some variance as normal |

---

## Version History

| **Version** | **Date** | **Changes** |
|------------|---------|-------------|
| 1.0 | February 2026 | Initial release — complete enablement package |

---

## Contact & Support

| **Need** | **Contact** |
|---------|------------|
| Growisto implementation support | Implementation team lead |
| Shopify Plus support | https://help.shopify.com/en/support/plus |
| Shopify Partner support | Via Partner Dashboard |
| Emergency (store down) | Shopify Plus 24/7 priority support line |

---

*← [Resources & Training](11-resources-training.md) | [Back to README](../README.md)*
