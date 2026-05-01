# The Trust Stack for Agentic Commerce

Query a major luxury retailer's product catalog with a plain HTTP request — no browser, no login, no JavaScript. You get back 60 products with prices and brand reference codes. Query a second retailer the same way. You get: `Reference BOT: 0.561e1202.1777634870.45b2368`.

One shows up when a customer asks an AI shopping agent to find the best price. The other doesn't. Neither made that decision deliberately.

In April 2026, Cloudflare processed 241 billion tokens through AI Gateway in a single week. The same week, they shipped MCP Server Portals — infrastructure that lets any merchant decide which AI agents can access their storefront, with what permissions, against a verified identity. Google and Shopify's Universal Commerce Protocol, now backed by Visa, Mastercard, Amazon, and Stripe, added a credential layer that lets a shopping agent prove a real customer is behind it.

The trust stack for agentic commerce is being assembled. Here is what each layer does and who's building it.

---

## The problem agents create

When an AI shopping agent queries a product catalog, it arrives with the same signature as a scraper: a plain HTTP request, no credential, no intent signal. A merchant cannot distinguish OpenAI's Shopping feature — routing a customer ready to buy — from a competitor's price monitor extracting data for arbitrage.

Without a way to tell them apart, merchants face a bad binary: block all unrecognised traffic and lose distribution through the AI interfaces their customers are using, or allow everything and hand pricing data to every competitor running an automated monitor.

The trust stack is how merchants avoid choosing between them.

---

## Layer 1 — robots.txt: signal, not security

OpenAI, Google, and Perplexity publish the user agents their shopping crawlers send: GPTBot, Google-Extended, PerplexityBot. Allowlisting them in robots.txt and blocking everything else takes an hour and costs nothing.

This won't stop a sophisticated actor who spoofs the header. But it immediately filters commodity scrapers who don't bother. It also sends a signal to legitimate agents that the merchant wants to be found — the same way adding a sitemap in 2005 told Google a site wanted to be indexed.

---

## Layers 2 and 3 — Cloudflare: behaviour detection and authenticated access

A legitimate shopping agent behaves like a customer. It searches, filters, opens a product page, checks availability. A scraper hits listing pages in parallel across all categories — dozens of simultaneous connections, no session continuity, no cart interaction. The pattern is distinguishable at the network level before a request reaches application code.

Cloudflare's behavioural fingerprinting runs at the CDN layer: request cadence, sequential versus parallel access, session continuity. Any merchant on Cloudflare gets this without building it.

Cloudflare MCP Server Portals, now in open beta, goes further. It centralises every agent connection — authenticated, permissioned, observable in one place. A merchant configures it to serve structured product data to agents with verified identities and return nothing to everything else. The 241 billion tokens Cloudflare processed through AI Gateway in Agents Week represent the operating scale this infrastructure already runs against. A concrete example of what this looks like in practice: Cloudflare's own internal teams — product, sales, marketing, finance — are now running agentic workflows through the same MCP infrastructure they ship to merchants. They built it for themselves first, which is how the edge cases get found.

---

## Layer 4 — UCP + AP2: the credential standard

Cloudflare implements the authentication check. The Universal Commerce Protocol defines what the credential means.

UCP, co-developed by Google and Shopify and backed by Amazon, Meta, Microsoft, Stripe, Visa, Mastercard, Amex, Walmart, Best Buy, and Zalando among others, includes AP2 — the Agent Payments Protocol. AP2 gives a shopping agent a verifiable credential to present to any merchant: proof that a real customer with purchase intent is behind the request. Not a spoofable header — a cryptographically signed token in a standard the entire commerce infrastructure is converging on.

A practical example of what this changes: when a customer tells their AI assistant to find and buy a specific item, the agent queries merchants using AP2 credentials. Merchants inside the UCP trust layer receive the query, verify the credential, and respond with structured product data. Merchants outside it don't receive the query — the agent has no authenticated channel to reach them.

The analogy that holds: OAuth standardised "which apps can access your account data." UCP/AP2 is standardising "which agents can access your storefront." The consortium building it overlaps almost entirely with the consortium that built card payments infrastructure — these companies set defaults, they don't propose options.

---

## What this stack means for distribution

Agent traffic is becoming the dominant discovery channel for commerce in the way search traffic did in 2005–2010. The merchants inside the trust stack receive those queries. The merchants outside it don't.

This is a distribution decision, not a security decision. Security budget protects a site. This budget determines whether the site appears when customers shop through AI. The window to be intentional about which side of the stack you're on is roughly 12 months — before the standards solidify and the defaults get set by the companies who are already setting them.

---

*Sources: Cloudflare Agents Week in Review (blog.cloudflare.com/agents-week-in-review) · Cloudflare Enterprise MCP (blog.cloudflare.com/enterprise-mcp) · Cloudflare MCP Server Portals (blog.cloudflare.com/zero-trust-mcp-server-portals) · Universal Commerce Protocol (developers.googleblog.com, shopify.engineering/ucp)*
