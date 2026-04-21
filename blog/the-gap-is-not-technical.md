# The Gap Is Not Technical

*April 21, 2026 · 9 min read · Strategic Finance*

---

Sundar Pichai runs the most AI-capable company on earth. Mati Staniszewski built a voice AI company from zero to $450M ARR in three years with 470 people. Neither of them thinks the bottleneck is the technology.

The gap between what AI can do and what enterprises have deployed is not a capability gap. It's an organisational gap. And it's bigger than most leadership teams realise.

---

## The Capability Is Already There

Pichai's arc is worth sitting with for a moment. Google Brain's cat recognition demo in 2012 felt like a research curiosity. By 2026, he's describing agents completing complex multi-step tasks without human supervision — and coding workflows where the programming language has become an irrelevant detail. What matters is the outcome; the implementation is delegated.

Staniszewski's arc is even more compressed. Three years ago, voice AI wasn't good enough for production. Two years ago, real-time versions started working. A year ago, production-ready systems with context and memory became viable. Today, voice agents pass the Turing test for customer support. Automotive OEMs know the technology is ready. They haven't integrated it. That's not a technology problem.

The question enterprises need to stop asking is "is AI good enough yet?" For most use cases, that question has been answered. The question is: why hasn't your organisation deployed it?

---

## The Five Real Blockers

John Collison at Stripe — via Pichai — gave the clearest taxonomy I've seen of what's actually in the way. None of the five are technical:

**1. Prompting expertise.** Generic prompting underperforms. Getting real value requires domain-specific knowledge of how to instruct models for your context — Stripe-specific prompting, Farfetch-specific prompting. That expertise has to be built, and it takes time.

**2. Data access pipelines.** Agentic workflows require clean, accessible data. Most enterprises have data that is siloed, inconsistently formatted, and permission-controlled in ways that predate the concept of an agent needing to traverse it.

**3. Permissions infrastructure.** Collison put it plainly: *"When you get into a bigger company, the permissions engine of who can access this data needs to be rewritten."* This is unglamorous, foundational work. It doesn't show up in a product demo. But without it, agents operate in a degraded environment — they can see some things and not others, and the seams show.

**4. Role redefinition.** The traditional boundaries between Engineering, Product, and Design are dissolving. Organisations haven't updated their job architecture, their hiring profiles, or their performance frameworks to reflect this. People are operating with old maps.

**5. Change management.** This is the one most leadership teams underestimate. Pichai described adoption moving in "concentric circles" — and understanding what that actually means clarifies why broad deployment is harder than it looks.

---

## What "Concentric Circles" Actually Means

Google didn't mandate AI adoption from the top down. It spread it from the inside out — starting where the technical density was highest and letting it diffuse outward.

The first circle was engineering. Google's internal tool — codenamed "Jet Ski," built by their Antigravity team — gave software engineers an agent-manager workflow: instead of writing code directly, engineers orchestrate agents that write, test, and deploy, with the human acting as reviewer and director rather than implementer. Pichai rolled this out to the Search team specifically — not as a pilot, but as standard practice.

The second circle, quieter and more telling, was SRE — Site Reliability Engineering. These are highly technical people doing a mix of reactive work (fixing things when they break) and proactive work (building systems to prevent breakage). What they found, once they had agent tools, wasn't that AI replaced their jobs. They started seeing *automated workflow opportunities they'd never had the bandwidth to pursue before*. Toil they'd accepted as unavoidable became automatable. Monitoring that required human eyes became agent-delegable. The role didn't disappear — it upgraded.

This is the concentric circle pattern: AI capability spreading outward from the highest technical density toward the rest of the organisation. Engineering first. Then adjacent technical functions. Then — Pichai's explicit prediction — non-engineering processes in 2027.

The implication is precise. If you're waiting for AI to be "ready for everyone," you're misreading the diffusion model. It doesn't arrive everywhere at once. It starts where technical fluency is highest, generates proof points, and then the challenge shifts from "does this work?" to "how do we move the next circle?" Google is two years into that diffusion. Most enterprises haven't started the first circle.

---

## What the Companies That Have Crossed Look Like

ElevenLabs is the most concrete public model of an AI-native organisation at meaningful scale — 470 people, $450M ARR run rate, and a structure that looks nothing like a conventional company of that size.

The org is flat in a way that would make most management consultants uncomfortable. Both Staniszewski and his co-founder carry 15+ direct reports — versus the conventional 6–8. Teams are ~10 people, organised around outcomes rather than functions. Decision-making is fast because the hierarchy is thin.

But the structural detail that matters most is this: **every team has a technical resource embedded directly in it.** Not a liaison from IT. Not a shared services queue. A person sitting inside finance, inside talent, inside go-to-market, who understands the domain *and* can automate workflows, build internal tools, and upskill their teammates.

Staniszewski took this model from an unlikely source: Ukraine's DIIA platform — one of the most sophisticated digital government systems in the world, built at extraordinary speed. DIIA's approach wasn't to centralise all technical work in a single "digital team." Every ministry had its own technical staff embedded directly in the function — a health ministry tech lead, a benefits ministry tech lead, each deeply understanding their domain. The central DIIA layer set standards, assembled systems, and connected the pieces. The intelligence lived at the edges; the coordination lived at the centre.

At ElevenLabs, that model produces a company where AI adoption doesn't require a top-down mandate — because the capability is already distributed. Every function can move at the speed of the technical person inside it.

This is the opposite of how most enterprises approach AI: stand up a central "AI Centre of Excellence" and have everyone file requests. That model creates a bottleneck at exactly the moment you need speed. The DIIA model creates a network.

---

## The 2027 Deadline

Pichai was explicit: 2026 is engineering. 2027 is when non-engineering processes shift.

Staniszewski's land-and-expand data corroborates it. The enterprise pattern runs 12–18 months per department. Deutsche Telekom started with marketing, moved to customer support, and is now expanding to network-wide agents. Ukraine's DIIA covered benefits, then healthcare booking, then frontline information delivery. Companies starting their first deployments in customer support now will hit finance, HR, and operations in 2027.

The concentric circles, applied to enterprise timelines, converge on the same date from two directions.

---

## The Pricing Signal

One more confirmation that the old model is broken: every AI infrastructure layer is converging on consumption pricing simultaneously.

ElevenLabs shifted from subscription-only to pay-as-you-go this year. Their newest models are offered at cost — deliberately subsidised to drive adoption and show the world what's possible. Salesforce replaced seats with Flex Credits. Anthropic moved Claude Enterprise to consumption-based charges.

This isn't coincidence. It reflects the same underlying reality: in an agent-native world, value is created by *usage*, not by *access*. The fixed-cost mental model for software — pay for seats, budget predictably, approve headcount — is structurally misaligned with how AI actually delivers value.

Pichai spends a dedicated hour a week tracking compute allocation at a granular level across teams and projects. Compute budgets now rival headcount as a resource constraint at Google. For most enterprises, that's a foreign concept. It won't be for long.

---

## The Honest Take

Most enterprises are treating AI adoption as an IT project. The companies that have crossed the line are treating it as an organisational redesign — permissions infrastructure, data architecture, job structure, culture, and pricing model all changing together.

The technology is not the hard part. It hasn't been for at least a year.

The hard part is being honest that the blocker is internal. That the permissions engine needs rebuilding. That the job architecture is outdated. That a central AI team filing requests is not a strategy. That the concentric circles need to start somewhere, and that somewhere needs to be now.

Pichai said something that lands: *"You can paralyse yourself thinking 10 years ahead when the curve is steep. Focus on next year."*

For most leadership teams, next year is already late.

---

*Sources: Sundar Pichai interview, Cheeky Pint Substack. Mati Staniszewski interview, Cheeky Pint Substack.*
