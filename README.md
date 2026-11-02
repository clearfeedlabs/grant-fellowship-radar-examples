# Grant & Fellowship Radar: examples

Federal grant and fellowship alerts from Grants.gov, NSF and NIH in one table.

This repo shows how to call the [Grant & Fellowship Radar](https://apify.com/clearfeedlabs/grant-fellowship-radar) Apify Actor from JavaScript or Python and what the output looks like.

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

## Files
- `input.json`: a working example input
- `run.mjs` / `run.py`: run the Actor and print the first results
- `sample-output.json`: one trimmed example record (long fields shortened)

## Pricing
Pay per result on Apify. See the current price list on the [Store page](https://apify.com/clearfeedlabs/grant-fellowship-radar).

## Links
- Actor on the Apify Store: https://apify.com/clearfeedlabs/grant-fellowship-radar
- Guide: https://clearfeedlabs.com/guides/grant-fellowship-radar/
- Clearfeed Labs: https://clearfeedlabs.com
- Bugs or questions: open an issue on the Actor's Issues tab on Apify.

Data comes from public sources and is provided as-is. Check the original source before relying on it. Not legal, financial or investment advice.

License: MIT
