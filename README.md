# Windows VPS License Included: What That Phrase Really Covers, Three Billing Models Compared, and How to Price a Windows Server Before You Order

A Windows VPS advertised at $3.99 a month and another at $13.50 can end up costing the same by month two. The gap comes from what each provider means by "Windows." Some bundle a Microsoft licence into the monthly fee. Some hand you a template and a reminder to bring your own key. Some ship a 180-day evaluation that starts shutting the server down every hour once it lapses. The headline price tells you nothing about which of the three you are buying.

Below are the three models with the published numbers from providers using each, the checks that separate them in under a minute, and how the same test applies to AvaHost (ava.hosting), whose Windows VPS range runs from €5/mo for a 1 vCPU managed box up to €40/mo for 8 vCPU and 16 GB RAM, all KVM with dedicated cores and NVMe, hosted in Chișinău, Moldova.

> **Where to start:** AvaHost's €10/mo Windows plan (2 vCPU / 4 GB RAM / 50 GB NVMe) covers a small IIS or .NET site, a SQL Server Express database, or two or three people on RDP. If you would rather not patch the OS yourself, the managed Windows line starts at €5/mo. Either way, get the licence terms confirmed in a ticket before you pay, because that one answer can change the monthly cost by more than the server itself.
>
> 👉 [See AvaHost's Windows VPS plans and current EUR prices](https://my.ava.hosting/aff.php?aff=15562)

## Three things "license included" can mean

| What the page says | What you actually get | Providers doing it |
| --- | --- | --- |
| "Licence included", "no additional licence fees" | The provider holds the licence, usually under SPLA, and it is inside the monthly fee | Redeco Hosting (Windows Server 2025 Standard), Virtarix (base OS image) |
| "BYOL", "licence not included" | You supply the key, activate it, and stay compliant | VPSGrid, Vultr (separate fee on top of the base price) |
| "$0 licence cost", "evaluation" | Microsoft's 180-day evaluation build, with the licence sold as an add-on | MassiveGRID ($6.31 per vCPU/month) |

**Bundled, in the monthly fee.** Redeco Hosting states that every Windows Server VPS includes a valid Microsoft SPLA licence for Windows Server 2025 Standard, with no additional licence fees and free installation; Windows Server 2022 is available on request. Datacenter edition, RDS CALs and SQL Server licensing are quoted separately. Virtarix includes the licence for the base Windows Server image and says you do not need to bring your own key for a standard deployment, while noting that separate Microsoft licensing may still apply for extra roles, users, or software you install.

**Bring your own.** VPSGrid's policy is explicit: its Windows VPS plans are BYOL, the provider supplies the KVM virtual machine, a Windows Server template, the primary IP, power controls and billing, and you supply and activate a valid licence. Support cannot choose or validate a Microsoft licence for you and cannot activate Windows on your behalf. The company also spells out something worth repeating: RDP access is how you administer the server, and RDP being available does not mean a licence is included. Vultr takes a slightly different route to the same place, applying an additional licensing fee on top of the base monthly price, sized by the Compute plan you pick.

**Evaluation, with the licence as an upgrade.** MassiveGRID installs every Windows Server template (2016, 2019, 2022, 2025) as Microsoft's evaluation build at no licence cost. It must be activated online within the first 10 days, then runs fully featured for 180 days with the remaining days shown on the desktop. After day 180 your data and software stay in place, but the server shuts down every hour until a licence is added, and adding it converts the installation in place with no reinstall. The licence costs $6.31 per vCPU per month, so $12.62/month on 2 vCPU and $25.24/month on 4 vCPU.

## Four checks that settle it in under a minute

1. **Does the plan name carry "(BYOL)"?** VPSGrid labels its plans that way in the store, which makes it hard to miss once you know to look.
2. **Is there a separate licence line in the cart?** Per-vCPU pricing (MassiveGRID) or a per-plan surcharge (Vultr) both mean the advertised price is a shell price.
3. **Does the page mention activation within N days, or a countdown on the desktop?** That is an evaluation build, and the clock starts the day you provision, not the day you start using it seriously.
4. **Does it separate the base OS licence from RDS CALs and SQL Server?** Virtarix and Redeco both do. If a provider never mentions them at all, assume they land on you.

## What a Windows VPS costs once the licence is real

The cheapest Windows VPS listings are usually one of two things: an evaluation build, or a box too small to run the OS. MassiveGRID's $3.99 plan is 1 vCPU, 1 GB RAM and 32 GB NVMe, and the same page states that Windows Server itself uses about 2 GB of RAM. That configuration pages from the first boot, and the licence is another $6.31 per vCPU on top of it.

| Provider | Entry configuration | Licence cost on top | Catch |
| --- | --- | --- | --- |
| MassiveGRID | 1 vCPU / 1 GB / 32 GB NVMe, $3.99 | $6.31 per vCPU/month | 180-day evaluation; 1 GB is below Windows Server's ~2 GB footprint |
| Vultr | Varies by Compute plan | Extra fee, rate published on its Windows Servers page | Base monthly price excludes the licence |
| VPSGrid | Varies by plan | Your own licence | Support will not activate or validate it |
| Virtarix | 3 vCPU / 6 GB / 50 GB NVMe, $13.50 | Included for the base OS image | RDS CALs may be extra |
| Redeco Hosting | 4 GB RAM recommended minimum | Included, SPLA | Datacenter, RDS CALs and SQL quoted separately |

Here is where the arithmetic gets uncomfortable for the "cheap" model. At $6.31 per vCPU, a three-core licence alone runs about $18.93 a month, which is more than Virtarix charges for an entire 3 vCPU / 6 GB server with the licence already inside. On the entry MassiveGRID box the licence takes $3.99 to $10.30 before you have added the RAM that Windows actually needs.

That comparison is the whole point of reading the licence line. "Included" is worth roughly one small VPS per month, per core on some providers.

## AvaHost's Windows VPS plans and prices

| Plan | vCPU / RAM / NVMe | Price | Suits | Order |
| --- | --- | --- | --- | --- |
| Managed Windows VPS, entry | 1 / 2 GB / 25 GB | €5.00/mo | Staging, a single small app, patching handled by AvaHost | [Open plan](https://my.ava.hosting/aff.php?aff=15562) |
| Windows VPS, minimum documented plan | 2 / 4 GB / 50 GB | €10.00/mo | IIS or .NET site, SQL Express, one or two admins | [Open plan](https://my.ava.hosting/aff.php?aff=15562) |
| Managed Windows VPS, top of range | 8 / 16 GB / 160 GB | €40.00/mo | SQL Server, several services, multi-user work | [Open plan](https://my.ava.hosting/aff.php?aff=15562) |

Every plan is KVM with dedicated vCPU cores, NVMe storage, a 1 Gbps port, unlimited bandwidth, DDoS protection at no extra cost and a dedicated IPv4 address. The network and power SLA is 99.9% uptime, support runs 24/7 over ticket and chat, and the servers sit in Chișinău, Moldova, which is a reasonable latency bet for European users and a worse one for US or Asian traffic. Configurations between these three points are in the order configurator, which is the authority on both spec and price.

AvaHost also runs a Linux/KVM line called Power VPS at €5 (VPS One), €20 (VPS Power) and €40 (VPS Ultra). If the workload turns out not to need Windows, that is where the money goes instead.

## Does AvaHost's price include the Windows licence?

This is the question to nail down before paying, and the honest state of the public pages is that they describe the Windows product without spelling out the licence paperwork.

What is documented: Windows Server is sold as a product, not a template you cobble together, with Windows Server 2012, 2016 and 2019 images listed in AvaHost's own FAQ. The managed Windows VPS takes over OS configuration, software installation, patch management, IIS bindings and application pools, and Windows Firewall rules. SQL Server is described as running natively on Windows Server.

What is not documented anywhere I could read: whether the licence sits under AvaHost's SPLA in their name, or whether you are expected to bring a key. Nor which edition gets installed, nor who supplies RDS CALs when a third person needs to log in at the same time.

That gap is worth one support ticket, because the difference is not cosmetic. On the numbers above, a licence you have to buy yourself can add more per month than the server costs. AvaHost's Windows entry point also sits at €10 while the Linux/KVM entry sits at €5, and whether that €5 gap is the licence is exactly the sort of thing a provider will answer in one line.

Send this, verbatim, if it helps:

1. Is the Windows Server licence included in the monthly price, and under which arrangement (SPLA in your name, or BYOL with my key)?
2. Which Windows Server edition and version will be installed, and does it activate automatically on first boot?
3. If more than two people need to connect over RDP at once, do you supply RDS CALs, and at what price?

👉 [Check the plan notes on AvaHost's Windows VPS order page](https://my.ava.hosting/aff.php?aff=15562)

## The limits that never make the headline

**Two admin sessions by default.** MassiveGRID spells it out: every server comes with the two administrative sessions Windows Server allows, and anything beyond that needs extra RDP user licences at $8.90 per user per month plus Remote Desktop Services configuration. Virtarix says the same thing in softer language. A team of five on one Windows VPS is a licensing project, not a configuration tweak.

**Desktop Windows cannot be rented.** Microsoft does not let hosting providers rent out desktop Windows licences, so Windows 10 Pro and 11 Pro images install unactivated and you enter your own product key after the first login. Windows 11 Pro needs at least 2 GB of RAM, which is why the smallest configuration starts there rather than at 1 GB. Windows 10 reached end of support on 14 October 2025 and no longer receives security updates, so new builds should use Windows 11 Pro or Windows Server.

**BYOL has categories, and some of them do not cover production.** VPSGrid's knowledge base lists the traps: retail licences are often intended for a single server you control and cloud eligibility depends on the SKU; Volume Licensing cloud rights may hinge on Software Assurance; MSDN and Visual Studio subscriber licences are typically limited to development and test and not for production workloads; SPLA is for hosts, not for end-customer BYOL.

**SQL Server is a separate bill.** SQL Server Express is free and covers databases up to 10 GB. Web and Standard editions need your own licensed copy on most providers, and Redeco quotes SQL Server licensing separately rather than bundling it.

**Windows Server eats memory before your app does.** Budget about 2 GB for the OS. Redeco recommends at least 4 GB for an RDP workstation or small .NET app, and 8 GB with dedicated vCPUs for SQL Server, Active Directory, or several concurrent RDP sessions.

## When the managed option earns its price

AvaHost's managed Windows VPS covers OS patching, IIS bindings and app pools, firewall rules and component upgrades, with DDoS mitigation already in the price. If you are running a .NET application for a business and nobody on staff wants to own Windows Update on a Sunday, that is the version to buy. If you are a developer who will be on the box daily anyway, the unmanaged Windows VPS at €10 keeps the same KVM isolation and NVMe without paying for remote hands.

👉 [Compare AvaHost's managed Windows plans](https://my.ava.hosting/aff.php?aff=15562)

## Which configuration fits which workload

A single IIS or ASP.NET site, SQL Server Express, one or two administrators: the 2 vCPU / 4 GB / 50 GB plan at €10/mo. Nothing above that buys you anything you will notice.

SQL Server Standard, Active Directory, or a small team connecting over RDP: 8 vCPU / 16 GB / 160 GB at €40/mo, and get the RDS CAL question answered before you deploy, not after.

A staging environment or one small internal app where you would rather not manage patching: the managed entry at €5/mo, accepting 1 vCPU and 2 GB as its ceiling.

A Linux workload: skip Windows entirely and look at the Power VPS line, where €5 buys a 1 vCPU instance without the licensing question hanging over it.

## FAQ

**Is the Windows licence included in a Windows VPS price?**
Depends on the provider, and the page usually tells you if you know the three patterns. Bundled (Redeco, Virtarix), BYOL (VPSGrid), or evaluation plus a per-vCPU add-on (MassiveGRID at $6.31 per vCPU per month).

**Can I install my own Windows Server key on a VPS?**
Yes on BYOL providers, but the licence has to permit cloud or VPS use. MSDN and Visual Studio subscriptions are generally development and test only, and volume licences may depend on Software Assurance.

**How many people can use one Windows VPS at the same time?**
Two administrative sessions come with Windows Server. More than that needs Remote Desktop Services plus RDS CALs, which at MassiveGRID run $8.90 per user per month before any configuration work.

**Does a 1 GB Windows VPS work?**
Not for anything you care about. Windows Server itself uses roughly 2 GB of RAM, so a 1 GB plan is an evaluation toy or a very slow experiment.

**Can I get Windows 11 Pro on a VPS instead?**
On providers that offer the template, unactivated, with your own key, at 2 GB RAM minimum. Windows 10 is out of support as of 14 October 2025 and should not be used for new deployments.

## Before you order

Match the plan to the workload first, then settle the licence question. For most people that means AvaHost's 2 vCPU / 4 GB plan at €10/mo for a single Windows application, or the 8 vCPU / 16 GB at €40/mo if SQL Server or a multi-user RDP setup is involved.

Two things to confirm in writing before you pay: whether the monthly price covers the Windows Server licence and which arrangement it sits under, and whether a third concurrent RDP user needs CALs you have to buy. Both answers change the real monthly cost, and neither is in the headline price.

👉 [Start with AvaHost's €10/mo Windows plan](https://my.ava.hosting/aff.php?aff=15562)
