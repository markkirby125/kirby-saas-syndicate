# Module 3: The 1v1 Versus Spoke Intercept Network (Rob Hoffman BOFU Comparison Cluster)

*Source: Rob Hoffman ("How To Build A Page That Ranks #1 On ChatGPT (AI SEO Tutorial)", `OUEELIis-do` / Teamtown BOFU comparison cluster case study).*

When deploying comparison architecture across primary challenger brands and eligible post-sandbox satellite properties (subject to the 90-day sandbox cap in Stage 2, the 4-Point Mountain Verification Gate in Stage 3, and the dedicated-review-satellite prohibition in [`kirby-seo-deployment`](../../kirby-seo-deployment/SKILL.md) Module 17 §17.5), integrate the **1v1 Versus Spoke Intercept Network** ([`kirby-aiseo-skill`](../../kirby-aiseo-skill/SKILL.md) Module 2 §2.50 & Module 10 §10.11F).

---

## 3.1 The Unbranded-to-Branded Sequencing Law (`Alternatives Hub` First ➔ `1v1 Versus Spokes` Second)

* **Why Sequence Matters:** Prospects fleeing an overpriced enterprise incumbent do not know a challenger or syndicate brand's name yet — zero buyers search `"[Challenger] vs [Incumbent]"` before discovery. They search `"[Incumbent] alternatives"` (unbranded switching intent).
* **Step 1 (Unbranded Capture):** Deploy the flagship **`[Incumbent] Alternatives` Hub** (`/blog/[incumbent]-alternatives`) first to capture high-intent unbranded switching demand (`../../kirby-zero-to-100-seo/SKILL.md` §2.1 Incumbent Ad-Spend Intercept Play). Position the challenger transparently with explicit first-person bias disclosure (*"Position #1 is our company, discount accordingly"*), selectable HTML `<table>` data (`<33d` verified pricing timestamp), and symmetrical competitor strengths (*"When [Incumbent] May Still Be the Better Fit"*).
* **Step 2 (Branded Pairwise Conversion):** Once the Alternatives Hub introduces the challenger at #1 alongside category peers, prospects click through to the 1v1 pairwise spokes (`/comparisons/[incumbent]-vs-[challenger]`), converting unbranded discovery traffic into branded evaluation traffic while feeding AI crawlers dense entity-to-entity co-occurrence.

---

## 3.2 The Tri-Node Bidirectional Intercept Web (`Alternatives Hub` ↔ `Challenger vs Incumbent` ↔ `Competitor A vs Competitor B`)

Wire a closed, bidirectional internal linking mesh across the three comparison node types (strictly below the primary hero viewport inside competitor breakdown cards, the decision matrix, and comparison footers to preserve [`kirby-text-first-cro`](../../kirby-text-first-cro/SKILL.md) §6.4 & §10 item 11 hero link-minimalism):

```
┌─────────────────────────────────────────────────────────────────────────┐
│             1v1 VERSUS SPOKE INTERCEPT NETWORK TOPOLOGY                 │
├─────────────────────────────────────────────────────────────────────────┤
│                     [Node 1: Alternatives Hub]                          │
│                  /blog/[incumbent]-alternatives                         │
│                    (Unbranded Discovery Entry)                          │
│                         ▲               ▲                               │
│                         │               │                               │
│                         ▼               ▼                               │
│   [Node 2: Challenger vs Incumbent] ◄─► [Node 3: Competitor A vs B]     │
│   /comparisons/[incumbent]-vs-[brand]   /comparisons/[comp-a]-vs-[comp-b]│
│     (Direct Pairwise Conversion)          (Sideways Rival Intercept)    │
└─────────────────────────────────────────────────────────────────────────┘
```

1. **Node 1 (`Alternatives Hub` — `/blog/[incumbent]-alternatives`):**
   - Inside the #1 Challenger card (*"Want to go deeper? Read our full [Challenger] vs [Incumbent] comparison"*) and the bottom `"Which [Incumbent] Alternative Is Right for You?"` decision matrix, link out to every 1v1 spoke (`/comparisons/[incumbent]-vs-[challenger]`, `/comparisons/[competitor-a]-vs-[challenger]`, `/comparisons/[competitor-a]-vs-[competitor-b]`) and to sibling alternatives hubs (`/blog/[competitor-a]-alternatives`).
2. **Node 2 (`Challenger vs Incumbent` Spoke — `/comparisons/[incumbent]-vs-[challenger]`):**
   - Deep head-to-head teardown comparing contract lock-ins, hidden platform fees, turnaround SLAs, and verifiable G2/Trustpilot/Reddit review sentiment (`../../kirby-off-page-seo/SKILL.md` Module 26 §26.3).
   - Links back up to the parent `Alternatives Hub` and laterally to `Competitor A vs Competitor B` spokes for buyers whose use case fits neither.
3. **Node 3 (`Competitor A vs Competitor B` Neutral Intercept Spoke — `/comparisons/[competitor-a]-vs-[competitor-b]`):**
   - Captures sideways comparison searches between two third-party rivals (`../../kirby-aiseo-skill/SKILL.md` Module 2 §2.16.1C), evaluates both fairly using the 99%/1% Consensus Rule, introduces the Challenger as the high-value third option for mid-market buyers, and links back to both the `Alternatives Hub` and the `Challenger vs Incumbent` spoke.

---

## 3.3 Syndicate Satellite Governance & FTC Disclosure Invariants

* **No Fake "Independent Review Bureau" Satellites:** Never spin up fake neutral third-party review domains to rank comparison spokes (`../../kirby-seo-deployment/SKILL.md` Module 17 §17.5). Comparison clusters must live on real product domains or disclosed editorial properties with genuine utility and pass the 4-Point Mountain Verification Gate (`00_dispatcher.md` Stage 3).
* **Mandatory FTC Common-Ownership Disclosure:** Whenever two or more syndicate brands owned by the same parent appear inside an `Alternatives Hub`, `Challenger vs Incumbent` spoke, or `Competitor A vs Competitor B` matrix, enforce the `00_dispatcher.md` Stage 3 FTC guardrail: disclose common ownership visibly and in plain words near the top of the page, use real verified founder/SME bylines (headshot + LinkedIn/X links), and log all cross-brand links in `brands/footprint_log.md`.
