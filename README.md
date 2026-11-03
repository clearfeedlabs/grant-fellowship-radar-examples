# Grants.gov Scraper & Grant Finder API: NSF, NIH Fellowships: examples

Federal grant and fellowship alerts from official Grants.gov, NSF Award Search and NIH RePORTER APIs. Filter by keyword, agency, eligibility, category and deadline window. Normalized, deduplicated rows, new-since-last-run mode and 30/7-day deadline alerts.

This repo shows how to call the [Grant & Fellowship Radar](https://apify.com/clearfeedlabs/grant-fellowship-radar) Apify Actor from JavaScript or Python, and what the output looks like.

## What's new
- Phrase search for multi-word keywords, title matches ranked first, new `keywordMatch` field; "machine learning" now returns 8/8 relevant rows in ~11 s (was 1 row in 74 s).

## Use cases
- Graduate students and postdocs looking for fellowships
- Research labs and sponsored-programs offices tracking deadlines
- Nonprofits watching federal funding in their field
- Seeing who won similar awards before you apply

## Quick start
1. Create a free Apify account and copy your API token from Settings > Integrations.
2. Set it as an environment variable: `export APIFY_TOKEN=...` (never commit it).
3. Edit `input.json`, then run one of:
   - JavaScript: `npm i apify-client && node run.mjs`
   - Python: `pip install apify-client && python run.py`

## Output fields (first of many)
`duplicateListings`, `rowType`, `source`, `id`, `isNew`, `isUpdated`, `opportunityNumber`, `title`, `agency`, `agencyCode`, `status`, `postedDate`, `closeDate`, `daysUntilDeadline`, `deadlineUrgency`, `archiveDate`, `awardFloorUsd`, `awardCeilingUsd`

See `sample-output.json` for one trimmed record.

## Ready-made example tasks
- [Graduate fellowships closing soon](https://apify.com/clearfeedlabs/grant-fellowship-radar/examples/graduate-fellowships-closing-soon)
- [Machine learning ai research funding](https://apify.com/clearfeedlabs/grant-fellowship-radar/examples/machine-learning-ai-research-funding)
- [Nih health research grants awards](https://apify.com/clearfeedlabs/grant-fellowship-radar/examples/nih-health-research-grants-awards)

## Pricing
Pay per result: **$2.00 per 1,000 rows**, with no subscription. The [Store page](https://apify.com/clearfeedlabs/grant-fellowship-radar) always shows current prices and every optional add-on event.

## Related Clearfeed Labs Actors
- [USAspending Scraper: Federal Contract & Grant Award Alerts](https://apify.com/clearfeedlabs/money-trail-federal-awards): federal contract and grant awards with recompete details
- [ClinicalTrials.gov Scraper & Trial Change Tracker: PubMed + FDA](https://apify.com/clearfeedlabs/clinical-trial-tracker): ClinicalTrials.gov changes and new trials
- [Internship & New Grad Jobs Scraper API + H-1B Sponsors](https://apify.com/clearfeedlabs/entry-jobs-feed): internships and new-grad roles with H-1B history
- [All Clearfeed Labs Actors](https://apify.com/clearfeedlabs)

## FAQ
**Is this data official?** Yes. It comes from the public source named above, and each record links back to it.
**Do I need a login or proxy?** No. It uses documented public endpoints only.
**Can I schedule it?** Yes. Use Apify Schedules, the API or integrations (Zapier, Make, webhooks, MCP-compatible AI agents).

## Links
- Actor on the Apify Store: https://apify.com/clearfeedlabs/grant-fellowship-radar
- Details & pricing: https://clearfeedlabs.com/actors/grant-fellowship-radar/
- Clearfeed Labs: https://clearfeedlabs.com
- Bugs or questions: open an issue on the Actor's Issues tab on Apify.

Data comes from public sources and is provided as-is. Check the original source before relying on it. Not legal, financial or investment advice.

License: MIT
