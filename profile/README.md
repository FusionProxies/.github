<div align="center">

<a href="https://fusionproxy.net/?utm_source=github&utm_medium=referral&utm_campaign=org-profile">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/FusionProxies/.github/main/assets/logo-on-dark.png">
    <img src="https://raw.githubusercontent.com/FusionProxies/.github/main/assets/logo-on-light.png" alt="Fusion Proxy" height="56">
  </picture>
</a>

### Residential, ISP and datacenter proxies for scraping, automation and multi-accounting

[![Website](https://img.shields.io/badge/Website-fusionproxy.net-1784f5?style=for-the-badge)](https://fusionproxy.net/?utm_source=github&utm_medium=referral&utm_campaign=org-profile)
[![Dashboard](https://img.shields.io/badge/Dashboard-Sign_up-14213d?style=for-the-badge)](https://dashboard.fusionproxy.net/#/register?utm_source=github&utm_medium=referral&utm_campaign=org-profile)
[![Guides](https://img.shields.io/badge/Guides-Setup_docs-2ea44f?style=for-the-badge)](https://fusionproxy.net/guides?utm_source=github&utm_medium=referral&utm_campaign=org-profile)
[![Free tools](https://img.shields.io/badge/Free_tools-Proxy_checker-8a63d2?style=for-the-badge)](https://fusionproxy.net/tools?utm_source=github&utm_medium=referral&utm_campaign=org-profile)

</div>

---

## Products

| Product | What you get | Price |
|---|---|---|
| **[Residential](https://fusionproxy.net/proxies/residential?utm_source=github&utm_medium=referral&utm_campaign=org-profile)** | Rotating or sticky sessions (1 to 120 min), country, state and city targeting, HTTP(S) and SOCKS5, traffic that never expires | $2.95/GB, down to $0.65/GB at 10,000 GB |
| **[Unlimited residential](https://fusionproxy.net/proxies/unlimited-residential?utm_source=github&utm_medium=referral&utm_campaign=org-profile)** | Unlimited traffic, priced by bandwidth | from $39.99 per week (5 Mbps) |
| **[Static ISP](https://fusionproxy.net/proxies/isp?utm_source=github&utm_medium=referral&utm_campaign=org-profile)** | Dedicated static ISP IP, unlimited bandwidth | $10.80 per IP for 30 days |
| **[Dedicated datacenter](https://fusionproxy.net/proxies/datacenter?utm_source=github&utm_medium=referral&utm_campaign=org-profile)** | Dedicated static IP, unlimited bandwidth | $2.60 per IP for 30 days |

Pay by card or crypto (crypto top-ups get a 3% bonus). Prices: [fusionproxy.net/pricing](https://fusionproxy.net/pricing?utm_source=github&utm_medium=referral&utm_campaign=org-profile).

## Quick start

```bash
# rotating residential IP in the United States
curl -x http://resi.fusionproxy.net:12286 -U "USERNAME-country-us:PASSWORD" https://ipinfo.io/json

# same IP for 10 minutes (sticky session)
curl -x http://resi.fusionproxy.net:12286 -U "USERNAME-country-us-sessid-4821937-sessTime-600s:PASSWORD" https://ipinfo.io/json
```

Your username and password are in the [dashboard](https://dashboard.fusionproxy.net/?utm_source=github&utm_medium=referral&utm_campaign=org-profile). The [endpoint generator guide](https://fusionproxy.net/guides/endpoint-generator?utm_source=github&utm_medium=referral&utm_campaign=org-profile) explains every option.

## Free tools

| Repository | What it does |
|---|---|
| [proxy-checker](https://github.com/FusionProxies/proxy-checker) | Fast command-line proxy checker: speed, exit IP, country and network for thousands of proxies |
| [fusionproxy-mcp](https://github.com/FusionProxies/fusionproxy-mcp) | MCP server that lets Claude, Cursor and VS Code fetch pages through residential IPs in any country |
| [scrapy-proxy-middleware](https://github.com/FusionProxies/scrapy-proxy-middleware) | Scrapy middleware: country targeting, sticky IP per site, new IP on 403/429 blocks |
| [free-proxy-list](https://github.com/FusionProxies/free-proxy-list) | Public HTTP, SOCKS4 and SOCKS5 proxies from five lists, merged every 30 minutes, as TXT, JSON and CSV |
| [proxy-anonymity-test](https://github.com/FusionProxies/proxy-anonymity-test) | Find out whether a proxy is transparent, anonymous or elite |

```bash
go install github.com/FusionProxies/proxy-checker@latest      # or a binary from the Releases page
pip install git+https://github.com/FusionProxies/scrapy-proxy-middleware
claude mcp add fusionproxy -e FUSION_USER=... -e FUSION_PASS=...   -- uvx --from git+https://github.com/FusionProxies/fusionproxy-mcp fusionproxy-mcp
```

All repositories are MIT licensed.

## Integrations

| Repository | What is inside |
|---|---|
| [fusionproxy](https://github.com/FusionProxies/fusionproxy) | Endpoints, username options and working examples in cURL, Python, Node.js, Go, PHP, Java, C# and Ruby |
| [playwright-proxy](https://github.com/FusionProxies/playwright-proxy) | Playwright (Python and Node.js) with authenticated proxies and one IP per browser context |
| [puppeteer-proxy](https://github.com/FusionProxies/puppeteer-proxy) | Puppeteer with authenticated proxies and one IP per browser context |
| [selenium-proxy](https://github.com/FusionProxies/selenium-proxy) | Selenium proxy authentication for Chrome and Firefox, headless included |

## Tutorials

| Repository | Topic |
|---|---|
| [python-requests-proxy](https://github.com/FusionProxies/python-requests-proxy) | How to use a proxy with Python requests |
| [python-requests-retry](https://github.com/FusionProxies/python-requests-retry) | How to retry failed requests, with backoff and a new IP after blocks |
| [nodejs-proxy](https://github.com/FusionProxies/nodejs-proxy) | How to use a proxy in Node.js: fetch, axios, SOCKS5 |
| [curl-proxy](https://github.com/FusionProxies/curl-proxy) | How to use a proxy with cURL |
| [proxy-cheatsheet](https://github.com/FusionProxies/proxy-cheatsheet) | Proxy settings for git, npm, pip, Docker, apt, SSH, Windows, macOS and more |
| [python-async-scraping](https://github.com/FusionProxies/python-async-scraping) | Async web scraping with asyncio, httpx and aiohttp |
| [rotating-proxies-python](https://github.com/FusionProxies/rotating-proxies-python) | Rotating proxies in Python: a proxy rotator and rotating gateways |
| [user-agent-rotation-python](https://github.com/FusionProxies/user-agent-rotation-python) | User-Agent rotation done right |
| [scrape-sitemap-python](https://github.com/FusionProxies/scrape-sitemap-python) | Get every URL of a website from its sitemap |
| [scrape-html-tables-python](https://github.com/FusionProxies/scrape-html-tables-python) | Scrape HTML tables with pandas and BeautifulSoup |
| [python-download-images](https://github.com/FusionProxies/python-download-images) | Download images from a website with Python |
| [python-web-scraping](https://github.com/FusionProxies/python-web-scraping) | Web scraping with Python: requests and BeautifulSoup |
| [nodejs-web-scraping](https://github.com/FusionProxies/nodejs-web-scraping) | Web scraping with Node.js: axios and cheerio |
| [golang-web-scraping](https://github.com/FusionProxies/golang-web-scraping) | Web scraping with Go and Colly |
| [scrape-infinite-scroll](https://github.com/FusionProxies/scrape-infinite-scroll) | How to scrape infinite scroll pages |
| [scrape-javascript-website](https://github.com/FusionProxies/scrape-javascript-website) | How to scrape JavaScript-rendered websites, often without a browser |
| [scrape-website-with-login](https://github.com/FusionProxies/scrape-website-with-login) | How to scrape a website that requires a login |

## Links

[Pricing](https://fusionproxy.net/pricing?utm_source=github&utm_medium=referral&utm_campaign=org-profile) ·
[Free trial](https://fusionproxy.net/free-trial?utm_source=github&utm_medium=referral&utm_campaign=org-profile) ·
[Guides](https://fusionproxy.net/guides?utm_source=github&utm_medium=referral&utm_campaign=org-profile) ·
[Proxy checker](https://fusionproxy.net/tools/proxy-checker?utm_source=github&utm_medium=referral&utm_campaign=org-profile) ·
[What is my IP](https://fusionproxy.net/tools/my-ip?utm_source=github&utm_medium=referral&utm_campaign=org-profile) ·
[Contact](https://fusionproxy.net/contact?utm_source=github&utm_medium=referral&utm_campaign=org-profile)
