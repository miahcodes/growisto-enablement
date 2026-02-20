# Sidekick: Shopify's AI Commerce Assistant

## What is Sidekick?

Sidekick is Shopify's conversational AI assistant embedded directly in the Shopify Admin. Think of it as having a Shopify expert who knows your store's data, understands commerce best practices, and can execute complex tasks through natural language.

**Key Distinction**: Sidekick isn't a chatbot—it's an **AI commerce operator** with read/write access to your store.

### Core Capabilities

```
Merchant: "Show me my top 10 products by revenue this month compared to last month"
Sidekick: [Generates comparison table with revenue, units sold, traffic, and conversion rate]

Merchant: "Create a discount code for 25% off for VIP customers, valid during Diwali week"
Sidekick: [Creates discount code, applies customer segment, sets date range, confirms]

Merchant: "Why did our conversion rate drop last week?"
Sidekick: [Analyzes traffic sources, product availability, checkout abandonment, and identifies root cause]
```

## Core Capabilities Deep Dive

### 1. Store Setup & Configuration

#### What Sidekick Can Do:
- **Product setup**: Create products with variants, pricing, inventory across locations
- **Collection creation**: Build smart collections based on tags, price, inventory, vendor
- **Theme customization**: Modify theme settings, add sections, update copy
- **App recommendations**: Suggest apps based on merchant goals
- **Shipping setup**: Configure zones, rates, and shipping rules

#### Enterprise Use Case:
**Scenario**: Launch 500 SKUs for new product category before Diwali

**Traditional Approach**: 
- 2-3 days for product data entry and QA
- Manual collection setup
- Trial-and-error on theme updates

**With Sidekick**:
```
Merchant: "Import products from this CSV, create collections by brand and price range 
(under ₹999, ₹1000-2499, ₹2500+), and add a 'Diwali Gifts' banner to the homepage hero section"

Sidekick: 
✓ Imported 500 products
✓ Created 15 collections with smart rules
✓ Updated theme with seasonal banner
✓ Suggested: "Would you like me to create a Diwali discount campaign?"

Time saved: ~20 hours → 10 minutes
```

### 2. Analytics & Reporting Queries

#### Natural Language Analytics:
Sidekick understands commerce-specific questions without requiring SQL or custom reports.

**Examples**:

| **Question** | **What Sidekick Analyzes** |
|--------------|---------------------------|
| "Which products are underperforming?" | Sessions vs conversion rate vs benchmark |
| "Show me customer cohorts by acquisition channel" | Lifetime value and retention by UTM source |
| "What's driving our repeat purchase rate?" | Product affinity, email engagement, discount sensitivity |
| "Compare festive season 2025 vs 2024" | Revenue, orders, AOV, new vs returning customer split |

#### Advanced Analytics Capabilities:

**Attribution Analysis**:
```
Merchant: "Break down revenue attribution for our Diwali campaign across Meta, Google, 
and influencer referrals"

Sidekick: 
- First-touch attribution: Meta (45%), Google (30%), Influencer (25%)
- Last-touch attribution: Google (52%), Meta (35%), Influencer (13%)
- Multi-touch model (recommended): Meta (42%), Google (38%), Influencer (20%)
- Insight: Influencers drive discovery, Google captures intent, Meta drives consideration
```

**Predictive Insights**:
```
Merchant: "Will we hit our ₹2 crore target for Q4?"

Sidekick:
- Current trajectory: ₹1.65 crore (82.5% of target)
- Factors: 12% growth rate, 2 major campaigns remaining
- Probability of hitting target: 68%
- Recommendation: Increase ad spend by ₹3 lakh in weeks 11-12 to reach 85% probability
```

### 3. Marketing Suggestions & Automation

#### Campaign Ideation:
Sidekick analyzes inventory, customer segments, and market trends to suggest campaigns.

**Example**:
```
Merchant: "I have excess inventory of winter wear. What should I do?"

Sidekick:
- Detected: 450 units of winter jackets, 280 units of sweaters (45 days of inventory at current sell-through)
- Segment identified: 2,340 customers in cold-weather cities (Delhi, Shimla, Srinagar) who haven't purchased in 60 days
- Campaign suggestion:
  • Email: "Winter Wardrobe Refresh - 30% Off"
  • Target: Lapsed customers in cold regions
  • Timing: Send Wednesday 10 AM (optimal open rate)
  • Projected impact: ₹8.5 lakh revenue, 180-220 units sold
- Create campaign now? [Yes] [Modify] [No]
```

#### Discount Strategy Optimization:
```
Merchant: "What discount should I offer for new customer acquisition?"

Sidekick:
- Analysis of 8,450 first-time orders:
  • 35% converted with no discount (email capture only)
  • 42% converted with 10-15% discount
  • 18% converted with 20-25% discount
  • 5% converted with 30%+ discount
- Recommendation: Tiered approach
  • Default: 10% welcome discount (email signup)
  • Cart abandonment: 15% after 24 hours
  • Browse abandonment: 20% after 3 visits, no purchase
- Avoid blanket 30% discounts - they reduce LTV by 28% vs 10% discount cohorts
```

### 4. Inventory Insights & Forecasting

#### Stock Health Analysis:
```
Merchant: "Show me inventory issues"

Sidekick:
⚠️ Stockout Risks (7-14 days):
- ProductA (Navy, L): 12 units remaining, selling 3/day
- ProductB (Gold variant): 28 units, Diwali surge expected

⚠️ Overstock Issues (>90 days inventory):
- ProductC (Pink): 340 units, 0.5 units/day sell-through
- Recommendation: Bundle with best-sellers or 25% clearance

✓ Optimal Stock (30-60 days):
- 78% of SKUs in healthy range

Action Items:
1. Reorder ProductA and ProductB immediately
2. Create "Mystery Bundle" with ProductC + top sellers
3. Adjust forecasting model for ProductC's color preference
```

#### Predictive Restocking:
```
Merchant: "When should I reorder ProductX?"

Sidekick:
- Current stock: 145 units
- Sell-through rate: 8.5 units/day (trending +15% from last week)
- Lead time from supplier: 12 days
- Safety stock recommendation: 30 units (3.5 days)
- Reorder trigger: When inventory hits 132 units (~15 days from now)
- Order quantity: 250 units (based on next 30-day forecast)
- Set automated reorder alert? [Yes] [No]
```

### 5. Multi-Store Management (Enterprise Feature)

For holding companies or multi-brand merchants managing 3-10+ Shopify Plus stores:

```
Merchant: "Compare performance across all my stores this month"

Sidekick:
[Aggregated Dashboard]
Store A (Fashion): ₹42L revenue (+18% MoM) - 🟢 On track
Store B (Home Decor): ₹28L revenue (-8% MoM) - 🟡 Needs attention
Store C (Beauty): ₹35L revenue (+22% MoM) - 🟢 Exceeding targets
Store D (Kids): ₹19L revenue (+5% MoM) - 🟡 Slower than expected

Insight: Beauty outperforming due to influencer campaign. 
Recommendation: Replicate influencer strategy for Home Decor to reverse trend.
```

**Cross-Store Insights**:
```
Merchant: "Which customers shop across multiple brands?"

Sidekick:
- 1,240 customers purchased from 2+ stores (cross-brand shoppers)
- Average LTV: ₹18,500 (vs ₹6,200 single-store)
- Top combo: Fashion + Beauty (680 customers)
- Opportunity: Create unified loyalty program, cross-brand bundles
- Projected revenue impact: ₹15-22 lakh additional annual revenue
```

## How Merchants Interact with Sidekick

### Access Points

1. **Shopify Admin Sidebar**: Persistent chat interface
2. **Contextual Triggers**: Sidekick proactively offers help based on merchant behavior
3. **Mobile Admin App**: Full functionality on iOS/Android
4. **Voice Commands** (2025+): "Hey Sidekick, show me today's sales"

### Conversation Patterns

#### Simple Commands:
- "Show sales dashboard"
- "Create a discount code"
- "Export customer list"

#### Complex Queries:
- "Identify customers who viewed ProductA 3+ times but didn't purchase, segment by city, and draft an email campaign"
- "Compare CAC across all channels for the past 6 months, adjusted for LTV, and recommend budget reallocation"

#### Multi-Turn Conversations:
```
Merchant: "I want to launch a loyalty program"
Sidekick: "Great! Let's set this up. What's your goal - increase repeat purchases or average order value?"

Merchant: "Repeat purchases"
Sidekick: "Perfect. Based on your data:
- Current repeat purchase rate: 23%
- Industry benchmark: 30%
- Top opportunity: Customers who purchased 1x in last 90 days (1,850 people)

Would you like a points-based or tiered program?"

Merchant: "Points-based"
Sidekick: "Recommended structure:
- Earn 5 points per ₹100 spent
- 500 points = ₹500 discount
- Birthday bonus: 250 points

This matches your 18% margin profile. Install loyalty app now?"
```

## Enterprise Use Cases

### Use Case 1: Multi-Market Expansion
**Client Profile**: Fashion brand expanding from India to Middle East

**Challenge**: Different product catalogs, currencies, languages, customer preferences

**Sidekick Workflow**:
```
Merchant: "Help me set up our UAE store based on our India store"

Sidekick:
✓ Duplicated store structure
✓ Converted pricing to AED (₹→AED at 0.045 rate)
✓ Updated shipping zones for GCC countries
✓ Recommended: Remove cash-on-delivery (low adoption in UAE), add Tabby (buy-now-pay-later)
✓ Content localization: Translated product descriptions to Arabic
✓ Adjusted size charts for regional preferences
✓ Recommended removing 15 products with low GCC cultural fit

Time saved: 3 weeks → 4 hours
```

### Use Case 2: Team Productivity & Training
**Client Profile**: ₹50 crore GMV merchant with 8-person operations team

**Challenge**: High turnover, inconsistent decision-making, training bottlenecks

**Sidekick as Team Multiplier**:
- **New hire onboarding**: Sidekick answers questions, guides workflows, reduces training from 2 weeks to 3 days
- **Consistent execution**: Junior team members can execute senior-level analysis
- **Reduced escalations**: 60% of "ask manager" questions answered by Sidekick

**Example**:
```
Junior Team Member: "A customer wants a refund but it's been 40 days. What's our policy?"

Sidekick:
- Store policy: 30-day returns
- This order: 42 days old
- Customer LTV: ₹24,000 (top 5% customer)
- Recommendation: Approve as one-time exception, note in customer profile
- Action: Issue refund and send personalized apology with 10% next purchase code?
```

### Use Case 3: Complex Pricing Strategies
**Client Profile**: Electronics merchant with dynamic pricing needs

**Challenge**: Manage competitive pricing across 2,000 SKUs

**Sidekick Workflow**:
```
Merchant: "Monitor competitor pricing and alert me when we're >5% higher on top 100 SKUs"

Sidekick:
✓ Set up daily competitor price monitoring
✓ Created alert system
✓ Identified 12 SKUs currently overpriced

Alert (automated):
- ProductA: Your price ₹12,999 vs competitor ₹11,799 (-9%)
- Impact: Projected 40 units/month lost (₹5.2L revenue)
- Recommendation: Match at ₹11,799 or bundle with accessories to justify premium
```

## Hands-On Exercises for Growisto Team

### Exercise 1: Analytics Mastery (30 minutes)

**Objective**: Learn to extract business insights without custom reports

**Tasks**:
1. Ask Sidekick: "What were our top 10 products last month by revenue?"
2. Follow-up: "Which of these had the highest profit margin?"
3. Advanced: "Show me customer acquisition cost by channel for customers who purchased these products"
4. Strategic: "Should we increase ad spend on the channel with the highest ROAS or lowest CAC? Why?"

**Expected Outcome**: Understand how to chain queries for strategic analysis.

---

### Exercise 2: Campaign Creation Sprint (45 minutes)

**Objective**: Build complete marketing campaign using only Sidekick

**Scenario**: You have 300 units of excess inventory (Product: "Festive Kurta Set")

**Tasks**:
1. Ask Sidekick to identify target customers (hint: past purchasers of ethnic wear)
2. Request campaign strategy (discount %, timing, channel)
3. Have Sidekick create:
   - Discount code
   - Customer segment
   - Email draft
   - Social media copy
4. Set up automated email with Sidekick's suggested timing

**Success Metric**: Campaign created and launched in <30 minutes.

---

### Exercise 3: Inventory Optimization (30 minutes)

**Objective**: Use AI forecasting to prevent stockouts and overstock

**Tasks**:
1. "Show me products at risk of stockout in next 14 days"
2. "Which products have >60 days of inventory?"
3. "Create a reorder recommendation report for our top 50 SKUs"
4. "Set up automated alerts when any product hits reorder point"

**Expected Outcome**: Proactive inventory management system.

---

### Exercise 4: Multi-Store Intelligence (For merchants with 2+ stores)

**Objective**: Gain cross-brand insights

**Tasks**:
1. "Compare average order value across all stores"
2. "Identify customer overlap between Store A and Store B"
3. "Which products in Store A would perform well in Store B based on customer preferences?"
4. "Create a unified best-sellers report across all brands"

**Expected Outcome**: Cross-pollination opportunities identified.

## Current Limitations & Roadmap

### Current Limitations (as of Feb 2026)

#### What Sidekick CAN'T Do (Yet):
1. **Execute third-party app configurations**: Can recommend apps but can't configure them
2. **Modify checkout customizations**: Shopify Scripts and checkout.liquid require manual editing
3. **Access historical data >2 years**: Analytics limited to 24-month lookback
4. **Generate design assets**: Can modify text/copy but not create graphics (use Shopify Magic for images)
5. **Process refunds/cancellations**: Can recommend actions but requires manual approval for financial transactions
6. **Custom development**: Can't write Liquid code or custom app integrations

#### Accuracy Considerations:
- **Data freshness**: Analytics are near-real-time but may have 5-10 minute delay
- **Predictive accuracy**: Forecasts are 75-85% accurate; use as guidance, not gospel
- **Context limitations**: Sidekick doesn't know external factors (competitors' sales, macro trends) unless you provide context

### Workarounds for Current Limitations:

**For third-party apps**:
```
Merchant: "Set up Klaviyo integration"
Sidekick: "I can't configure Klaviyo directly, but here's the step-by-step:
1. Install Klaviyo from App Store
2. Sync customer lists using these segments: [provides segment IDs]
3. Recommended flows: abandoned cart, welcome series, post-purchase
Need me to create the customer segments in Shopify first? [Yes/No]"
```

**For checkout customization**:
```
Merchant: "Add a survey question at checkout"
Sidekick: "I can't modify checkout directly (Plus-only feature), but I've prepared the code.
[Provides Liquid snippet]
Copy this to: Settings > Checkout > Additional Scripts
Want me to walk you through it?"
```

### Roadmap (2026-2027)

#### Q2 2026:
- **Autonomous campaigns**: Sidekick can create, launch, and optimize campaigns with one-click approval
- **Voice commerce**: "Sidekick, what sold today?" via mobile app
- **Visual dashboard generation**: "Create a dashboard for Diwali performance" → generates custom dashboard

#### Q3 2026:
- **Predictive demand forecasting**: 90-day forecasts with 90%+ accuracy
- **Automated supplier communication**: Sidekick drafts and sends reorder emails to suppliers
- **Multi-language support**: Conversations in Hindi, Tamil, Bengali, etc.

#### Q4 2026:
- **Cross-platform orchestration**: Sidekick manages inventory across Shopify + Amazon + Flipkart
- **AI-powered team delegation**: "Sidekick, assign this discount campaign to Priya and notify me when live"
- **Custom AI training**: Upload your brand guidelines, and Sidekick learns your specific tone/preferences

#### 2027:
- **Autonomous store operations**: Sidekick runs day-to-day operations (pricing, inventory, campaigns) with minimal human oversight
- **Industry-specific models**: Sidekick trained specifically for fashion, electronics, beauty, etc.

## Why This Matters for Indian Enterprise Merchants

### 1. **Talent Gap Bridge**
Finding experienced Shopify operators in Tier 2/3 cities is challenging. Sidekick democratizes expertise—a junior team member in Jaipur can perform like a senior analyst in Mumbai.

### 2. **Festive Commerce Agility**
During Diwali/BBD, decision velocity matters. Sidekick enables real-time campaign adjustments without waiting for analyst availability or BI tools.

### 3. **Cost Efficiency**
- **Traditional approach**: ₹15-25 LPA for senior e-commerce analyst
- **Sidekick approach**: ₹6-8 LPA junior + Sidekick = same output
- **Savings**: ₹10-15 LPA per analyst role

### 4. **24/7 Operations**
Sidekick doesn't sleep. Brands running midnight flash sales or serving global customers (NRI audience) benefit from always-on intelligence.

### 5. **Data Democracy**
Founders and marketing teams can access insights without waiting for tech teams to build reports. Faster iteration = competitive advantage.

## Best Practices for Growisto Partners

### 1. **Train Clients on "Chaining" Queries**
Poor: "Show me sales"
Good: "Show me sales by product category, then break down the top category by customer segment, then show me which segment has the highest repeat rate"

### 2. **Use Sidekick for Client Onboarding**
During implementation calls, use Sidekick to:
- Explain features to clients in real-time
- Generate sample reports to showcase capabilities
- Create configuration templates

### 3. **Build Sidekick Into SOPs**
Standard operating procedures should say: "Ask Sidekick for [X]" rather than "Use Analytics dashboard."

### 4. **Combine with Shopify Magic**
Sidekick for strategy + Shopify Magic for execution = powerful combo
Example: Sidekick identifies underperforming products → Magic generates new descriptions → Sidekick measures impact

### 5. **Document Sidekick "Recipes"**
Create a library of effective queries for common scenarios:
- Pre-Diwali inventory check
- Post-campaign attribution analysis
- Monthly business review generation
- New product launch checklist

## Key Takeaways

1. **Sidekick is an AI operator**, not just an analytics tool—it combines insights with action.

2. **Natural language unlocks velocity**—complex analyses that took hours now take minutes.

3. **Enterprise value = team multiplication**—one expert + Sidekick can manage workload of 3-4 traditional analysts.

4. **Best results come from conversation, not commands**—treat Sidekick like a smart colleague, not a search box.

5. **Continuous improvement**—Sidekick learns from merchant behavior and gets better over time.

---

**Next**: Doc 03 explores Unified Customer Profile and how AI powers predictive customer analytics.

**Document Version**: 1.0  
**Last Updated**: February 2026  
**Prepared for**: Growisto Partner Enablement
