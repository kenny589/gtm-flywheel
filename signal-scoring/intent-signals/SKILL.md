---
name: intent-signals
description: "Detect, categorize, and score buying intent signals from multiple data sources. Transform raw company activity into actionable outreach triggers."
---

# Intent Signals

## When to Use
- Building signal-based outbound campaigns (vs. spray-and-pray)
- Setting up monitoring systems for real-time prospect alerts
- Prioritizing which accounts to contact first from a large list
- Training SDRs or AI systems on what qualifies as a meaningful buying signal

## Framework

### What Intent Signals Are

An intent signal is any observable action or change that suggests a company or person may be ready to buy. It's the difference between "this company matches our ICP" (fit) and "this company matches our ICP AND is actively looking for a solution" (fit + intent).

**Fit alone:** "They're a 200-person SaaS company in our target industry."
**Fit + Intent:** "They're a 200-person SaaS company that just posted 3 SDR job openings, raised a Series B last month, and their VP Sales is engaging with content about outbound scaling."

Intent signals don't guarantee a sale. They guarantee **relevance** — which is the single most important factor in cold outreach conversion.

---

### The Intent Signal Taxonomy

All intent signals fall into one of four categories, each with different reliability and actionability:

#### Category 1: First-Party Signals (Highest Reliability)
*Actions the prospect takes that directly involve your brand.*

| Signal | Reliability | Urgency | Example |
|--------|------------|---------|---------|
| Visited your website (specific pages) | Very High | High | Viewed pricing page twice in one week |
| Downloaded your content | Very High | Medium-High | Downloaded "Outbound Playbook" guide |
| Attended your webinar | Very High | Medium | Registered and attended live |
| Replied to previous outreach positively | Very High | Very High | "Not now, but reach back out in Q2" |
| Free trial or demo request | Very High | Critical | — |
| Opened previous emails (multiple times) | Medium | Medium | Opened 3 emails but didn't reply |

**Challenge:** You need website tracking, marketing automation, and CRM data to capture these. Many companies don't have this infrastructure.

#### Category 2: Third-Party Intent Signals (High Reliability)
*Actions the prospect takes on other platforms that suggest buying intent.*

| Signal | Reliability | Urgency | Detection Method |
|--------|------------|---------|-----------------|
| Researching your category on G2/Capterra | High | Very High | G2 Buyer Intent, Capterra alerts |
| Searching for competitor alternatives | High | Very High | Intent data providers (Bombora, 6sense) |
| Consuming content about your problem space | Medium-High | Medium | Topic-based intent providers |
| Engaging with competitor content | Medium | Medium | Social monitoring |
| Posting questions in relevant communities | Medium | Medium-High | Reddit, Slack communities, forums |

**Challenge:** Requires paid intent data subscriptions. Quality varies wildly by provider.

#### Category 3: Public Signals (Medium Reliability, Free)
*Observable events anyone can detect with the right monitoring.*

| Signal | Reliability | Urgency | Source |
|--------|------------|---------|--------|
| **Hiring signals** | High | High | LinkedIn Jobs, Indeed, careers page |
| **Funding announcements** | High | Medium-High | Crunchbase, TechCrunch, press releases |
| **Leadership changes** | Medium-High | Medium | LinkedIn, press releases |
| **Product launches** | Medium | Medium | Company blog, PR, Product Hunt |
| **Tech stack changes** | Medium | Medium-High | BuiltWith, Wappalyzer, job descriptions |
| **Earnings reports** | Medium | Low-Medium | SEC filings, press releases |
| **Awards/recognition** | Low-Medium | Low | Industry publications |
| **Conference speaking** | Low-Medium | Low | Event websites |
| **Office expansion** | Medium | Medium | News, job listings in new locations |
| **M&A activity** | High | Medium | News, SEC filings |

**Advantage:** Free and widely available. These should be the backbone of any signal-based outbound strategy.

#### Category 4: Social Signals (Variable Reliability)
*Content the prospect publishes or engages with on social platforms.*

| Signal | Reliability | Urgency | Source |
|--------|------------|---------|--------|
| Posted about a pain you solve | High | High | LinkedIn, Twitter |
| Shared a competitor's content | Medium | Medium | LinkedIn, Twitter |
| Asked for vendor recommendations | Very High | Very High | LinkedIn, communities |
| Commented on industry trends related to your space | Medium | Low-Medium | LinkedIn |
| Changed their LinkedIn headline (new role) | High | High | LinkedIn notifications |
| Published a thought leadership piece on your topic | Medium | Medium | LinkedIn, company blog |

---

### Signal Scoring Model

Not all signals are equal. Score each signal to prioritize outreach:

#### Signal Strength Matrix

| Factor | High Score | Medium Score | Low Score |
|--------|-----------|-------------|-----------|
| **Recency** | Last 7 days | Last 30 days | 30-90 days |
| **Directness** | Explicit buying action (demo request, vendor search) | Implicit buying action (hiring, funding) | Tangential (content consumption) |
| **Frequency** | Multiple signals in same timeframe | Single signal | Historical signal |
| **Specificity** | Specific to your exact category | Related to your general space | Broadly related |
| **Source reliability** | First-party or verified third-party | Public, verifiable | Inferred or aggregated |

**Maximum signal age.** A signal older than the campaign's maximum signal age (see the Signal-Based Campaign Brief) is not a signal: don't score it. If no maximum is set, use 90 days, where the Recency column ends.

#### Scoring Formula

```
Signal Score = (Recency × 3) + (Directness × 3) + (Frequency × 2) + (Specificity × 1) + (Source × 1)
```

Each factor rated 1-5:

| Score | Priority | Action |
|-------|----------|--------|
| 40-50 | Critical | Contact within 24 hours |
| 30-39 | High | Contact within 3 days |
| 20-29 | Medium | Include in next campaign batch |
| 10-19 | Low | Add to monitoring list |
| Below 10 | Noise | Ignore |

---

### Signal Combinations (Stacking)

Single signals are useful. Signal combinations are powerful. When multiple signals converge, the probability of buying intent increases dramatically:

#### High-Confidence Combinations

| Combination | Confidence | Why |
|------------|-----------|-----|
| Funding + Hiring for target role | Very High | Money + action = active buying cycle |
| Leadership change + Tech evaluation (G2) | Very High | New leader re-evaluating the stack |
| Hiring SDRs + Content about scaling outbound | High | Building the function + researching solutions |
| Competitor churn + Your website visit | Very High | Actively looking for alternatives |
| Conference in your space + LinkedIn post about the topic | Medium-High | Problem is top of mind |

#### Signal Stacking Rules

1. **Two signals from different categories = 2x the score.** A hiring signal (public) + a G2 research signal (third-party) is much stronger than two hiring signals.

2. **Recency trumps everything.** A weak signal from yesterday beats a strong signal from 3 months ago.

3. **Person-level signals > Company-level signals.** The VP Sales posting about outbound challenges (person) is stronger than the company posting 3 SDR jobs (company) — because you know exactly WHO is feeling the pain.

4. **Don't stack noise.** Three weak signals don't equal one strong signal. "Posted on LinkedIn" + "website has a blog" + "company is in tech" = noise, not intent.

---

### Building a Signal Monitoring System

#### Manual Monitoring (0 cost, 30 min/day)

| Activity | Frequency | Tool |
|----------|-----------|------|
| Check LinkedIn for job postings at target accounts | Daily | LinkedIn Jobs search, saved searches |
| Monitor Crunchbase for funding in your verticals | Weekly | Crunchbase alerts (free tier) |
| Track LinkedIn posts from target personas | Daily | LinkedIn feed, saved searches |
| Check Google Alerts for target companies | Daily | Google Alerts (free) |
| Scan industry communities for vendor questions | Weekly | Reddit, Slack groups, forums |

#### Automated Monitoring (Paid tools)

| Tool Category | Examples | What It Monitors |
|--------------|---------|-----------------|
| **Intent data** | Bombora, 6sense, ZoomInfo Intent | Category-level research signals |
| **Job monitoring** | LinkedIn Recruiter, Otta, PredictLeads | Hiring signals |
| **Funding alerts** | Crunchbase Pro, PitchBook | Capital events |
| **Tech detection** | BuiltWith, Wappalyzer, HG Insights | Stack changes |
| **Social monitoring** | Mention, Brand24, PhantomBuster | Social signals |
| **Website tracking** | Clearbit Reveal, RB2B, Leadfeeder | Website visit signals |

#### Signal Pipeline Architecture

```
Data Sources (APIs, scraping, alerts)
    ↓
Signal Detection Layer
    → Parse raw data for relevant signals
    → Categorize (hiring, funding, tech, social, first-party)
    ↓
Scoring Engine
    → Apply signal scoring formula
    → Stack multiple signals per account
    → Calculate composite score
    ↓
Prioritization Queue
    → Tier 1 (score 40+): Immediate outreach
    → Tier 2 (score 30-39): Next batch
    → Tier 3 (score 20-29): Add to campaign
    → Below 20: Monitor or discard
    ↓
Outreach Trigger
    → Route to appropriate campaign
    → Match signal to personalization angle
    → Enrich contact data if needed
```

---

### Signal-to-Message Mapping

Every signal should map to a specific outreach angle:

| Signal | Opening Line Approach | Campaign Angle |
|--------|---------------------|----------------|
| Hiring SDRs | "Building the outbound team?" | Scaling outbound |
| Series B funding | "Post-Series B is when pipeline becomes a board metric" | Growth acceleration |
| New VP Sales | "First 90 days in a new VP Sales role..." | New leader priorities |
| Competitor evaluation | "Evaluating {{category}}? Here's what teams miss" | Competitive displacement |
| Tech stack change | "Migrating to {{tool}} — most teams also rethink..." | Stack optimization |
| LinkedIn post about pain | "Your post about {{topic}} resonated" | Thought leadership bridge |
| Conference attendance | "Ahead of {{event}}, thought you'd find this relevant" | Event-based relevance |

## Templates

### Signal Tracking Sheet
```
| Company | Signal Type | Signal Detail | Date Detected | Source | Score | Action | Status |
|---------|------------|--------------|---------------|--------|-------|--------|--------|
| ___ | ___ | ___ | ___ | ___ | ___/50 | ___ | ___ |
```

### Signal-Based Campaign Brief
```
Campaign: {{campaignName}}
Target Signal: {{primarySignal}}
Supporting Signals: {{secondarySignals}}

Signal Detection:
- Source: {{dataSource}}
- Refresh frequency: {{howOften}}
- Estimated volume: {{leadsPerWeek}}

Personalization Map:
- Opening line template: "___"
- Value prop connection: "___"
- CTA: "___"

Qualification Threshold:
- Minimum signal score: ___
- Required firmographic fit: ___
- Maximum signal age: ___ days
```

## Tips
- The best time to email someone is within 48 hours of a signal firing. After 2 weeks, the signal is stale and your "I noticed..." line sounds like a lie.
- Don't chase every signal. Pick 2-3 signal types that correlate with your highest close rates and build systematic monitoring around just those. Depth beats breadth.
- Hiring signals are the single most reliable free signal for B2B outbound. If a company is hiring for the role your product serves, they are actively investing in that function.
- Person-level signals always beat company-level signals. "The VP Sales posted about needing better pipeline visibility" is 10x more actionable than "the company raised a round."
- Create a feedback loop: track which signal types lead to the most meetings. After 3 months, double down on the winners and drop the losers.
- Signal + fit > fit alone > signal alone. A perfectly matched ICP company with intent signals is your #1 priority. A perfectly matched ICP company with no signals is Tier 2. A non-ICP company with signals is usually noise — don't chase it.

---

*Progressive disclosure: load signal provider integrations and API configurations only when setting up monitoring for a specific campaign.*
