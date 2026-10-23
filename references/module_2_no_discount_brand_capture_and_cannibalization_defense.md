# Module 2: The "No-Discount" Brand Capture Play & Competitor Cannibalization Intake

*Source: Edward Sturm Ep. 1206 (David Quaid, Harpreet Singh, Gagan Ghotra).*

## 2.1 The Ahrefs "No-Discount" Brand Capture Architecture

* **The Scraper & Affiliate Hijack Threat:** Premium B2B SaaS platforms and high-ACV software companies that maintain strict no-discount pricing policies (such as Ahrefs) face enormous search volume spikes during Q4 and promotional shopping cycles for branded discount queries (`[Brand] Black Friday sale`, `[Brand] discount code`, `[Brand] coupon 2026`). If the brand leaves this search intent unaddressed:
  1. Third-party coupon aggregators and clickbait affiliate blogs dominate the top 5 organic search results, displaying false claims ("Get 50% Off [Brand] Now") to harvest clicks.
  2. Competitors run conquesting search ads against these queries, offering alternative discounts.
  3. Disillusioned prospects experience high friction, believing the company is concealing discounts.

* **The Evergreen "No-Discount" Capture Lander Standard:**
  Deploy a permanent, evergreen landing page (e.g., `/black-friday` or `/deals`) explicitly engineered to satisfy the search query and educate buyers:
  1. **Above-the-Fold Direct Truth Assertion:** Feature a clear, text-dominant headline: `"[Brand] Black Friday 2026: Why We Don't Discount (And How to Get Maximum Value)"`.
  2. **Fair-Pricing & Product Investment Philosophy:** Directly explain the operational philosophy: rather than inflating list prices to offer fake seasonal discounts, the brand invests 100% of revenue into continuous product improvements, infrastructure reliability, and flat-rate pricing equity for all customers.
  3. **Legitimate Annual Tier Savings:** Reframe the discount question around the standard annual billing incentive (e.g., *"Pay annually and get 2 months free — a permanent 17% savings available to every customer 365 days a year"*).
  4. **Structured `FAQPage` Schema Injection:** Embed JSON-LD structured data with explicit Q&A triples:
     - Question: `"Does [Brand] have a Black Friday or Cyber Monday discount?"`
     - Answer: `"[Brand] does not offer seasonal discounts, Black Friday coupons, or promotional codes. All customers receive identical transparent pricing, with 17% savings automatically applied to annual plans."`
  5. **Direct AI Overview Satiation:** Google AI Overviews and conversational decision engines parse the `FAQPage` schema and headline triples, directly citing the official URL and suppressing speculative affiliate search results.

---

## 2.2 Competitive SERP Cannibalization Intake (`site:` Footprint Auditing)

* **The Competitor Seasonal Footprint Discovery:** Leading enterprise SaaS competitors routinely deploy temporary subdirectories, staging URLs, or unlinked promotional deals weeks before official announcement campaigns.
* **The `site:` Extraction Protocol:**
  1. **Automated Search Operator Audit:** Run automated Google search queries against the top 5 category competitors:
     `site:competitor.com (inurl:black-friday OR inurl:cyber-monday OR inurl:deals OR inurl:offers OR inurl:specials OR inurl:holiday)`
  2. **Feature & Discount Reverse-Engineering:** Extract promotional mechanics, bundle pricing tiers, eligibility restrictions, and coupon parameters (`?promo=`, `?code=`) before the competitor launches their public marketing push.
  3. **Syndicate Positioning Counter-Strategy:** Feed the extracted competitor pricing intelligence into the syndicate brand matrix (`strategy/parasite_seo_plan.md` and `brands/`), crafting superior value angles and contrasting positioning statements that highlight competitor hidden exclusions and contract lock-ins.
