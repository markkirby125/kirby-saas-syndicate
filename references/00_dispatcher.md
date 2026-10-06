# Kirby SaaS Syndicate: Launch Playbook

This skill automates the "SaaS Syndicate" launch strategy based on the Jackie Chow & David Quaid methodology (Episode 1184). It scaffolds multi-brand setups (the "NordVPN Tactic"), plans expired domain staging (the "Ryan Donnie" workflow), and architects parasite SEO operations.

## Stage 1: Interactive Intake

Prompt the user for the following information (if not running in `-y` or non-interactive mode. If non-interactive, use best-guess defaults from context):
1. **Target SaaS Niche & Core Function** (Used to slugify the path: apply NFKC normalization, lowercase, strip diacritics, replace non-alphanumerics with hyphens, and strictly match regex `\A[a-z0-9]([a-z0-9-]{0,62})[a-z0-9]\Z` to prevent newlines and traversal paths like `../`).
2. **Domain Strategy** (Branch output based on: Expired Domain/EMD ($2k-$3k for domains with historical interaction), or PMD (to confuse Google regarding exact entity)).
3. **Syndicate Scale** (How many separate-brand products with the same tech but separate back-ends to scaffold for the NordVPN Tactic? e.g., 3).
4. **Target Budget** (Branch parasite plan based on budget: e.g. $500-$5k for placements, $5k-$50k for aged subreddits).

**Idempotency & Rerun Policy:** Verify the target absolute path is a directory (not a file or symlink). If the directory already exists, pause and ask the user whether to `resume` (skip existing files), `clobber` (safely empty the directory), or `abort`. Even in non-interactive mode, `clobber` requires explicit user confirmation to prevent data loss. Default to `resume` if no input is provided.

## Stage 2: On-Site Groundwork (Workspace Scaffolding)

Create the `[niche-slug]-syndicate/` directory (using absolute paths). **Before creating any files, explicitly echo the resolved absolute path to the user.** Populate it:

*   **`/strategy/`**
    *   `domain_staging_playbook.md`: Detailed steps for the "Ryan Donnie" workflow (buy expired domain, check Wayback Machine for relevance, rebuild with historical content, force index via Index Checks, send niche edits, rank, then link to main site and run Meta/Reddit ads through the backlink). Branch strategies based on Intake Step 2.
    *   `parasite_seo_plan.md`: Strategy for buying placements on high-ranking listicles, publishing on high-authority sites (Medium, LinkedIn), 301-redirecting dead/penalized domains to the root URL of your parasite profile (e.g. linkedin.com/in/yourname), and acquiring aged subreddits. Tailor to the budget from Intake Step 4.
*   **`/brands/`**
    *   For each brand requested in the Syndicate Scale (e.g., `brand-1`, `brand-2`, `brand-3`), scaffold a directory with an explicit file manifest (e.g., `index.html`, `vibe_coding_prompt.md`).
    *   *Warning:* Do not over-engineer on-site SEO for these domains during the first 3 months to avoid the Google Sandbox. Output lightweight HTML/MD stubs and "vibe-coding" product architecture guidelines.
    *   Ensure separate back-end configurations are planned but core logic is shared.

## Stage 3: Guardrails & Execution Rules

*   **Guardrail:** You MUST require explicit user confirmation before executing any "parasite SEO", "301 redirect mapping", or "subreddit acquisition" tactics. Note that buying aged subreddits is a black-market tactic that violates terms of service; ensure the user accepts this risk.
*   **Guardrail:** You MUST ensure proper FTC disclosure guidelines are documented for the "NordVPN Tactic" (owning multiple brands on the same listicle).
*   **Cross-Skill Routing:** For general off-page execution details or link building, refer to the [kirby-off-page-seo](../../kirby-off-page-seo/SKILL.md) skill.
*   **Hollow Shell Rule:** The full logic lives here in `00_dispatcher.md`. Never alter `../SKILL.md`.
