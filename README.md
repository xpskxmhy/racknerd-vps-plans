# RackNerd VPS specials: which of the five annual plans do you actually need, does the renewal price hold, and can you get your money back? (Full plan table inside)

RackNerd's VPS specials are five annual KVM plans priced from **$21.99 to $119.99 a year**, and the rate you sign up at is the rate you renew at for as long as you keep the server. Most people should be choosing between the 2 GB at $35.99/year and the 4 GB at $59.99/year. What follows is where the line falls between those two, what the renewal clause actually says, and the limits that decide whether RackNerd is the wrong shop for you.

> **Quick pick:** the 4 GB KVM special at **$59.99/year** — 3 vCPU, 60 GB SSD, 7 TB monthly transfer — handles a Docker stack, a small database, a couple of sites behind a reverse proxy, and the 4 GB one-click apps such as Ollama or AnythingLLM. Running only a proxy, a bot or an uptime monitor? The 1 GB at $21.99/year is enough. 👉 [check the 4 GB special's current price and locations](https://my.racknerd.com/cart.php?a=add&pid=954&aff=11397)

## All five specials, side by side

Every plan below is KVM with full root access, one IPv4, a 1Gbps port, and deployment in multiple datacenters. Provisioning happens right after payment, so the box is online within minutes rather than after a manual review.

| Plan | vCPU / RAM / SSD / monthly transfer | Price | Billing | Order |
| --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 vCPU · 1 GB · 20 GB SSD · 3 TB | $21.99 | Annual | [ order the 1 GB special](https://my.racknerd.com/cart.php?a=add&pid=952&aff=11397) |
| 2 GB KVM VPS | 2 vCPU · 2 GB · 35 GB SSD · 5 TB | $35.99 | Annual | [ order the 2 GB special](https://my.racknerd.com/cart.php?a=add&pid=953&aff=11397) |
| 4 GB KVM VPS | 3 vCPU · 4 GB · 60 GB SSD · 7 TB | $59.99 | Annual | [ order the 4 GB special](https://my.racknerd.com/cart.php?a=add&pid=954&aff=11397) |
| 6 GB KVM VPS | 6 vCPU · 6 GB · 100 GB SSD · 12 TB | $89.99 | Annual | [ order the 6 GB special](https://my.racknerd.com/cart.php?a=add&pid=955&aff=11397) |
| 8 GB KVM VPS | 7 vCPU · 8 GB · 150 GB SSD · 20 TB | $119.99 | Annual | [ order the 8 GB special](https://my.racknerd.com/cart.php?a=add&pid=956&aff=11397) |

Two details worth flagging because older write-ups get them wrong. The 4 GB tier ships **3 vCPU cores**, not 2. And the control panel is **ctrl**, RackNerd's in-house panel, not SolusVM — ctrl covers power, OS reinstalls, an HTML5 VNC console, one-click apps, an inbound firewall and tier upgrades, and RackNerd publishes an interactive demo of it you can click through without an account.

## Pick by what you'll install, not by vCPU count

On a box this size, RAM runs out first. RackNerd publishes minimum memory for its one-click app catalog, which makes a better sizing rule than counting cores:

- **OpenClaw:** at least 8 GB
- **Hermes Agent, AnythingLLM, Ollama, LibreChat:** at least 4 GB
- **n8n, Coolify:** comfortable from 2 GB

That maps cleanly onto the ladder. A reverse proxy plus n8n or Coolify plus a couple of containers fits the 2 GB at $35.99. Once a local model enters the picture, the 4 GB at $59.99 stops being optional, and it is the cheapest tier that clears the 4 GB threshold. OpenClaw is the one workload that forces the 8 GB at $119.99 — nothing below it qualifies.

The 1 GB tier is fine for a proxy, a bot, a VPN endpoint, a DNS or monitoring box. Put a real database on it with 20 GB of disk and 1 vCPU and you'll spend your evenings in the console.

The 6 GB at $89.99 is the awkward rung. Thirty dollars more buys 8 GB, 7 vCPU, 150 GB of disk and 20 TB of transfer. Buy the 6 GB only if 100 GB of storage and 12 TB of bandwidth describe your actual ceiling and the extra RAM would sit idle.

## What "lifetime recurring" means for your bill

RackNerd states it plainly in the specials FAQ:

> "These RackNerd VPS specials are lifetime recurring. You can renew at the same rate for as long as you decide to keep the service."

No intro rate that doubles in year two, which is the usual trap in this price bracket. The same 2 GB tier on standard monthly billing works out to roughly $247 a year, about seven times the $35.99 special, though the monthly plan does include more storage and an extra vCPU. The specials themselves are annual only. If you want month-to-month, you're on the standard plans, not this list.

👉 [see the 2 GB special at $35.99/year](https://my.racknerd.com/cart.php?a=add&pid=953&aff=11397)

## Five things to check before you pay

**1. There is no money-back guarantee.** The terms read: "Refunds are issued on a case-by-case basis since by default no refunds are provided once payment is received." The knowledge base is blunter still — no refunds, no guarantee, prepaid account credit isn't returnable. A dead-on-arrival VPS is the realistic refund case. A change of mind isn't. RackNerd's own suggested workaround is to buy monthly first, confirm the route and the load, then move to an annual special.

**2. It's unmanaged.** You get root and a panel. ctrl handles power, reinstalls, the VNC console, one-click apps and firewall rules, and RackNerd support is available 24/7 for platform problems. Nobody is going to debug your Nginx config or your database.

**3. Nested virtualization needs written approval.** Running VMs or reselling VPS slices inside one of these requires permission, and exposed VT-x/AMD-V flags aren't guaranteed. Container workloads are explicitly allowed: Docker, Docker Compose, LXC/LXD, Kubernetes, K3s. CPU mining, outbound DDoS, spam and brute-force traffic are banned platform-wide.

**4. IPv6 is limited by location.** Up to 100 free IPv6 addresses via support ticket in Los Angeles and France; other datacenters are listed as coming soon.

**5. You don't need a coupon.** The specials are already the discounted price. Codes circulating as "30% off VPS" don't apply here, so don't let an expired code stop you at checkout. Stock OS templates are CentOS, Rocky Linux, AlmaLinux, Fedora, Debian and Ubuntu; anything else, including a custom ISO, goes through a support ticket.

👉 [see all five annual specials in one list](https://bit.ly/RacKnerd)

## The fall giveaway closes November 30

RackNerd's current promotion runs through **November 30, 2026** and requires no purchase. Prizes: a Meta Quest 3 512GB, a Synology DS225+ two-bay NAS, two Acer Nitro 27-inch monitors, five KVM VPS (4 GB RAM, 3 vCPU, 60 GB SSD, 7 TB transfer) free for the first year and renewing at $59.99/year with no obligation, and ten $50 account credits.

LowEndTalk members get extra entries: send a private message to @giveaway containing the word **PUMPKIN**, and you'll get a code worth 100 bonus entries. Accounts needed to be 30 days old as of November 1, 2026 to qualify for that bonus. If you're reading this after the deadline, ignore the section — it won't reopen.

## FAQ

**Can I run Docker and WordPress?**
Yes. Docker with Portainer is a one-click install in ctrl, or install it yourself over SSH. WordPress fits AdminBolt, CyberPanel or CloudPanel, all one-click, or you can build the stack manually. A 2 GB plan covers a modest WordPress site; a busy WooCommerce store with Redis wants the 4 GB.

**Can I install Windows?**
Not from the stock templates, which are all Linux. Custom ISO installs are available on request via ticket, so ask support about your specific image before paying rather than assuming.

**Can I upgrade later?**
Yes, one tier up, and it takes a reboot of roughly a minute. The server isn't rebuilt, and ctrl handles the move.

**Is this managed hosting?**
No. Unmanaged KVM with root access.

**Can I get more IPs?**
One IPv4 is included on every plan. Extra IPv6 addresses are free in Los Angeles and France, up to 100, requested by ticket.

## Which one to buy

Match the plan to the job and stop there:

- Proxy, bot, VPN endpoint, monitoring, DNS: **1 GB at $21.99/year**
- Docker stack, small database, a few sites, n8n or Coolify: **2 GB at $35.99** if it's lean, **4 GB at $59.99** if you'd rather not think about it again
- Ollama, AnythingLLM, LibreChat, Hermes Agent: **4 GB at $59.99** is the floor
- OpenClaw or a pile of containers: **8 GB at $119.99**
- Running VMs inside a VPS or reselling slices: none of these — that's a dedicated server conversation

Before checkout, confirm two things on the order form: the datacenter closest to your users, and that you're buying an annual plan, because that's the only billing cycle the specials come in.

👉 [open the 1 GB special at $21.99/year](https://my.racknerd.com/cart.php?a=add&pid=952&aff=11397)
