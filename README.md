# GOD'S PLAN

**Create Your Own Future.** GOD'S PLAN is an early personal strategy workspace for turning goals into practical actions, recording progress, and reviewing what to improve.

## Current web version

The deployed entry point is `index.html`. It is a static, single-page HTML/CSS/JavaScript application; no build step or package installation is currently required.

### Run locally
1. Clone this repository.
2. Open `index.html` in a modern browser.
3. Export your data if you want to keep a copy.

## Implemented in the current browser version

- Goal and constraint inputs (available time, budget, skills, experience).
- Rule-based strategy draft and daily action suggestions.
- Editable execution task list with completion tracking.
- Daily practice log and progress chart.
- JSON export/import for user-managed backups.
- Rule-based strategy review (not a live AI response).
- Share text and share-card image generation.
- Korean, English, Chinese, and Japanese interface text.

## Important limitations

- Tasks and practice logs are held in the current browser session's JavaScript memory. Refreshing or closing the page can clear them.
- JSON export/import is the current manual backup path; it is not automatic cloud sync.
- Strategy draft and review are local rule-based examples. No model API is called by this page.
- There is no account system, server-side database, payment integration, or subscription entitlement in this repository.
- Do not enter sensitive personal information. Shared cards can include text entered by the user.

Do not describe proposed capabilities as live features.

## Product direction

Long-term vision: **Personal Strategy OS**. Initial product focus: help a person clarify a goal and real-world constraints, compare practical options, turn a selected direction into small actions, record execution, and use outcomes to improve the next plan.

Core loop: `Goal → Diagnosis → Options → Strategy → Execution → Results → Review → Updated strategy`.

## Repository map

- `index.html` — current Vercel static-site entry point.
- `gods_plan_green_premium (1).html` — retained alternate HTML version; confirm its purpose before replacing or deleting it.

## Development principles

1. Preserve the working public prototype while changes are reviewed.
2. Make changes on a feature branch and use a pull request before merging to `main`.
3. Separate implemented, proposed, and verified features.
4. Never put private API keys in browser JavaScript or committed files. Future AI integration must use a server-side endpoint that protects credentials and validates input.
5. Test data export/import and existing workflows whenever changing the application.
