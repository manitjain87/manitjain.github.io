# Ai, Honestly — Source Intelligence Reference

A persistent knowledge base of frameworks, data points, and insights from primary sources.
Used to inform and ground blog posts. Always cite the original source when referencing in posts.

---

## Interview: History & Future of AI at Google (Sundar Pichai)
**Source:** Cheeky Pint Substack — https://cheekypint.substack.com/p/the-history-and-future-of-ai-at-google

### Enterprise AI Adoption Barriers (via John Collison / Stripe)
Five structural blockers to enterprise AI deployment — not capability gaps, organisational gaps:
1. **Prompting skill gap** — engineers must develop domain-specific prompting expertise; generic prompting underperforms
2. **Codebase collaboration** — high code churn and "blast radius" of AI-generated changes makes sharing hard
3. **Data access bottlenecks** — agentic workflows require clean data pipelines; most enterprises don't have them
4. **Permission infrastructure** — "When you get into a bigger company, the permissions engine of who can access this data needs to be rewritten"
5. **Role redefinition** — traditional Eng/PM/Design boundaries may merge; orgs haven't caught up

### The "Concentric Circles" Adoption Model (Pichai)
- Some groups shifting profoundly now; broader diffusion requires change management
- **2027 expected as inflection point for non-engineering processes**
- "This year, the curve is shifting pretty dramatically" — 2026 is engineering; 2027 is everyone else
- Internal Google: GDM and SWE groups already using agent-manager workflows ("Jet Ski")
- SRE teams discovering automated workflow opportunities within existing roles

### Capital Allocation as New Constraint
- Compute budgets now rival headcount as resource constraint
- Pichai spends "a dedicated hour a week thinking about compute allocation at a pretty granular level"
- Cloud commitments are sacrosanct; forward planning solves most allocation conflicts
- Google CapEx: $30B → $175–185B (600% increase in a few years)
- Memory is "one of the most critical components now" — physical bottleneck alongside power/electricians

### AI as Orchestration Layer
- "The bigger the product surface area, the more that benefit hits" — AI solves navigation complexity
- GCP/MCP integration: AI programmatically interacts with cloud services
- Search becomes "an agent manager" — agentic search combining task completion with information-seeking
- Visceral internal example: executives using agents for business intelligence ("What did people think about this? Tell me the worst/best five things")

### Data Points
- Google Search latency improved 30% over 5 years despite major feature additions
- Gemma 4 (open-source): 90% capability of pro models at "USB stick" scale
- CapEx growth: 600% over a few years
- Waymo investment increased when "rest of world got pessimistic" — contrarian long-term conviction

### Pichai's Visceral AI Moments (for humanising posts)
- 2012: Jeff Dean's Google Brain cat recognition demo
- 2014: DARPA autonomous vehicle challenge observation
- Recent: agents completing complex tasks without supervision; coding where programming language becomes irrelevant detail

---

## Interview: The World of Voice AI with Mati Staniszewski (ElevenLabs)
**Source:** Cheeky Pint Substack — https://cheekypint.substack.com/p/the-world-of-voice-ai-with-mati-staniszewski
**Company context:** ElevenLabs — $350M ARR end-2025, $100M net new ARR in Q1 2026, $11B valuation, 470 employees

### The AI-Native Org Design (ElevenLabs Model)
- **Flat structure:** CEO and co-founder both have 15+ direct reports (vs. traditional 6–8)
- **470 employees in ~10-person teams** — small, autonomous, outcome-focused
- **Every team has a technical resource/"tech lead"** — ops, talent, GTM — who automates workflows and upskills team
- Inspired by **Ukraine's DIIA digital transformation model**: ministries had technical staff; central layer assembled systems
- "Agency" is the cultural differentiator — "high-agency people amplified by AI tools"
- Four culture pillars: first principles thinking, ownership/agency, excellence with humility, fun

### The Enterprise AI Adoption Pattern
- **Land-and-expand motion**: start in one department, prove value, spread org-wide
- Deutsche Telekom: started marketing → customer support → network-wide agent
- Ukraine DIIA: benefits, healthcare booking, frontline information delivery
- Self-serve provides feedback loop on technology quality and surfaces future use cases
- Enterprise customers prefer **cascaded** (speech-to-text → LLM → TTS) over speech-to-speech for **visibility** into decision-making

### The Deployment Gap
- Technology exists; companies haven't integrated it — "automotive OEMs lagging" despite voice being ready
- Quality barrier only cleared ~3 years ago — recency advantage in production systems
- Customer support agents already pass the voice Turing test; open-ended conversation still far away
- Timeline of progress:
  - Quality voice narration: 3 years ago
  - Real-time versions: 2 years ago
  - Production-ready with context: 1 year ago
  - Cloud-based automotive: 2026
  - Offline/in-car: 2–3 years away

### Pricing Evolution (mirrors Salesforce/enterprise AI broadly)
- Shifted from subscription-only to pay-as-you-go / usage-based billing
- Newest models offered at cost to encourage adoption — "subsidise usage to show the world what's possible"
- Per-token for TTS, per-minute for voice agents/transcription
- Early adopters get attractive economics at trial stage to demonstrate value

### The "Voice Turing Test" Problem
- Text LLMs passed Turing test years ago; voice agents haven't yet
- Missing: robust turn-taking, context persistence, tool orchestration
- Three layers required: speech-to-text + turn-taking mechanism + response generation/execution
- Key challenge: when to stop listening vs. waiting for clarification vs. responding immediately

### Data / Business Metrics (ElevenLabs)
- $350M ARR (end-2025) → ~$450M+ (Q1 2026 run rate after $100M net new ARR)
- 50%+ sales-led enterprise business
- 470 employees; ~10-person team structure
- $500M raised at $11B valuation
- Voice models: "a few billion to tens of billions" parameters (vs. hundreds of billions for leading LLMs)

### Second-Order Effects Worth Tracking
- Polish TV dubbing: replacing poor single-voice-over with high-quality AI alternatives
- Guinness Index (Guinndex): agents calling pubs for price data and business reporting
- Lead capture: voice agents increase form completion and openness to complex use cases
- Voice accessibility: restoring voices for ALS/throat cancer patients

---

## Cross-Interview Frameworks

### The Capability-Adoption Gap
Both interviews confirm the same dynamic: **the bottleneck is not AI capability, it's deployment readiness**.
- Pichai: permissions infrastructure, data access, role redefinition
- Staniszewski: automotive OEMs know voice is ready but haven't integrated; enterprises land then expand slowly
- The gap is organisational, not technical

### The 2027 Inflection Point
- Pichai explicitly: non-engineering process automation accelerates in 2027
- Staniszewski implicitly: enterprise adoption patterns suggest 2026 is customer support/marketing; 2027 is ops/finance/HR
- **For CFO/finance audiences**: 2027 is when the budget and headcount implications become unavoidable

### AI-Native vs. AI-Augmented
- AI-augmented: add AI tools to existing structures (most enterprises today)
- AI-native: design the org around AI from the ground up (ElevenLabs, Meta Reality Labs pods)
- The ElevenLabs model is the most concrete public example of what AI-native looks like at 470 people
- Key structural markers: flat hierarchy, tech lead in every function, 10-person pods, high-agency culture

### The Consumption Pricing Convergence
- ElevenLabs: shifting from subscriptions to usage-based
- Salesforce: seats → Flex Credits
- Anthropic: Claude Enterprise shifting to consumption
- Pattern: AI infrastructure pricing converges on consumption models as value shifts from access to usage

---

## Tags / Themes for Future Posts
- `#adoption-gap` — capability vs. deployment readiness
- `#ai-native-org` — flat structure, tech leads, 10-person pods
- `#consumption-economics` — seat → usage pricing shift
- `#2027-inflection` — non-engineering process automation
- `#capital-allocation` — compute as new headcount
- `#voice-ai` — ElevenLabs, turn-taking, Turing test
- `#enterprise-expansion` — land-and-expand, Deutsche Telekom, Ukraine DIIA
