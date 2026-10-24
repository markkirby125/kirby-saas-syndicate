# Kirby SaaS Syndicate: Launch Playbook

This skill automates the "SaaS Syndicate" launch strategy based on the Jackie Chow & David Quaid methodology (Episode 1184). It scaffolds multi-brand setups (the "NordVPN Tactic"), plans expired domain staging (the "Ryan Donnie" workflow), and architects parasite SEO operations.

## Stage 1: Interactive Intake

Prompt the user for the following information (if not running in `-y` or non-interactive mode. If non-interactive, use best-guess defaults from context):
1. **Target SaaS Niche & Core Function** (Used to slugify the path: apply NFKC normalization, lowercase, strip diacritics, replace non-alphanumerics with hyphens, and strictly match regex `\A[a-z0-9]([a-z0-9-]{0,62})[a-z0-9]\Z` to prevent newlines and traversal paths like `../`).
2. **Domain Strategy** (Branch output based on: Expired Domain/EMD [$2k-$3k for domains with historical interaction], or PMD [to confuse Google regarding exact entity]. *EMD Doorway Risk Caution*: The 2026 SEO Meta Study [Ćorluka Zenodo DOI: 10.5281/zenodo.22768160; Ep. 1191/1207] confirms that shotgun-launching thin programmatic doorway directories on fresh or EMD domains triggers rapid algorithmic suppression and template de-indexing ['Mountain Pattern' collapse]. EMD syndicate sites MUST incorporate proprietary data density or an authentic interactive utility).
3. **Syndicate Scale** (How many separate-brand products with the same tech but separate back-ends to scaffold for the NordVPN Tactic? e.g., 3).
4. **Target Budget** (Branch parasite plan based on budget: e.g. $500-$5k for placements, $5k-$50k for aged subreddits).

**Idempotency & Rerun Policy:** Verify the target absolute path is a directory (not a file or symlink). Gate `resume` logic by checking for a `.kirby-syndicate-marker` file (written only upon successful completion of scaffolding). Keep a rollback log of created paths, and use `mkdir` exclusive mode with rollback on partial failure. If the directory already exists without a marker, treat as an interrupted or foreign directory and prompt for `clobber`/`abort` (never `resume`). If the directory exists with a marker, pause and ask whether to `resume` (skip existing files), `clobber` (safely empty the directory), or `abort`. In non-interactive mode, refuse `clobber` outright. Default to `resume` if no input is provided.

## Stage 2: On-Site Groundwork (Workspace Scaffolding)

Create the `[niche-slug]-syndicate/` directory (using absolute paths). **Before creating any files, explicitly echo the resolved absolute path to the user.** Populate it:

*   **`strategy/`**
    *   `domain_staging_playbook.md`: Detailed steps for the "Ryan Donnie" workflow (buy expired domain, check Wayback Machine for relevance, rebuild with historical content, force index via Index Checks, send niche edits, rank, then link to main site and run Meta/Reddit ads through the backlink). Branch strategies based on Intake Step 2. Also incorporate David Quaid's on-site entity takeover tactic (*"Who is the King of SEO?"* experiment, Ep 1202) using exact-match H1, slug, and H2s on the primary domain to force Google AI Overviews to attribute category leadership to the brand entity.
    *   `parasite_seo_plan.md`: Strategy for buying placements on high-ranking listicles, publishing on high-authority sites (Medium, LinkedIn), 301-redirecting dead/penalized domains to the root URL of your parasite profile (e.g. linkedin.com/in/yourname), and acquiring aged subreddits. Integrate Kyle Roof's Two-Factor Law: target high-traffic forum/community threads ranking #1–#5 on Google for parasite comments/citations, passing direct PageRank and triggering AI engine citations via clicked nofollow links (`../../kirby-off-page-seo/SKILL.md` Module 23). Tailor to the budget from Intake Step 4.
    *   `interactive_calculators_playbook.md`: Strategy for deploying client-side interactive calculators (e.g., ROI calculators, usage estimators, pricing simulators) as syndicate anchor assets. In the 2026 SEO Meta Study, editorial backlinks acquired through digital PR campaigns produced an as-reported directional average of **+71% organic sessions lift** (treat as a directional benchmark, not a guaranteed return). Scaffolds embeddable vanilla JS or lightweight calculators that act as high-yield link magnets for digital PR outreach and generate rich LLM citations per `../../kirby-off-page-seo/SKILL.md` Module 28.
*   **`brands/`**
    *   For each brand requested in the Syndicate Scale (e.g., `brand-1`, `brand-2`, `brand-3`), scaffold a directory with an explicit file manifest (e.g., `index.html`, `vibe_coding_prompt.md`).
    *   *Warning:* Do not over-engineer on-site SEO for these domains during the first 3 months to avoid the Google Sandbox. Output lightweight HTML/MD stubs and "vibe-coding" product architecture guidelines. One lightweight client-side calculator satisfies the interactive anchor requirement without bloating the crawl footprint; do not expand on-site page count beyond it during the 90-day sandbox window.
    *   Ensure separate back-end configurations are planned but core logic is shared.

## Stage 3: Guardrails & Execution Rules

*   **Guardrail:** You MUST require explicit user confirmation before executing any "parasite SEO", "301 redirect mapping", or "subreddit acquisition" tactics. Note that buying aged subreddits is a black-market tactic that violates terms of service; ensure the user accepts this risk.
*   **Guardrail:** You MUST ensure proper FTC disclosure guidelines are documented for the "NordVPN Tactic" (owning multiple brands on the same listicle).
*   **Mountain Pattern Safeguard:** Before deploying programmatic content directories across syndicate domains, apply the 4-Point Mountain Verification Gate (unique data density, context saturation, zero orphans, hard approval gate) defined in `../../kirby-zero-to-100-seo/SKILL.md` (dispatcher §2.2 *Controlled Launch Sequencing*) to prevent catastrophic template de-indexing.
*   **Cross-Skill Routing:** For off-page link building and digital PR interactive calculator workflows, route to `../../kirby-off-page-seo/SKILL.md` (Module 28). For entity attribution and knowledge graph anchoring, route to `../../kirby-technical-aeo/SKILL.md`.

## Module Index

- **Module 1: Parasite Expansion Pack — Google Domain Parasites, Platform Matrix, Arbitrage & CRO (Charles Floate E1193)** -> Read `./module_1_parasite_expansion_pack.md` (§1.1 SRA state + boundary test, §1.2 Google-domain parasites, §1.3 platform matrix, §1.4 5-step pipeline, §1.5 internal link arbitrage, §1.6 parasite CRO, §1.7 longevity/defense routing)
- **Module 2: The "No-Discount" Brand Capture Play & Competitor Cannibalization Intake (Gagan Ghotra, Harpreet Singh & David Quaid Ep. 1206)** -> Read `./module_2_no_discount_brand_capture_and_cannibalization_defense.md` (§2.1 Ahrefs-style "no-discount" brand capture landers and FAQ schema, §2.2 competitor `site:` operator footprint extraction)

**Parasite Expansion & Brand Capture routing:** When Stage 2 drafts `parasite_seo_plan.md` or brand landing strategies, apply Modules 1 and 2. Every tactic MUST first pass the SRA boundary test in `../../kirby-aiseo-skill/SKILL.md` Module 15 §15.3 (unmoderated authority-rental on legacy media — including unmoderated paid leases — is struck doctrine; moderated UGC/dev hubs remain open).
*   **Hollow Shell Rule:** The root `../SKILL.md` stays hollow; workflow logic lives here in `00_dispatcher.md`, and module doctrines live in `./module_*.md`.
