# Cheap dedicated server at Vultr: what $120/month buys, why year two costs the same, and when a $5 instance is the better buy (all 11 plans)

Vultr's cheapest dedicated server is **$120/month**: an Intel E3-1270 with 4 cores, 32 GB RAM, 2 × 240 GB SSD and a 10 Gbps port, billed hourly with no setup fee, and it renews at the same $120. That is well above the numbers most "cheap dedicated server" pages lead with. Scaleway lists a €4.99/month box, Namecheap advertises $37.33/month for the first year, and the general market band sits around $50–100/month. Everything Vultr sells below $120 is a cloud compute instance, not a physical machine.

So the useful question is what the extra money buys, and what the cheaper headline prices turn into once the discount period ends. Both parts are checkable with published numbers, and this page does the arithmetic.

## Quick pick

> **Need a physical machine with a fast port and no lock-in:** the **$120/month E3-1270** (4 cores, 32 GB, 2 × 240 GB SSD, 10 Gbps) is Vultr's entry dedicated plan. Hourly billing, no setup fee, identical renewal price. 👉 [Check the $120 E3-1270 dedicated plan](https://www.vultr.com/products/bare-metal/?ref=9738262-9J)
>
> **Need to run a site, a proxy or a build box:** a $5–$20 cloud compute instance covers it, and Vultr charges the same rate on renewal there too.

## All 11 Vultr dedicated plans

Every plan below is unmanaged, comes with no control panel licence and no managed support tier, and is billed hourly with no setup fee. None of the dedicated plans are listed as including DDoS protection, so budget for that separately if you need it.

| Plan (CPU) | RAM | Storage | Port | Price | Order |
| --- | --- | --- | --- | --- | --- |
| Intel E3-1270, 4 cores | 32 GB | 2 × 240 GB SSD | 10 Gbps | $120/mo | [E3-1270 price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| Intel E-2286G, 6 cores | 32 GB | 2 × 960 GB SSD | 10 Gbps | $185/mo | [E-2286G price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 4245P, 6 cores | 32 GB | 2 × 960 GB NVMe | 10 Gbps | $295/mo | [EPYC 4245P price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| Intel E-2288G, 8 cores | 128 GB | 2 × 1.92 TB NVMe | 10 Gbps | $350/mo | [E-2288G price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| Intel E-2388G, 8 cores | 128 GB | 2 × 1.92 TB NVMe | 10 Gbps | $350/mo | [E-2388G price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 4345P, 8 cores | 64 GB | 2 × 1.945 TB NVMe | 10 Gbps | $365/mo | [4345P 64 GB price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 4345P, 8 cores | 123 GB | 2 × 1.945 TB NVMe | 10 Gbps | $395/mo | [4345P 123 GB price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 7443P, 24 cores | 256 GB | 2 × 480 GB SSD | 10 Gbps | $725/mo | [EPYC 7443P price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 9254, 24 cores | 384 GB | 2 × 480 GB SSD | 10 Gbps | $825/mo | [EPYC 9254 price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 9255, 24 cores | 384 GB | 2 × 480 GB NVMe | 10 Gbps | $995/mo | [EPYC 9255 price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |
| AMD EPYC 9354P, 32 cores | 768 GB | 2 × 480 GB SSD | 10 Gbps | $1,450/mo | [EPYC 9354P price](https://www.vultr.com/products/bare-metal/?ref=9738262-9J) |

Two things stand out in that list. Every plan ships a 10 Gbps port, which is not standard at the low end of this market. And the first NVMe plan costs $295, so if you want NVMe rather than SATA SSD, the entry price more than doubles. Work out whether your workload is actually disk-bound before paying that jump.

Vultr's cloud compute line, for reference: $2.50/month for 512 MB and 1 vCPU (IPv6-only), $3.50 with IPv4, $5/month for 1 GB / 1 vCPU / 25 GB SSD / 1 TB transfer, $20/month for 4 GB / 2 vCPU / 80 GB, $80 for 16 GB / 6 vCPU. Bandwidth overage runs $0.01/GB and block storage $0.10/GB/month.

## Where $120 sits on the price ladder

Cheap dedicated hardware in late 2026 clusters into three tiers, and each tier buys a different thing.

The bottom is Scaleway's **€4.99/month** START-2-S-SSD: an Intel Avoton C2350 at 2 cores / 2 threads, 1.7 GHz, 4 GB RAM, one 120 GB SSD, up to 1 Gbps. This runs a static site, a jump host or a monitoring node. It will not run a database you care about.

The middle is crowded. Namecheap's **$37.33/month** first-year price (list $87.88) gets a Xeon E-2236, 6 cores / 12 threads, 32 GB ECC DDR4 and 2 × 480 GB SSD in software RAID. Server Mart lists an E3-1220 with 16 GB and a 480 GB SSD at **$45/month**, an E3-1230v3 with 32 GB at **$54/month**, and an 8-core E5-2667v4 with 64 GB at **$49.50/month** on a 50% discount. That is a lot of cores and RAM per dollar.

Vultr enters at **$120**. On cores and RAM alone it loses to Server Mart and Namecheap's first year. What the $120 covers is the 10 Gbps port, hourly billing, a same-price renewal and a footprint across 20 countries, including the US, Germany, UK, Japan, Singapore, Brazil and India. If your reason for wanting a dedicated box is raw cheap RAM, Vultr is not the cheapest answer and pretending otherwise wastes your time.

## The second year is where cheap prices end

Namecheap publishes both numbers side by side, which makes the arithmetic easy. The $37.33 plan lists at $87.88. The $41.53 plan lists at $69.88. The $135.41 dual-Xeon plan lists at $227.88. Those are first-year discounts of 58%, 41% and 41%, and they expire.

Take the $37.33 box. Year one costs $447.96 if you prepay annually. Year two costs $1,054.56 at list. Over three years you pay roughly $2,557, and the monthly figure you compared against other providers was only true for twelve months. Namecheap also states that its displayed monthly prices are based on annual billing, so the entry ticket is the full $447.96 up front, not $37.33.

Scaleway takes the opposite approach. Its low prices are tied to 12- or 36-month commitments, with the 36-month term saving up to 15%, and the commitment plans are the ones that freeze your monthly rate and reserve hardware stock. You get price certainty by giving up the ability to leave.

Vultr sits in a third position: no prepayment, no commitment, hourly billing, and the listed price is the renewal price. A $120 plan run for 40 hours costs about $6.90 at Vultr's hourly rate rather than a month's rent, and a month is capped at 672 billable hours. Over three years the E3-1270 runs $4,320, more than the discounted Namecheap box. For a workload that exists for three years straight and never needs more than 32 GB, the cheaper first-year deal wins on cash. For anything intermittent, or anything you might move in eight months, the hourly model is what keeps the total down.

## What the sticker price leaves out

Namecheap's management tiers are separate line items: **Basic $20/month**, **Complete $50/month**, or user-responsible for free. Add Basic to the $37.33 plan and you pay $57.33, a 54% increase. Add Complete and it is $87.33, up 134%. In year two those become $107.88 and $137.88 against an $87.88 base.

Per-incident charges sit on top of that. A server restore is $10 flat. A core software change, meaning an OS reinstall or a version change, is $20 flat for the first hour and $10/hour after. Root-cause investigation follows the same schedule. cPanel is billed separately now, starting at **$19.88/month** for the Solo tier, so a $37.33 box with Basic management and cPanel lands near $77/month before you have installed anything.

The equivalent costs at Vultr are yours to arrange. Plans are unmanaged, which means the OS, the panel, the hardening and the backups are your work or your contractor's invoice. Vultr's dedicated line is also listed without DDoS protection and without self-serve IPMI/KVM, so a failed reinstall is a support ticket rather than a console session. Those are real limits, and they are the reason the $120 plan is not $185.

## Billing details that cost more than the plan

Three rules on Vultr's billing pages catch people who assume a powered-off server is a free server.

Charges start when a server is deployed, whether it is running or not. Stopping an instance does not stop billing, because the compute, storage and IP allocation stay reserved. To end billing you destroy the server. If you spin up a $120 box to test a migration over a weekend and just power it off, the meter keeps running.

There are no refunds on services, and credits are non-refundable. Prepaying is not reversible, so start with hourly billing until the workload is proven.

Promotional credit is not cash. The current offers include **$300 free credit** on the FLY300VULTR code, $200 on FLYTWOHUNDRED, $250 on 250VULTRFLY, and a deposit match up to $100 on VULTRMATCH. All of them are new-customer only, require a linked card or PayPal, are limited to one code per user, cannot be combined with other offers, and apply to select products only. Unused credit expires, with the current offer text putting the window at 30 days. 👉 [See Vultr's current credit offers](https://www.vultr.com/coupons?ref=9738262-9J)

At $120/month, $300 covers two and a half months of the entry dedicated plan at list price, if the credit is eligible for that product line. The terms say select products, so confirm in the console that the credit is being applied before you assume the first months are free.

## Which plan fits which job

**A static site, a proxy, a VPN endpoint or a monitoring node.** Take the $5/month cloud compute tier, or the $2.50 IPv6-only tier if your provider supports IPv6. A physical machine at $120 is 24 times the cost for capacity you will not touch.

**One busy site or database with steady load.** The $120 E3-1270 is the floor here, and 32 GB of RAM is the part that matters, not the four cores. Check your disk IOPS before assuming the SATA SSDs are enough.

**Multiple sites with real memory pressure.** The $350 E-2288G or E-2388G at 128 GB and 2 × 1.92 TB NVMe is the point where NVMe stops being an add-on. Above that, the $725 EPYC 7443P at 256 GB is the next step, and the $1,450 EPYC 9354P at 768 GB is for virtualization hosts.

**Seasonal or short-lived workloads.** Anything measured in hours or weeks belongs on Vultr regardless of spec, because the alternative is a 12-month term you cannot exit.

**Strict EU data residency on a tiny budget.** Scaleway's Paris, Amsterdam and Warsaw regions start at €4.99 with a 99.9% SLA. Vultr has European locations too, but not at that price.

## When Vultr is the wrong buy

Your budget is under $100/month and the machine will run continuously for years: Server Mart's $45–$54 plans and Namecheap's first-year pricing give more cores and RAM per dollar, and Server Mart's 24-hour free trial lets you verify the box before committing.

You want the provider to manage the server: Namecheap's Complete tier at $50/month includes weekly backups to separate storage up to 200 GB, and Vultr has no equivalent line item.

You need DDoS protection bundled, or self-serve IPMI/KVM on a $120 box, or a refund window. Vultr's dedicated plans do not list the first two, and its refund policy is explicit that payments are final.

You want an unmetered port. HOSTKEY advertises 1–10 Gbps ports with free inbound traffic, but outbound is capped by the traffic plan you buy, so read the allowance rather than the port speed. Note also that HOSTKEY's own page gives uptime as both 99.982% per year and a 99.99% guarantee.

| Provider | Cheapest verified plan | Spec | Price | Billing note |
| --- | --- | --- | --- | --- |
| Scaleway | START-2-S-SSD | Avoton 2C/2T 1.7 GHz, 4 GB, 120 GB SSD | €4.99/mo | most low prices need 12- or 36-month commitment |
| Namecheap | Xeon E-2236 | 6C/12T, 32 GB ECC, 2 × 480 GB SSD | $37.33/mo first year, $87.88 list | monthly figure assumes annual prepay |
| Server Mart | E3-1220 | 4 cores, 16 GB, 480 GB SSD + 500 GB SATA | $45/mo | 100 Mbps unmetered port, US locations only |

## Before you order

Match the plan to the constraint that actually binds. If it is RAM, the $120 and $350 tiers are the ones that matter and the core count is noise. If it is disk speed, the $295 EPYC 4245P is the first NVMe plan and there is no cheaper way into NVMe on the dedicated line. If it is price alone, Vultr is not the cheapest dedicated host in this market and no amount of plan comparison changes that.

Two things to confirm at checkout rather than assume: whether the $300 credit applies to the dedicated product line for your account, and whether you are being billed hourly or monthly. Hourly keeps you flexible and costs slightly more per month; monthly lowers the rate but starts the meter whether the server is on or off, and only destroying the instance stops it.

👉 [Start with the $120 E3-1270 and scale up when the workload proves it needs more](https://www.vultr.com/products/bare-metal/?ref=9738262-9J)
