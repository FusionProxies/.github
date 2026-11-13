# Contributing

Thanks for helping. These repositories are small, practical tools and examples for working with proxies, and fixes from people who use them are welcome.

## Good contributions

- A bug fix, with the steps or input that showed the bug
- An example that no longer works with a current library version
- A missing proxy format, protocol or edge case in a tool
- Clearer wording where the documentation was confusing

Before a large change or a new feature, open an issue first so we can agree on the approach.

## How

1. Fork the repository and create a branch.
2. Make the change. Keep it focused: one fix or feature per pull request.
3. Run the tests if the repository has them:
   - Go: `go test ./...`
   - Python: `pip install -e ".[test]"` or `pip install -r requirements.txt pytest`, then `pytest`
4. Open a pull request and describe what changed and why.

## Rules

- Never commit real proxy credentials, API keys or customer data. Examples read `FUSION_USER` and `FUSION_PASS` from the environment.
- Examples should run against public test sites (for example `quotes.toscrape.com`, `books.toscrape.com`) or the user's own targets, and respect `robots.txt` and the sites' terms.
- Contributions are released under the repository's license (MIT).

## Questions about your account

Billing, plans, credentials and proxy issues on your account are handled by support, not in GitHub issues: see [SUPPORT.md](SUPPORT.md).
