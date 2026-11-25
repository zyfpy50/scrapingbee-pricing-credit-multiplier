# ScrapingBee Pricing: What Each Plan Costs, What 1,000 Pages Really Cost, and When the Credit Multiplier Stops Working in Your Favor (Full Plan Table)

ScrapingBee's standard plans cost **$19, $49, $99, $249 and $599 a month** for 75,000, 250,000, 1 million, 3 million and 8 million API credits. Billing is monthly only, prices exclude VAT, and there is no free plan; new accounts get 1,000 credits once, no card required. What the plan card does not show is the credit multiplier. JavaScript rendering is on by default, so an ordinary request costs 5 credits, and a stealth request costs 75. That puts the real price anywhere from about **$0.07 to $19 per 1,000 pages** on those same five plans.

Below is every tier with its converted per-page cost, the billing terms that decide what you actually pay at month end, and the workloads where a per-domain API such as ScraperAPI fits better than a credit multiplier.

> Most buyers comparing ScrapingBee pricing should start at Hobby or Freelance. Startup only makes sense once your monthly credit burn is above roughly 250,000. If most of your pages need a headless browser, budget at the 5-credit line: Freelance's 250,000 credits fetch about 50,000 rendered pages, not 250,000. If your volume swings month to month or you want a free allowance that renews, ScraperAPI's Hobby is $49 for 100,000 credits with a permanent 1,000-credit free tier and 10% off annual billing.
>
> 👉 [See ScraperAPI's plan prices and free tier](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## ScrapingBee plans: the full list

| Plan | Monthly price | API credits | Concurrent requests |
| --- | --- | --- | --- |
| Hobby | $19 | 75,000 | 25 |
| Freelance | $49 | 250,000 | 50 |
| Startup (marked Recommended) | $99 | 1,000,000 | 100 |
| Business | $249 | 3,000,000 | 200 |
| Business + | $599 | 8,000,000 | 400 |

Priority email support, a dedicated account manager and team management start at Business. Hobby, Freelance and Startup ship the same scraping features (rendering, rotating and premium proxies, geotargeting, screenshots, extraction rules, the dedicated Google/Amazon/Walmart/YouTube endpoints) without the account-management layer.

Above Business + the tiers are self-serve too, not sales-gated: **$999 / $1,599 / $2,399** for 14M / 24M / 41M credits at 500 / 600 / 700 concurrent requests, and **$3,599 / $5,799** for 69M / 120M credits at 800 / 900. The top of the range is $5,799 a month, and no tier requires a call.

Two things to ignore while you shop. Older reviews and cached help pages still quote $49.99, $99.99 and concurrency of 10 or 50, which was the lineup before Hobby existed. The live pricing page is the source, and it starts at $19.

## What a page actually costs on each plan

ScrapingBee sells credits, not pages, and the conversion depends on two switches: whether the page needs a browser and which proxy tier gets through.

| Request type | Credits per page |
| --- | --- |
| Classic proxy, JavaScript off | 1 |
| Classic proxy, JavaScript on (the default) | 5 |
| Premium proxy, JavaScript off | 10 |
| Premium proxy with rendering | 25 |
| Stealth proxy | 75 |
| Google URL, classic or premium | about 15 (documentation gives a 10 to 15 range) |
| AI extraction add-on | +5 |

Convert those credits at the plan's per-credit rate and the same $99 plan spans a factor of 74:

| Plan | 1 credit (static) | 5 credits (default render) | 25 credits (premium + render) | 75 credits (stealth) |
| --- | --- | --- | --- | --- |
| Hobby $19 | $0.25 | $1.27 | $6.33 | $19.00 |
| Freelance $49 | $0.20 | $0.98 | $4.90 | $14.70 |
| Startup $99 | $0.10 | $0.50 | $2.48 | $7.43 |
| Business $249 | $0.08 | $0.42 | $2.08 | $6.23 |
| Business + $599 | $0.07 | $0.37 | $1.87 | $5.62 |

Figures are dollars per 1,000 pages, converted from ScrapingBee's published plan prices (checked 12 November 2026) and its credit documentation.

Read it in pages instead and the gap gets harder to ignore. Hobby's 75,000 credits buy 75,000 static pages, 15,000 rendered pages, 3,000 premium rendered pages or 1,000 stealth pages. The 1,000 free credits you get at signup buy about 13 stealth pages, which is enough to find out whether stealth works on one target and not much else.

For a typical commercial job, the honest planning number is 5 credits a page, because most retail, travel and listing sites built in the last few years return empty HTML without a browser. If even one site in five needs premium proxies, your blended average climbs well past 5.

## The billing terms that decide your month

These are the parts of ScrapingBee's terms that change what you pay, and they rarely appear in reviews.

**Credits expire at the end of each cycle.** Nothing rolls over, and there is no pay-as-you-go. Run out mid-month and your requests stall until renewal unless you upgrade the plan for that month, buy a one-time add-on whose price is not published, or renew early at full price and forfeit the remaining balance.

**Payments are non-refundable.** The only exception in the terms is a pro-rata refund for a defect you reported that ScrapingBee did not fix. "Cancel anytime" on the pricing page refers to stopping future renewals, not to getting a month back.

**404 and 410 responses are billed.** Failed requests cost nothing in general, and Auto Mode, added in July 2026, only charges the setting that eventually succeeded. But a page that returns 404 counts as a successful request, which matters if you crawl large site inventories where a slice of URLs is always dead.

**The trial cannot be extended by opening a second account.** That is spelled out in the terms. The 1,000 credits are once per customer.

**Prices exclude VAT**, so a European buyer on Hobby pays more than $19 at checkout.

## When ScrapingBee is the wrong buy

The multiplier model is fine when your target list is stable. It gets expensive in four situations.

**Your volume swings.** A quiet month wastes credits you paid for, and a busy month either stalls or forces an upgrade you did not plan. ScrapingBee has no overage billing and no carryover, so the plan becomes a ceiling rather than a budget.

**You want an annual commitment.** There is no yearly option at any tier, so there is no discount to negotiate and no way to lock a rate.

**Most of your pages sit behind serious bot protection.** Stealth is 75 credits a page, which is $7.43 per 1,000 on Startup and $19 per 1,000 on Hobby. At 50,000 stealth pages a month, Startup's million credits cover 13,300 pages, not 50,000.

**You need a per-URL cost estimate before the request runs.** ScrapingBee's dashboard shows the cost of a request, and Auto Mode tries the cheapest setting first, which helps at the margin. It does not let you publish a fixed rate card for a domain or hard-cap a single request.

ScraperAPI approaches the same job from a different direction: it prices per target domain rather than per proxy tier, renews 1,000 free credits every month, offers 10% off annual billing, and adds pay-as-you-go on Scaling and above so an unusual month does not stop a pipeline.

👉 [Check ScraperAPI's free tier and per-domain credit rates](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## ScraperAPI's plans, priced the same way

| Plan | Monthly price | API credits | Concurrent threads | Get started |
| --- | --- | --- | --- | --- |
| Free | $0 | 1,000 / month | 5 | [Free plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Hobby | $49 | 100,000 | 20 | [Hobby](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Startup | $149 | 1,000,000 | 50 | [Startup](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Business | $299 | 3,000,000 | 100 | [Business](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Scaling | $475 | 5,000,000 | 200 | [Scaling](https://www.scraperapi.com/pricing/?fp_ref=coupons) |

New accounts also get a 7-day trial with 5,000 credits, no card. Above Scaling, ScraperAPI lists Professional (10.5M credits, 300 threads), Advanced (21.5M credits, 500 threads) and Enterprise (22M+ credits, 500+ threads), quoted per account rather than at a flat posted rate; the live pricing page carries the current numbers. Annual billing takes 10% off, which puts Hobby at $44.10 a month across the year.

Credit costs depend on the target, not on which plan you are on:

| Target or feature | Credits per request |
| --- | --- |
| Standard page | 1 |
| Amazon, Walmart, eBay | 5 |
| Google or Bing, including subdomains | 25 |
| LinkedIn | 30 |
| Bot-protection bypass (Cloudflare, DataDome, PerimeterX, Akamai) | +10 on the base cost |
| JavaScript rendering (`render=true`) | 10 |
| Premium proxies | 10 |
| Premium proxies with rendering | 25 |
| Ultra premium | 30 (75 with rendering) |
| Screenshot | 10 |

Run those through the plan prices and Hobby ($49 per 100,000 credits) works out to **$0.49 per 1,000 standard pages and $4.90 per 1,000 rendered pages**. On Startup ($149 per 1M) the same pages cost $0.15 and $1.49. Fields such as geotargeting, sessions, device type and auto-parsing add nothing.

On raw credit volume, ScrapingBee is the cheaper buy at the entry level: $49 there buys 250,000 credits against ScraperAPI's 100,000, and its rendering multiplier is 5 against 10 here. Converted to rendered pages, ScrapingBee's Startup plan undercuts ScraperAPI's Startup by roughly two thirds. Where ScraperAPI pulls ahead is the shape of the bill: a monthly free allowance that does not expire with a trial, 10% off for paying annually, overage billing instead of a hard stop, a published rate for each domain, a `max_cost` parameter that caps any single request, and a bypass surcharge of 10 credits rather than a 75-credit stealth tier for protected pages.

## Questions buyers ask

**Does ScrapingBee have a free plan?** No. There is a one-time 1,000-credit allowance for new accounts, no ongoing free tier, and the terms forbid extra accounts to stretch it.

**Why does a default request cost 5 credits?** JavaScript rendering is enabled by default, and running a page in a headless browser costs more compute than fetching raw HTML. Turn rendering off for sites that serve content in the HTML and you get 1 credit per page.

**What happens when credits run out?** Scraping pauses until the next cycle. You can upgrade for the month, renew early at full price, or buy a one-time add-on whose price is not listed publicly.

**Is ScrapingBee cheaper than ScraperAPI?** On credits and rendered pages at the entry level, yes, by a wide margin. On workloads that need a free tier, annual billing, overage billing or per-domain budget caps, the comparison flips.

## How to choose

Match the plan to your page mix rather than to your page count.

Static HTML at a steady 50,000 to 250,000 pages a month: ScrapingBee Hobby or Freelance, with rendering switched off wherever the site allows it.

Rendered pages under about 50,000 a month: ScrapingBee Freelance at $49 covers 250,000 credits, which is 50,000 rendered pages.

Hard anti-bot targets at volume, or a need to forecast spend by domain: ScraperAPI's per-domain rate card and `max_cost` cap do more for the budget than a cheaper credit does.

Volume that moves, or a team that wants to pay yearly: ScraperAPI, where 1,000 credits renew monthly, annual billing saves 10%, and pay-as-you-go on Scaling and above absorbs the spikes.

Before you pay either vendor, run 30 to 50 of your real URLs through the dashboard and read the credits-per-page number it reports. Then check what happens at the limit, because neither vendor carries unused credits forward and only one of them lets you keep scraping past the cap.

👉 [Compare ScraperAPI's plans and start with 5,000 trial credits](https://www.scraperapi.com/pricing/?fp_ref=coupons)
