# japan vps hosting: Tokyo plans from $79 a year, when CN2 GIA is actually worth it, and how to pick without overpaying

Most "japan vps hosting" searches come down to three questions: how much does a decent Tokyo server really cost, will the route to my users actually be good, and which plan is worth the money. BandwagonHost (known as 搬瓦工 in Chinese communities) answers the first one more aggressively than almost anyone: two limited-edition Tokyo plans at **$79 and $99 per year** on its DC39v2 datacenter, backed by a 30-day money-back guarantee that applies to all plans — and, unusually for the Japan market, applies even if the IP gets blocked by the GFW.

There are catches, and they matter: those two plans are limited-stock, locked to one datacenter, and carry CPU usage caps written into the official terms of service. The premium Tokyo CN2 GIA line starts at $89.99 *per month*. Picking wrong costs you either performance or a lot of money, so this guide walks through the current Japan lineup, the real routing differences, the restrictions most reviews skip, and a promo code that also works on renewals.

> **Quick pick:** For most people searching for a budget Japan VPS, **The Tokyo Plan v2 at $99/year** (2 AMD cores, 2GB RAM, 40GB SSD, 1TB traffic, 5Gbps) is the sensible choice — about $8.25/month, and community tests report stable daytime performance with only occasional evening packet loss. If your users are mainly on China Telecom and you can't tolerate peak-hour jitter, you need the CN2 GIA line instead, starting at $89.99/month. One caveat before clicking: limited plans sell out regularly, so check stock first. 👉 [Check The Tokyo Plan v2 availability and current price](https://bandwagonhost.com/aff.php?aff=74518&pid=163)

## Every Japan plan BandwagonHost currently sells

BandwagonHost splits its Japan inventory into three lines: limited-edition Tokyo plans (DC39v2, CMI direct routing), premium Tokyo CN2 GIA (JPTYO_8), and Osaka on the Softbank route. The limited plans first:

| Plan | CPU / RAM / Storage | Traffic | Bandwidth | Price | Buy |
| --- | --- | --- | --- | --- | --- |
| The Tokyo Plan (limited) | 1 core AMD / 1 GB / 20 GB SSD | 500 GB/mo | 2.5 Gbps | **$79/year** | [Order The Tokyo Plan](https://bandwagonhost.com/aff.php?aff=74518&pid=162) |
| The Tokyo Plan v2 (limited) | 2 cores AMD / 2 GB / 40 GB NVMe SSD | 1 TB/mo | 5 Gbps | **$99/year** | [Order The Tokyo Plan v2](https://bandwagonhost.com/aff.php?aff=74518&pid=163) |
| SakuraBox (limited) | 1 core AMD / 1 GB / 30 GB SSD | 500 GB/mo | 1 Gbps | $79/year | [Order SakuraBox](https://bandwagonhost.com/aff.php?aff=74518&pid=154) |

The CN2 GIA tiers, all in the JPTYO_8 datacenter housed in Equinix TY8:

| Plan | CPU | RAM | Storage | Monthly traffic | Price |
| --- | --- | --- | --- | --- | --- |
| Tokyo Starter | 2 cores | 2 GB | 40 GB SSD | 500 GB | $89.99/mo or $899.99/yr |
| Tokyo Pro | 4 cores | 2 GB | 80 GB SSD | 1 TB | $155.99/mo or $1,599.99/yr |
| Tokyo Plus | 6 cores | 8 GB | 160 GB SSD | 2 TB | $299.99/mo or $2,999.99/yr |
| Tokyo Business | 8 cores | 16 GB | 320 GB SSD | 4 TB | $589.99/mo or $5,899.99/yr |
| Tokyo Enterprise | 10 cores | 32 GB | 640 GB SSD | 6 TB | $989.99/mo or $9,989.99/yr |
| Tokyo Flagship | 12 cores | 64 GB | 1 TB SSD | 8 TB | $1,889.99/mo or $18,989.99/yr |

(Current plan listings for the CN2 GIA line vary slightly between BandwagonHost's own pages and third-party trackers on the mid-tier annual prices and port speeds, so treat the figures above as indicative and confirm the exact spec on the order page before paying.)

The Osaka side runs on Softbank routing and follows the same Starter-to-Flagship ladder, plus a limited edition:

| Plan | CPU / RAM / Storage | Traffic | Price | Buy |
| --- | --- | --- | --- | --- |
| Osaka Starter | 2 cores / 2 GB / 40 GB SSD | 500 GB/mo | $49.99/mo or $499.99/yr | [Order Osaka Starter](https://bit.ly/BandwaGon) |
| Osaka Pro | 4 cores / 2 GB / 80 GB SSD | 1 TB/mo | $86.99/mo or $869.99/yr | [Order Osaka Pro](https://bit.ly/BandwaGon) |
| Osaka Plus | 6 cores / 8 GB / 160 GB SSD | 2 TB/mo | $165.99/mo or $1,665.99/yr | [Order Osaka Plus](https://bit.ly/BandwaGon) |
| Osaka Business | 8 cores / 16 GB / 320 GB SSD | 4 TB/mo | $329.99/mo or $3,199.99/yr | [Order Osaka Business](https://bit.ly/BandwaGon) |
| Osaka Enterprise | 10 cores / 32 GB / 640 GB SSD | 6 TB/mo | $549.99/mo or $5,549.99/yr | [Order Osaka Enterprise](https://bit.ly/BandwaGon) |
| Osaka Flagship | 12 cores / 64 GB / 1 TB SSD | 8 TB/mo | $1,059.99/mo or $10,559.99/yr | [Order Osaka Flagship](https://bit.ly/BandwaGon) |
| OSAKA LIMITED EDITION 40G | 2 GB / 40 GB SSD | 2 TB/mo, 2.5 Gbps | $79.99/yr | [Order Osaka Limited](https://bit.ly/BandwaGon) |

Beyond Japan, the catalog includes US KVM plans from $49.99/year, CN2 GIA-E plans from $169.99/year with 15+ switchable datacenters, and Hong Kong CN2 GIA from $899.99/year — worth knowing if your needs turn out to be broader than a single Tokyo box. 👉 [Browse all BandwagonHost plans and current stock](https://bit.ly/BandwaGon)

One framing note before you compare prices with other providers: everything BandwagonHost sells is **self-managed KVM VPS** on its in-house KiwiVM panel, running on its own hardware and IP space. The company (IT7 Networks, operating since 2012) states openly that self-management is how it keeps prices down. There's no managed support tier — you're expected to handle Linux administration yourself, though AlmaLinux, RockyLinux, CentOS, Debian, Ubuntu, CentOS Stream and Fedora are one-click installs, and additional ISO images can be requested.

## The Tokyo Plan vs The Tokyo Plan v2: is the extra $20 worth it?

Yes, almost always. The v2 launched on July 21, 2025, and doubles every spec of the original (which launched June 15, 2025): 2 cores instead of 1, 2GB RAM instead of 1GB, 40GB NVMe RAID-10 instead of 20GB SSD, 1TB monthly traffic instead of 500GB, and 5Gbps bandwidth instead of 2.5Gbps. Twenty dollars a year for all of that is an easy call. BBR congestion control is enabled by default on these boxes, which helps cross-border throughput out of the box.

The original $79 plan still makes sense in one scenario: you need a Japan IP for something light — a proxy endpoint, a small API, a personal project — and even $8.25/month feels like more than the job deserves. Just respect the 1GB RAM ceiling if you're tempted to add a database.

Both plans sit in the **DC39v2** datacenter (node code JPTYO_39), which BandwagonHost upgraded with more diverse carriers compared to the older DC39. SakuraBox, the $79 plan from February 2025, still runs in the older DC39 at 1Gbps — same price, less bandwidth, 10GB more disk. If all three are in stock, The Tokyo Plan beats SakuraBox on the fundamentals.

Independent benchmarking of a DC39v2 unit returned numbers you don't normally see at this price: an AMD EPYC-Genoa at 2,445 MHz scoring **3,679 in single-core Sysbench**, 4K random I/O around 70k IOPS (with some samples reaching 137.9k), sequential reads past 9 GB/s, and Tokyo-local nodes exceeding 9 Gbps in both directions. On the network side, Speedtest.net showed 6,979 Mbps down, and a single-test sample to a China Telecom 5G connection in Suzhou measured **2,195 Mbps upload at 35.95ms** — most Japan VPS offers in this price range would struggle to break 100 Mbps on that same test.

Stock is the practical hurdle. Reports from April 2026 had both v2 plans out of stock, and limited plans restock irregularly in batches. The official restock tracker at stock.bwg.net and the Telegram channel @BandwagonHostNews announce restocks and list test IPs.

## The routing question: CMI direct vs CN2 GIA vs Softbank

This is where "japan vps hosting" searches usually go wrong, because a Tokyo datacenter label tells you almost nothing about the route. Tokyo is only about 1,800 km from Shanghai, but geography doesn't set your latency — routing and transit quality do.

**DC39v2 (The Tokyo Plan / v2):** return traffic runs primarily through China Mobile's CMI network. That makes **China Mobile users the clear winners** — eastern China commonly sees 40–55ms, and measured results included Shanghai Mobile at ~37ms and Beijing Mobile at ~40ms. Unicom lands in a 45–85ms band via AS4837. Telecom is the wildcard: Beijing measured roughly 68–109ms depending on the test, Shanghai threw out samples as high as 175ms, and some provinces route back over the ordinary Telecom 163 backbone rather than premium transit. Great for Mobile and Unicom, acceptable-but-variable for Telecom.

**Tokyo CN2 GIA (JPTYO_8):** the premium line, with China Telecom CN2 GIA, Unicom 9929 and Mobile CMI on the return path. Measured latencies: Telecom Shanghai ~35–40ms, Mobile ~36–50ms, Unicom ~67–87ms. A 2026 performance test of this facility recorded NVMe reads around 1,126 MB/s with roughly 1.2 Gbps sustained under real load. The practical difference from DC39v2 shows up at 7–11pm China time, exactly when the CMI-heavy line can jitter for Telecom users. If your workload involves financial applications, live streaming back to China, or anything where a peak-hour latency spike costs you money, this is what you're paying for — at roughly ten times the limited plans' price. 👉 [Compare Tokyo CN2 GIA options and pricing](https://bit.ly/BandwaGon)

**Osaka Softbank:** the Softbank route tends to be friendlier to certain China Telecom paths, and the Osaka Limited Edition gives you 2TB of monthly traffic at $79.99/year — the most generous traffic allowance in the budget tier. For projects serving Japan domestically, Southeast Asia, or mixed international traffic rather than China specifically, Osaka Starter at $499.99/year is the baseline most people should start from.

A quick self-check before ordering: BandwagonHost's official-looking looking-glass tools let you ping a candidate IP from multiple Chinese cities at once and read the packet loss per city. Under 1% off-peak and under 3% at peak is generally fine for most uses. It takes two minutes and tells you more about *your* route than any review can.

## The restrictions buried in the terms

These come straight from BandwagonHost's current terms of service, and none of them appear in the headline pricing.

**CPU usage caps, now confirmed in the official ToS.** The Tokyo Plan is capped at **30%** sustained single-core usage, the v2 at **45%**, with SakuraBox also at 30%. Exceeding the hourly average doesn't suspend the VPS — KiwiVM throttles CPU cycles to the plan level, displays a notice on the panel, and lifts it automatically once usage drops. But it rules out sustained heavy workloads: AI inference, video transcoding, continuous compilation. Websites, proxies, APIs and lightweight databases are fine. (SLA-covered plans have no such cap, but the Japan limited plans aren't among them, and only plans explicitly listing an SLA get uptime credits.)

**Storage I/O fair use.** The terms prohibit sustained disk I/O above 100 MiB/s for more than 4 hours at a stretch. You'll get an email warning first; continue anyway and the VPS can be temporarily suspended. Relevant if you're planning bulk file processing or backup staging on a budget plan.

**The acceptable-use list is longer than most.** BitTorrent (trackers, clients, files, even links), public open proxies, Tor relay or exit nodes, cryptocurrency mining and mining-adjacent compute, bulk or marketing email (only occasional transactional mail is allowed), IRC, port scanning, and nested virtualization beyond Docker are all explicitly banned. Plenty of "cheap Japan VPS" buyers implicitly assume a Tor exit node or a seedbox is fine — on this provider it's a grounds-for-suspension item.

**No migration, no managed help, no data guarantees.** Limited-edition plans are locked to DC39v2 permanently; the rest of the catalog supports free datacenter migration through KiwiVM without data loss, which is genuinely useful when A/B testing Tokyo vs Osaka routing. The service is unmanaged, and the terms state plainly that the company accepts no liability for data loss — backups are your job, and the ToS recommends verifying they actually restore.

## The promo code, the renewal lock, and a checkout flow that works

The code **BWHCGLUKKB** is BandwagonHost's standing discount — roughly 6.7% off, applies to all plans — and it works on **renewals**, not just first orders. Two more things stack in your favor here: limited Tokyo plans renew at the same annual price you paid, and per the provider's renewal policy, your price stays locked at your original purchase rate even if list prices rise later. On the $79 plan, the code brings the first year to roughly $73.65, and it stays there.

The checkout order matters more than people expect:

1. Open the order page through a plan link and select **annual billing** (annual beats monthly on essentially every plan in the catalog).
2. Enter `BWHCGLUKKB` in the **Promotional Code** field and confirm the discount actually displays before paying. If it doesn't show, stop and re-enter it.
3. Register, pick your OS, and pay — credit card, PayPal, Alipay and UnionPay are all accepted, which matters if the Japan providers you've compared so far only take international cards.
4. Boot the server from KiwiVM and grab your SSH credentials.

The 30-day money-back guarantee covers all plans, so a wrong first pick is recoverable — with the notable detail that The Tokyo Plan's listing states it's refundable within 30 days even if the IP has been blocked by the GFW. That removes the main risk of buying a China-oriented Japan VPS in the first place, since IP reputation is the one thing you can't predict from a spec sheet. 👉 [Open the BandwagonHost order page and check current stock](https://bit.ly/BandwaGon)

## How this stacks up against the rest of the Japan VPS market

Context helps, because $79/year reads as either cheap or expensive depending on what you've been comparing. The Tokyo KVM market currently splits into two shapes: European providers selling Tokyo locations on monthly billing — EDIS Global, for instance, sells Tokyo VPS and charges €5/month per extra IPv4 — and China-focused providers offering annual plans with optimized routes. On the refund side, the comparison is lopsided: one SoftBank-connected Tokyo provider (LuckVM) advertises only a 3-day satisfaction guarantee, while BandwagonHost gives you 30 days, GFW-blocked IPs included, to actually test routing from your own connection.

The counterweight is the CPU caps and the self-managed model. Providers charging monthly rates don't throttle your single-core usage at 30%, and they'll answer a ticket about software configuration — BandwagonHost won't. For sustained compute workloads, the "cheaper" option can easily cost more per unit of actually usable performance.

## Questions that come up before ordering

**Will a Tokyo VPS give me low latency to China?** It depends on your carrier more than the datacenter. China Mobile users on DC39v2 see 37–55ms typically; Telecom users see anywhere from 35ms (CN2 GIA) to 175ms spikes (DC39v2 at peak, some cities). Test your own route during the refund window.

**Can I pay with Alipay?** Yes. Credit card, PayPal, Alipay and UnionPay all work.

**What if the plan I want is sold out?** Limited plans restock in irregular batches. Watch stock.bwg.net or the official Telegram channel, and don't buy SakuraBox as a substitute unless you specifically accept 1Gbps and the older DC39 facility.

**Can I switch OS later?** Yes — KiwiVM supports OS reload anytime, plus snapshots, rDNS (PTR) management, an emergency console and an API.

**Do prices go up on renewal?** Limited plans renew at the price you originally paid, and the promo code's discount applies at renewal too. That's written into how the provider handles renewals, and it's rare in this market.

**Can I run a seedbox or a Tor node?** No. Both are explicitly prohibited in the terms of service, along with crypto mining, open proxies and bulk email.

## So which one should you actually buy

Mainly China Mobile or Unicom users, or anyone who wants maximum spec per dollar: **The Tokyo Plan v2 at $99/year**, roughly $92 with the code. It's the highest-bandwidth limited plan BandwagonHost sells, and the specs double the base plan for $20 more.

Tightest possible budget, light workload: the original **The Tokyo Plan at $79/year** (~$73.65 with the code). Respect the 1GB RAM and 30% CPU cap and it'll hold its end of the deal.

China Telecom users running anything latency-sensitive at evening peak: skip the limited plans and go **Tokyo CN2 GIA**, starting at $89.99/month. It costs ten times more because the return route is genuinely different, and no benchmark chart substitutes for CN2 GIA at 8pm.

Traffic-heavy mixed international use, or you want migration flexibility: **Osaka** — the Limited Edition 40G at $79.99/year for 2TB of traffic, or Osaka Starter at $499.99/year if you want a plan that's reliably in stock and can move datacenters later.

Before you click buy, two last checks: confirm the plan actually shows in stock (limited plans sell out quietly, and both v2 plans were reported out of stock as recently as April 2026), and confirm the discount appears in the cart before payment. If both check out, 👉 [order The Tokyo Plan while stock lasts](https://bandwagonhost.com/aff.php?aff=74518&pid=162) — and if it doesn't, the restock tracker will tell you when to come back instead of settling for a plan you didn't want.
