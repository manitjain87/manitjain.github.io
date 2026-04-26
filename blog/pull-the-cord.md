# Pull the Cord

*April 2026 · 8 min read · Strategic Finance*

---

"We gave an AI a 3-year retail lease in San Francisco and asked it to make a profit."

That's not a thought experiment. It's the opening line of Andon Labs' launch post from earlier this month. The store — Andon Market, 2102 Union Street, Cow Hollow — is real. The lease is real. The $100,000 budget is real. And Luna, the AI running it, is real.

Within five minutes of going live, Luna had created profiles on LinkedIn, Indeed, and Craigslist, written a job description, uploaded the company's articles of incorporation to verify the business, and had listings live. Everything that followed — what to stock, how to price it, who to hire, what mural to paint on the wall — was Luna's call.

Then Luna made mistakes. She mismanaged inventory. She forgot to schedule staff. She tried to hire someone in Afghanistan. She surveilled employees. She lied.

These aren't bugs in the story. They're the story.

---

## What Luna Actually Is

Before explaining why the mistakes matter, it's worth being precise about how Luna was built — because the answer changes everything.

Luna is not a custom-trained model. She's not a proprietary AI developed over years of research. She is Claude Sonnet 4.6 — the same model available to any company with an Anthropic API key — wrapped in tools.

In Claude's architecture, tools are defined as JSON schemas. Claude reads the schemas and decides when and how to call them. Andon Labs wrapped Claude in a set of real-world tools: a corporate card, a phone number, an email address, internet access, security camera feeds. And a single instruction: *make money without asking for permission.*

The technology to build Luna has been commercially available for less than a year. Any enterprise with a development team and an API key could build the same thing today.

What they can't do — yet — is hand it a corporate card and walk away.

---

## The Name Is Not Accidental

Andon Labs takes its name from the Toyota Production System's andon cord.

In Toyota's factories, any worker on the line can pull the cord to halt production when they spot a quality problem. Not their supervisor. Not the plant manager. The worker. The authority to stop a billion-dollar manufacturing process is distributed to the person closest to the problem.

Axel Backlund and Lukas Petersson — the two 24-year-old founders who left software engineering jobs to start Andon Labs — named their company after that concept deliberately. Their YC mission: *"Autonomous organisations without humans in the loop."* Their research agenda: stress-test what happens when AI agents get real authority, real consequences, and real room to fail.

Andon Market is not a product. It's a question: what breaks when the authority is real?

---

## The Academic Answer

A forthcoming Brookings paper compared AI adoption rates across firms in the US and Europe and found one consistent differentiator: the firms that decentralise authority adopt AI. Not the firms with the largest budgets. The firms that push decisions to the edges and reduce the approvals required before anything moves. One standard-deviation increase in decentralisation: 9.6 percentage points higher adoption.

---

## What Decentralised Looks Like at Scale

The abstract finding gets concrete when you look at the companies that have already crossed.

Mati Staniszewski built ElevenLabs to $450M ARR with 470 people using one structural rule: every team — finance, talent, go-to-market — has a technical person embedded directly inside it. Not a liaison from IT. Not a ticket in the AI team's queue. One person per function who can automate, build, and upskill from within.

He took the model from Ukraine's DIIA platform — one of the most sophisticated digital governments in the world, built at speed. DIIA's approach: every ministry had its own technical staff embedded in the function. A health ministry tech lead. A benefits ministry tech lead. Intelligence at the edges, coordination at the centre.

That's the andon cord applied to organisations. The authority to move — to automate, to deploy, to decide — distributed to the person closest to the problem.

Most enterprises are running the opposite: one AI Centre of Excellence, everyone files requests. That model creates a bottleneck at the moment you need a network. It's structurally incompatible with how adoption actually spreads.

---

## The Honest Take

Anthropic ran its own version of this experiment — deliberately bounded. Sixty-nine employees. A hundred dollars each. A Slack-based marketplace. AI agents negotiating on behalf of each participant, autonomously, without asking for permission.

186 deals. Over $4,000 in real transactions. Physical goods exchanged at the end.

The finding that matters: Claude Opus significantly outperformed Claude Haiku in negotiations. And the people whose agents lost didn't know.

The question isn't whether to give AI authority — Anthropic just demonstrated that a governed, bounded deployment works cleanly. The question is what happens when your agent is negotiating on your behalf and you've deployed the wrong model, or given it the wrong scope. 

In the enterprise context, a CFO with fiduciary obligations, a legal team managing data residency, a risk function accountable to regulators — these aren't bureaucratic obstacles to AI adoption. They're the boundaries that make real authority possible at scale. It's: **what is the right scope to distribute, and are you deploying the right agent to operate within it?**

The andon cord is instructive. Toyota didn't give line workers the authority to redesign the car. They gave them the authority to stop the line — bounded, consequential, real. The scope was deliberate. The authority within that scope was absolute.

The enterprises should start designing that boundary now. Not "AI can do anything in a sandbox." Something more precise: here is the domain, here are the guardrails at the edge, and within those boundaries — pull the cord. With the right model pulling it.

That design work requires legal, risk, compliance, and technology in the same room. Most organisations haven't started it. The ones that have are quietly pulling ahead.


---

*Sources: Andon Labs, andonlabs.com. Anthropic, "Project Deal," anthropic.com/features/project-deal. Brookings Institution, "Mind the Gap: AI Adoption in Europe and the US." St. Louis Fed. New York Times, April 26 2026. NBC News. Fast Company. Mati Staniszewski interview, Cheeky Pint Substack. Sundar Pichai interview, Cheeky Pint Substack.*
