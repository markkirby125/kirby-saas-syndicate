# Kirby SaaS Syndicate: Launch Playbook

This skill automates the "SaaS Syndicate" launch strategy based on the Jackie Chow & David Quaid methodology (Episode 1184). It scaffolds multi-brand setups (the "NordVPN Tactic"), plans expired domain staging (the "Ryan Donnie" workflow), and architects parasite SEO operations.

## Stage 1: Interactive Intake

Prompt the user for the following information (if not running in `-y` or non-interactive mode. If non-interactive, use best-guess defaults from context):
1. **Target SaaS Niche & Core Function** (Used to slugify the path: apply NFKC normalization, then strictly match regex `^[a-z0-9]([a-z0-9-]{0,63})$`. Reject empty or traversal paths like `../`).
2. **Domain Strategy** (Expired Domain, Exact Match Domain (EMD), or Partial Match Domain (PMD)).
3. **Syndicate Scale** (How many "fake competitor" sibling brands to scaffold for the NordVPN Tactic? e.g., 3).
4. **Target Budget** for parasite placements and aged subreddits.

**Idempotency & Rerun Policy:** If the target workspace directory (always use absolute paths to avoid bare `./` traversal risks) already exists, pause and ask the user whether to `resume` (skip existing files), `clobber` (overwrite), or `abort`. Even in non-interactive mode, `clobber` requires explicit user confirmation to prevent data loss. Default to `resume` if no input is provided.

## Stage 2: On-Site Groundwork (Workspace Scaffolding)

Create the `[niche-slug]-syndicate/` directory (using absolute paths). **Before creating any files, explicitly echo the resolved absolute path to the user.** Populate it:

*   **`/strategy/`**
    *   `domain_staging_playbook.md`: Detailed steps for the "Ryan Donnie" expired domain workflow (buy expired domain, force index via Index Checks, send niche edits, rank, then link to main site and run Meta/Reddit ads through the backlink).
    *   `parasite_seo_plan.md`: Strategy for buying placements on AI-cited domains (ChatGPT/Overviews), publishing on high-authority sites (Medium, LinkedIn), 301-redirecting dead domains to those parasites, and acquiring aged subreddits.
*   **`/brands/`**
    *   For each brand requested in the Syndicate Scale (e.g., `brand-1`, `brand-2`, `brand-3`), scaffold a directory.
    *   *Warning:* Do not over-engineer on-site SEO for these domains during the first 3 months to avoid the Google Sandbox. Output lightweight HTML/MD stubs and "vibe-coding" product architecture guidelines.
    *   Ensure separate back-end configurations are planned but core logic is shared.

## Stage 3: Guardrails & Execution Rules

*   **Guardrail:** You MUST require explicit user confirmation before executing any "parasite SEO", "301 redirect mapping", or "subreddit acquisition" tactics to ensure compliance with terms of service and risk tolerance.
*   **Guardrail:** You MUST ensure proper FTC disclosure guidelines are documented for the "NordVPN Tactic" (owning multiple brands on the same listicle).
*   **Cross-Skill Routing:** For general off-page execution details or link building, refer to the [kirby-off-page-seo](../../kirby-off-page-seo/SKILL.md) skill.
*   **Hollow Shell Rule:** The full logic lives here in `00_dispatcher.md`. Never alter `../SKILL.md`.
