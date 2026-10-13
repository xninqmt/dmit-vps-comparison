# dmit vps: Pro, Eyeball and Tier 1 compared, with full plan prices and how to pick without overpaying

Open DMIT's product page for the first time and you'll see three network profiles, three regions, plan names like WEE, TINY, Pocket, MALIBU and CORONA, and prices running from $6.90 a month to $839. There's no obvious logic to the naming, and the cheapest and most expensive plans sit on the same page.

The plan names aren't what you're choosing between. The network profile is. Everything else on that page — CPU, RAM, disk — is secondary to a decision you make in the first two seconds, and it's the one most people get wrong.

One warning before the tables: DMIT's catalogue rotates constantly. Plans sell out and come back, and the hardware platform behind a plan name changes (AS3 → AN4 → AN5) with prices attached to the platform rather than the specs. The figures below are drawn from the most recent listings I could find; treat any specific price as indicative and the live product page as authoritative.

## The three network profiles, and what actually changes

DMIT sells the same box three ways depending on where you are and how much you care about routing.

**Premium (Pro)** is the top tier. China Telecom traffic goes out over CN2 GIA (AS4809), China Unicom connects directly over AS4837, China Mobile enters through Hong Kong Mobile (AS58453), and all three carriers come back on CN2 GIA. In plain terms: an expensive, lightly loaded path into mainland China that holds up at 9pm.

**Eyeball (EB)** is the middle tier. Traffic is distributed between AS9929 and AS58807 depending on carrier — China Mobile lands on CMIN2, Unicom mostly on AS9929. Not the absolute top routing, but the same hardware and a noticeably bigger traffic allowance.

**Tier 1 (T1)** has no China optimisation at all. It's plain international routing aimed at Asia–US and US domestic latency. It's also where the bargain plans live.

The practical consequence is worth spelling out, because it's the single most useful thing on this page. At almost every price point, Premium and Eyeball cost the same and Eyeball gives you roughly double the monthly traffic and double the port speed:

| Price | Premium (Pro) traffic / port | Eyeball (EB) traffic / port |
| --- | --- | --- |
| $10.90/mo | 1 TB @ 1 Gbps | 1.5 TB @ 2 Gbps |
| $16.90/mo | 1.5 TB @ 4 Gbps | 3 TB @ 4 Gbps |
| $34.90/mo | 3 TB @ 10 Gbps | 5 TB @ 10 Gbps |
| $62.90/mo | 5 TB @ 10 Gbps | 10 TB @ 10 Gbps |
| $87.90/mo | 7 TB @ 10 Gbps | 14 TB @ 10 Gbps |
| $199.90/mo | 14 TB @ 10 Gbps | 30 TB @ 10 Gbps |

So "Premium" isn't buying you a better machine, it's buying you a better route and less traffic. If you're on China Mobile and your workload is downloads or streaming, Eyeball at the same price is usually the smarter buy. If your users are on China Telecom and you're running something latency-sensitive, that's the case where the CN2 GIA premium earns its keep.

## The platform problem: why two identical-looking plans have different prices

Since early 2026, DMIT has been reshuffling its Los Angeles hardware, and this is why you'll find the same plan name at two prices.

The company announced in March 2026 that rising hardware costs had made the AN5 (Next) platform unprofitable to sell, so it was pulled, with AN4 Pro/EB brought in as a stopgap and AS3 (LTS) designated the long-term, higher-volume platform. AN5 then returned in April 2026 at higher prices — the entry Pro plan moved from roughly $10.90 to $12.98 a month, and the two cheapest configs lost the monthly billing option entirely, requiring quarterly payment. Older AN4 stock has largely disappeared from the site.

What that means in practice: **AS3 (AMD EPYC 7003) is the value tier, and AN5 (AMD EPYC 9005 / Turin, with DDR5) is the premium hardware tier at roughly 20–25% higher prices.** DMIT also stated that existing subscribers' renewal prices wouldn't change — only new purchases and upgrades move to the new pricing.

## DMIT Los Angeles plans and prices

Los Angeles is the flagship location and where the value sits. Current AS3-platform pricing:

### LAX.AS3 — Premium and Eyeball (optimised for mainland China)

| Plan | vCPU | RAM | SSD | Traffic | Port | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| LAX.AS3.Pro.TINY | 1 | 2 GB | 20 GB | 1 TB | 1 Gbps | $10.90/mo | [ Check this plan](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.Pocket | 2 | 2 GB | 40 GB | 1.5 TB | 4 Gbps | $16.90/mo | [ See Pocket pricing](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.STARTER | 2 | 2 GB | 80 GB | 3 TB | 10 Gbps | $34.90/mo | [ View STARTER](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MINI | 4 | 4 GB | 80 GB | 5 TB | 10 Gbps | $62.90/mo | [ Check stock](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MICRO | 4 | 4 GB | 160 GB | 7 TB | 10 Gbps | $87.90/mo | [ See MICRO specs](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MEDIUM | 6 | 8 GB | 160 GB | 14 TB | 10 Gbps | $199.90/mo | [ Check availability](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.TINY | 1 | 2 GB | 20 GB | 1.5 TB | 2 Gbps | $10.90/mo | [ See Eyeball TINY](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.Pocket | 2 | 2 GB | 40 GB | 3 TB | 4 Gbps | $16.90/mo | [ Check Eyeball Pocket](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.STARTER | 2 | 2 GB | 80 GB | 5 TB | 10 Gbps | $34.90/mo | [ View Eyeball STARTER](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MINI | 4 | 4 GB | 80 GB | 10 TB | 10 Gbps | $62.90/mo | [ See Eyeball MINI](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MICRO | 4 | 4 GB | 160 GB | 14 TB | 10 Gbps | $87.90/mo | [ Check Eyeball MICRO](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MEDIUM | 6 | 8 GB | 160 GB | 30 TB | 10 Gbps | $199.90/mo | [ See Eyeball MEDIUM](https://www.dmit.io/aff.php?aff=12046) |

All plans include 1 IPv4 plus 1 IPv6 /64, KVM virtualisation, and standard DDoS protection. Traffic over the quota doesn't cut you off — it throttles to 4 Mbps on the cheaper plans and 8–10 Mbps on the larger ones, which is enough for SSH and monitoring but not much else.

### LAX.AS3 Tier 1 (international routing, no China optimisation)

| Plan | vCPU | RAM | SSD | Traffic | Port | Over-quota | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LAX.AS3.T1.WEE | 1 | 1 GB | 20 GB | 1 TB | 4 Gbps | 100 Mbps unlimited | $36.90/year | [ Lowest entry price](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.TINY | 1 | 1 GB | 20 GB | 2 TB | 4 Gbps | 200 Mbps unlimited | $6.90/mo | [ Check T1 TINY](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.STARTER | 2 | 2 GB | 40 GB | 4 TB | 10 Gbps | 200 Mbps unlimited | $12.90/mo | [ See T1 STARTER](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.MINI | 2 | 4 GB | 80 GB | 8 TB | 10 Gbps | 200 Mbps unlimited | $21.90/mo | [ Check T1 MINI](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.MICRO | 4 | 4 GB | 120 GB | 16 TB | 10 Gbps | 500 Mbps unlimited | $32.90/mo | [ View T1 MICRO](https://www.dmit.io/aff.php?aff=12046) |

WEE works out to about $3.08 a month. That's the cheapest way into DMIT, and it's a legitimate deal if you can live with international routing.

### The AN5 hardware tier (same lines, newer silicon, higher prices)

| Plan | vCPU | RAM | SSD | Traffic | Port | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| LAX.AN5.Pro.TINY | 1 | 2 GB | 20 GB | 1 TB | 1 Gbps | $12.98/mo or $37.99/quarter | [ See AN5 Pro TINY](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.Pocket | 1 | 2 GB | 40 GB | 1.5 TB | 4 Gbps | $18.90/mo or $56.70/quarter | [ Check AN5 Pocket](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.STARTER | 2 | 2 GB | 80 GB | 3 TB | 10 Gbps | $38.90/mo | [ View AN5 STARTER](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.MINI | 4 | 4 GB | 80 GB | 5 TB | 10 Gbps | $76.90/mo | [ Check AN5 MINI](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.MICRO | 4 | 4 GB | 160 GB | 7 TB | 10 Gbps | $99.90/mo | [ See AN5 MICRO](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.MEDIUM | 6 | 8 GB | 160 GB | 14 TB | 10 Gbps | $219.90/mo | [ View AN5 MEDIUM](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.LARGE | 8 | 16 GB | 320 GB | 25 TB | 10 Gbps | $459.90/mo | [ Check AN5 LARGE](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.Pro.GIANT | 8 | 24 GB | 640 GB | 50 TB | 10 Gbps | $839.90/mo | [ See AN5 GIANT](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.EB.TINY | 1 | 2 GB | 20 GB | 1.5 TB | 2 Gbps | $12.98/mo | [ Check AN5 EB TINY](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.EB.Pocket | 2 | 2 GB | 40 GB | 3 TB | 4 Gbps | $18.90/mo | [ See AN5 EB Pocket](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.EB.STARTER | 2 | 2 GB | 80 GB | 5 TB | 10 Gbps | $38.90/mo | [ View AN5 EB STARTER](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.EB.MINI | 4 | 4 GB | 80 GB | 10 TB | 10 Gbps | $76.90/mo | [ Check AN5 EB MINI](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AN5.EB.MICRO | 4 | 4 GB | 160 GB | 14 TB | 10 Gbps | $99.90/mo | [ See AN5 EB MICRO](https://www.dmit.io/aff.php?aff=12046) |

The AN5 Tier 1 line has been restructured into two sub-series: VOLUME, which trades CPU for traffic and starts around $14.90 a month, and GENERAL, which leans toward memory and starts around $16.90. Both use the same international routing as AS3 Tier 1.

Paying the AN5 premium buys you newer silicon and DDR5. For a WordPress site or a proxy node, that extra CPU is mostly idle. Worth it if you're compiling, transcoding, or running something genuinely CPU-bound.

## DMIT Hong Kong plans and prices

Hong Kong is the low-latency option for mainland China — roughly 40–50 ms versus 150 ms and up from Los Angeles. It's priced accordingly.

### Hong Kong Premium (three-network CN2 GIA)

| Plan | vCPU | RAM | SSD | Traffic | Port | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| HKG.Pro.TINY | 1 | 1 GB | 20 GB | 500 GB | 1 Gbps | $39.90/mo | [ Check HKG Pro TINY](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.STARTER | 1 | 2 GB | 40 GB | 1 TB | 1 Gbps | $79.90/mo | [ See HKG Pro STARTER](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MINI | 2 | 2 GB | 60 GB | 1.5 TB | 1 Gbps | $126.90/mo | [ View HKG Pro MINI](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MICRO | 2 | 4 GB | 80 GB | 2 TB | 1 Gbps | $179.90/mo | [ Check HKG Pro MICRO](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MEDIUM | 4 | 4 GB | 160 GB | 2.5 TB | 1 Gbps | $239.90/mo | [ See HKG Pro MEDIUM](https://www.dmit.io/aff.php?aff=12046) |

Note that Hong Kong prices rise in bands rather than smoothly — doubling from TINY to STARTER costs you more than the specs suggest, because you're buying port and traffic on scarce Hong Kong capacity. The same Premium line has appeared over the past year with different specs and prices depending on whether the underlying hardware was AS3 or AN5, so verify before ordering.

### Hong Kong Tier 1 (international BGP)

| Plan | vCPU | RAM | SSD | Traffic | Port | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| HKG.T1.WEE | 1 | 1 GB | 20 GB | 1 TB | 4 Gbps | $36.90/year | [ Cheapest HK entry](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.TINY | 1 | 1 GB | 20 GB | 2 TB | 4 Gbps | $6.90/mo | [ Check HK T1 TINY](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.STARTER | 1 | 2 GB | 40 GB | 4 TB | 10 Gbps | $12.90/mo | [ See HK T1 STARTER](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MINI | 2 | 2 GB | 60 GB | 8 TB | 10 Gbps | $21.90/mo | [ View HK T1 MINI](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MICRO | 4 | 4 GB | 80 GB | 16 TB | 10 Gbps | $32.90/mo | [ Check HK T1 MICRO](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MEDIUM | 4 | 8 GB | 160 GB | 32 TB | 10 Gbps | $49.90/mo | [ See HK T1 MEDIUM](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.LARGE | 8 | 16 GB | 320 GB | 64 TB | 10 Gbps | $99.90/mo | [ View HK T1 LARGE](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.GIANT | 8 | 24 GB | 640 GB | 128 TB | 10 Gbps | $199.90/mo | [ Check HK T1 GIANT](https://www.dmit.io/aff.php?aff=12046) |

The Tier 1 traffic allowances here are enormous — 128 TB on the top plan — and over-quota traffic throttles to somewhere between 50 Mbps and 1 Gbps rather than stopping. The catch is real, though: no China optimisation means China Telecom users can end up with worse latency than a well-routed US box. If you're on Telecom and buying Hong Kong specifically for the low ping, Tier 1 will disappoint you.

## DMIT Tokyo plans and prices

Tokyo sits between the two on latency, with Premium routing typically landing in the 50–90 ms range from mainland China. Stock is the tightest of the three regions, and the Tokyo Eyeball line has been pulled from sale at times.

| Plan | vCPU | RAM | SSD | Traffic | Port | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| TYO.Pro.TINY | 1 | 1 GB | 20 GB | 500 GB | 1 Gbps | $21.90/mo | [ Check Tokyo Pro TINY](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.STARTER | 1 | 2 GB | 40 GB | 1 TB | 1 Gbps | $39.90/mo | [ See Tokyo Pro STARTER](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MINI | 2 | 2 GB | 60 GB | 2 TB | 1 Gbps | $79.90/mo | [ View Tokyo Pro MINI](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MICRO | 4 | 4 GB | 80 GB | 4 TB | 1 Gbps | $159.90/mo | [ Check Tokyo Pro MICRO](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MEDIUM | 4 | 8 GB | 160 GB | 5 TB | 1 Gbps | $259.90/mo | [ See Tokyo Pro MEDIUM](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.LARGE | 8 | 16 GB | 320 GB | 8 TB | 1 Gbps | $429.90/mo | [ View Tokyo Pro LARGE](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.GIANT | 8 | 24 GB | 640 GB | 15 TB | 1 Gbps | $799.90/mo | [ Check Tokyo Pro GIANT](https://www.dmit.io/aff.php?aff=12046) |

One thing to watch: DMIT's Tokyo Premium listings state that traffic overage pauses the instance rather than throttling it. If you buy Tokyo Pro, size the traffic allowance with real headroom, because hitting the cap means downtime until the next reset. Tier 1 in Tokyo starts at $36.90 a year and throttles instead of pausing.

## Coupon codes: rare, and specific about billing cycles

DMIT doesn't run the constant half-off promotions that cheaper hosts do. Codes come and go, they're usually tied to one product line and one billing cycle, and they need to be validated at checkout. These are the ones that have appeared repeatedly across multiple sources:

| Code | Applies to | Discount |
| --- | --- | --- |
| LAX-EB-LAUNCH-NON-MONTHLY-RECURRING-20OFF | Los Angeles Eyeball, non-monthly cycles | 20% recurring |
| 202510_HKG_TYO_PRO_20OFF_RECURRING | Hong Kong / Tokyo Premium, quarterly or longer | 20% recurring |
| 202510_HKG_TYO_T1_30OFF_RECURRING | Hong Kong / Tokyo Tier 1, quarterly or longer (excludes WEE) | 30% recurring |
| Lite-Annually-Recur-30OFF | Lite / Standard network plans, annual | 30% |
| Lite-Semi-Annually-Recur-20OFF | Lite / Standard network plans, semi-annual | 20% |

"Recurring" matters. Those discounts apply on renewals too, not just the first invoice, which changes the maths considerably over two or three years. Punch the code into the cart and hit Validate before you assume anything — an expired code fails silently otherwise.

## Billing cycle, and why month-to-month is the expensive option

Longer cycles carry a built-in discount that stacks on top of any coupon, and on the cheapest Los Angeles and Hong Kong configs the monthly price is higher than the annual equivalent by a wide margin. Tier 1 WEE at $36.90 a year is the clearest example, but the pattern holds across the range.

The counterargument is that DMIT's stock rotates, so a plan you like today may not exist at renewal. That cuts both ways: it also means you can't always re-buy a plan you gave up. If a config you want is listed and in stock, buying a longer cycle locks in both the price and the spec.

DMIT has also run time-limited promotions offering extra traffic (around 1.3x) on semi-annual and annual orders, plus account credit back on top of a discount during holiday sales. These don't appear on any schedule, so if you see one advertised, it's worth checking whether it applies to your cart before paying.

## What buying actually involves (and the one thing that trips up first-timers)

Register an account, pick region and line, choose a plan, apply the coupon, pay. Alipay, PayPal and credit cards are all accepted, and support is available in Chinese as well as English.

The step people get stuck on: **DMIT disables root password login by default.** You're expected to connect with an SSH key, which means uploading or generating a public key during or right after purchase. If you've only ever logged into a VPS with a password, this will look like a broken server. It isn't. You can set a root password from the console tab in the instance control panel and then log in through the web console if you need to, but the SSH key route is what the platform is built around.

Buyers' write-ups also recommend signing up without a proxy and with accurate details, since the signup flow has risk checks and a flagged order can be refunded automatically. That's a five-minute annoyance compared to sorting it out afterwards.

## Overages, IP replacement, upgrades and refunds

A few policy details that are worth knowing before you commit:

- **Traffic overage.** DMIT uses three different strategies depending on the plan: pause the instance, throttle the port, or leave it unlimited. Tier 1 plans generally throttle to a still-usable 100–500 Mbps. Tokyo Premium pauses. Check which applies to the plan you're buying.
- **Paid traffic resets.** Most regular plans let you reset your traffic quota mid-cycle for a fee equal to your renewal price divided by the billing cycle. Only some sPro-series plans support permanently adding traffic.
- **IP replacement.** Blocked IPs can be swapped, with free replacements available on a rolling basis (roughly every 15 days) and paid replacements otherwise around $5. The exact rules differ between the Pro/EB and Tier 1 lines, and IP-blocked instances aren't refundable.
- **Upgrades.** You can move up within the same series, to a plan that's currently in stock, and only if the new disk isn't smaller. Downgrades aren't supported. The upgrade fee is the full difference between the two plans' totals, and unused time on your current plan doesn't reduce it — so timing matters.
- **Refunds.** The stated policy is a full refund within 3 days if you've used under 30 GB, and a pro-rated partial refund within 30 days, minus payment gateway fees. Renewals, balance payments, and cases where you've already refunded the same series multiple times are excluded. Confirm the current terms on their policy page before ordering, because this is exactly the kind of thing that changes.

## Who should actually buy this

If your audience, team or customers are entirely outside Asia, DMIT is the wrong tool. You'd be paying for CN2 GIA routing and Hong Kong port capacity that your traffic never touches. A Tier 1 plan would be the only defensible choice there, and even then you're paying a routing premium for nothing.

The case for DMIT is narrow and specific: users in mainland China who notice the difference between a route that holds up at 9pm and one that doesn't. Within that, the decision is mostly mechanical.

- **Cheapest way in, international users only:** Los Angeles or Hong Kong Tier 1 WEE at $36.90/year.
- **China Mobile, streaming or heavy downloads:** LAX Eyeball. Same price as Premium, double the traffic.
- **China Telecom, latency-sensitive, business traffic:** LAX or HKG Premium. That's what CN2 GIA is for.
- **Sub-50 ms to mainland China:** Hong Kong Premium. Budget for it.
- **Asia-Pacific with the lowest latency available:** Tokyo Premium, but watch the overage policy and stock.

Two things DMIT is consistently credited with across the reviews I read: it doesn't oversell, so your allocated resources hold up under load, and support tickets get answered with compensation offered when something goes wrong. That's the reason people keep renewing at these prices rather than moving to a $2-a-month box. Whether that's worth 5x the cost depends entirely on whether bad evenings cost you money.

## FAQ

**Is DMIT worth it compared to a cheap VPS?** Only if China-optimised routing is a real requirement. For a hobby box or a site with international users, you're paying for a feature you won't use.

**What's the difference between Pro and EB?** Pro routes all three Chinese carriers over CN2 GIA. EB uses CMIN2 and AS9929, which is excellent for China Mobile and good for Unicom. At the same price, EB gives roughly double the traffic and double the port speed.

**Can I get Windows?** Not natively. Linux images are provided; Windows requires uploading your own ISO, which is more trouble than it's worth for most people.

**What happens if my IP gets blocked?** DMIT replaces blocked IPs, with free replacements available periodically and paid ones around $5. It isn't grounds for a refund, so test with a trial deployment before moving anything important.

**Do the prices in this article still apply?** Treat them as the most recent listings rather than a guarantee. DMIT changes platforms, adjusts prices and sells out regularly — the product page is the only place where the number you're actually going to pay is confirmed.

[👉 Check current DMIT plans, stock and pricing](https://www.dmit.io/aff.php?aff=12046)
