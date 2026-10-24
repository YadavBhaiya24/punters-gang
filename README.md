# Punters Gang Cricket Hub (starter)

A mobile-friendly static cricket companion website with:
- Match Centre with clearly labelled sample fixtures
- Match-analysis placeholder section
- Odds implied-probability calculator
- Potential return calculator
- Current and required run-rate calculators
- Local demo prediction poll
- Local personal record tracker
- Responsive dark dashboard

## Important
This starter does **not** show real live scores. Sample fixtures and analysis are explicitly labelled. The page refreshes its demo panel automatically, but a real live score feed requires a cricket data provider API and a server-side integration. Do not put private API keys in `index.html`. The demo poll and tracker save only in the current browser/device; they are not shared between Telegram members. There is no betting placement, payment, or guaranteed prediction feature.

## Deploy free with Cloudflare Pages
1. Extract this ZIP.
2. Create a GitHub repository and upload `index.html` (and this README if you like).
3. Open https://pages.cloudflare.com/ and sign in.
4. Create a Pages project and connect your GitHub repository.
5. Use the root directory as the project root. For a plain static site, no build command is needed; set the output directory to `/` if the setup asks for one.
6. Deploy and open the provided `pages.dev` address.

You can also use GitHub Pages for a simple static version.

## To make it truly automatic
- Choose a cricket data API plan with live fixtures/score endpoints.
- Add a server-side endpoint (e.g. a Cloudflare Pages Function) that reads the API key from environment secrets.
- Update the Match Centre to fetch your endpoint and handle rate limits, errors, and provider attribution.
- For shared polls/leaderboards, add a backend/database and appropriate spam protection.
