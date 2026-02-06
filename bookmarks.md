# Thursday, February 5, 2026

## @QwQiao - Compute Demands Reshape Investment Thesis
> Once in a while i get better investment ideas from doing than from reading. Case in point after a month of coding i bought more hyperscalers and semis. AMZN MSFT NVDA TSM the whole 9 yards. The market is completely unprepared for how much compute will be needed.

- **Tweet:** https://x.com/QwQiao/status/2019395154197770472
- **What:** Personal investment thesis derived from hands-on coding experience, revealing that market participants are underestimating the magnitude of compute infrastructure needed, leading to increased positions in hyperscalers and semiconductor companies.

## @zephyr_z9 - Memory Shortage Extends to 2028, Capex Revisions Continue
> Memory shortage is worse and will extend into 2028. We got big CAPEX revisions. The easiest way to make money is to bet on memory rn.

- **Tweet:** https://x.com/zephyr_z9/status/2019415216950587485
- **What:** Analysis of semiconductor market dynamics showing memory constraints persisting through 2028 with major capital expenditure revisions, positioning memory chip investments as the most direct profit opportunity.

---

# Wednesday, February 4, 2026

## @profplum99 - Trump administration policy alignment perspective
> This might as well be my position piece on the current administration. Spot on with how I see it

- **Tweet:** https://x.com/profplum99/status/2019000327194759479
- **Article:** https://macdonaldlaurier.ca/what-if-trump-is-painfully-right-stephen-nagy-for-inside-policy/
- **What:** Michael Green's endorsement of an article examining potential validity in Trump administration policies. The linked piece from Macdonald-Laurier Institute explores contrarian perspectives on current political direction.

## @thdxr - Tooling gaps persist despite AI code generation capabilities
> even with infinite ability to produce code we still have long standing tooling gaps\n\nthis was a major one (i even had a poc named openworkflow i never shipped)\n\nwhat's funny is it's getting buried under all the ai talk

- **Tweet:** https://x.com/thdxr/status/2019062073552941109
- **What:** Observation on persistent infrastructure and tooling gaps in development workflows that remain unsolved despite advances in AI-powered code generation. References the author's abandoned OpenWorkflow project as an example.

## @RHouseResearch - SentinelOne's Agentic Evolution and Platform Expansion
> I'm riding with Citron here on SentinelOne $S. Trading sub <4x ARR vs. 20x+ for its closest comp $CRWD, despite both growing topline at 22-23%. I struggle to see SMBs (SentinelOne $S plays more down-market) deciding to build in-house security solutions with vibe-coding tools. $S already seeing decent traction with their agentic offering PurpleAI (essentially a security operations workflow solution) reaching a record 40% attach rate on all licenses sold last quarter. ARR per customer also at a record high while non-endpoint (endpoint being the company's core product) bookings were 50% of total bookings last quarter. Both data points suggest company is evolving from endpoint point solution to broad security platform.

- **Tweet:** https://x.com/RHouseResearch/status/2019088197066645741
- **What:** Analysis of SentinelOne's valuation relative to competitors and evolution from an endpoint security vendor to a comprehensive security platform, highlighting PurpleAI's 40% attach rate and record ARR per customer as indicators of platform diversification.

## @sdand - vmux: Stateful Cloud Sandboxes for Coding Agents
> Introducing vmux - incredibly fast, stateful cloud sandboxes for coding agents. For the first time you get persistent GPU/CPU sandboxes via Modal/CF backed by Durable Objects to stream logs live, native preview URLs, and attach a real shell. Spin up a notebook or train nanogpt via codex - with a Modal sandbox spun up in seconds.

- **Tweet:** https://x.com/sdand/status/2019183574516195703
- **What:** Introduction to vmux, a new tool providing persistent GPU/CPU sandboxes for AI coding agents with live log streaming, preview URLs, and shell access, leveraging Modal and Cloudflare Durable Objects for fast deployment.

## @cajunpies - Semiconductor and Infrastructure Spending Priorities
> @felipexbt @zephyr_z9 $TSM $AVGO $VRT $FIX $HUBB $ANET $ETON $GEV $MU $STX $SNDK $ONTO $KLAC $ASML to name a few

- **Tweet:** https://x.com/cajunpies/status/2019265497175388346
- **What:** Response listing multiple semiconductor and infrastructure companies (TSM, AVGO, MU, ASML, KLAC and others) as beneficiaries of major compute spending initiatives, indicating where AI infrastructure investment is flowing.

---

# Tuesday, February 3, 2026

## @alxfazio - Building Fleet of Vertical Agents with Fly.io Infrastructure

> i'm building a fleet of vertical agents where each one gets its own full computer (100gb persistent disk, 8gb ram, ~600ms wake from hibernation) using Fly.io sprites and Z.ai glm 4.7. they're built entirely on claude code cli, no openclaw and no claude agent sdk. `claude --print` (non-interactive mode) is what makes this possible. the hatcher sends a prompt, claude code runs headlessly on the sprite, and streams structured json back. you can talk to them from discord or drop into a terminal and pick up the same session from anywhere

we call them droids. Fly.io sprites give them ~$0 compute when idle and auto-hibernate after 30 seconds of inactivity. when a user sends a message, the sprite wakes in ~600ms and picks up right where it left off. they'll be hatchable from a base config using what i call a "droid hatcher," similar to botfather on telegram

we were already building useful vertical agents with claude code, but we're all busy and travel a lot. having to sit down in front of a laptop and open a terminal just to use claude code (because the app and claude.ai don't have the same toolset) was creating a lot of friction. creating a new agent was an entire project. sharing one meant pushing to github, sharing the repo, pulling updates. group chats with claude code didn't exist, you couldn't have multiple people talking to the same agent in isolated threads. with this setup anyone in the company can hatch a new droid directly from discord using the droid hatcher, share it with others, or co-work on one together, all in full safety

i wanted something like openclaw for my business, but openclaw is too opinionated. it abstracts away too much of the claude code configuration, which kills customisation and portability. it would also force me to rewrite the claude code setups we already share across employees. and the agent sdk is too high-level for what i need. i want each droid to own its entire machine, not run inside someone else's runtime. because these are full claude code instances on isolated vms, the agents can self-improve, self-edit their own code, and their machines are fully auditable. we can ssh in and inspect anything at any time

this system solves all three problems. each droid is its own machine (no git pull needed), lives in a discord forum channel where each post is an independent session, and multiple people can interact with it concurrently

i can already resume a droid's session from a terminal whenever i want, instead of going through discord. their main home will be a dedicated discord server. i chose discord because i used midjourney a lot and i know what's possible on discord in terms of ux for bot-driven workflows. it also avoids dumping noise into our main slack channel, but they'll still be mentionable from slack when needed

anyone in my company will be able to create and customise their agent, all from a single chat. new people, collaborators, and contractors can be onboarded safely in discord, since each droid lives in its own forum channel and permissions are managed directly through discord roles. no complex business logic needed. contractors can even bring their own api key and hand it to the droid hatcher to spawn a droid they pay for, while still working transparently inside our org

the system supports third-party model providers like Z.ai for tasks that don't need frontier intelligence. glm 4.7 is fast and cheap enough for most vertical agents. this also matters because anthropic has been banning accounts that use their max subscription inside third-party wrappers, and running through a separate api provider means your anthropic account stays clean

i think this is a better and safer version of both claude cowork and openclaw. each droid has its own isolated vm. not a shared sandbox, not a container, a full machine. if something goes wrong, you restore the entire machine from a previous checkpoint. no need to buy a mac mini just to feel safe, and no risk of an agent messing with your actual computer

this is probably the most fun llm project i've worked on so far. right now i only have a working slack prototype, but the signs are all there, and it has me genuinely excited. the full system with discord forum channels, the droid hatcher, and session forking is what's coming next. i already have a full design spec for the discord system and i'll share it when the time is right. i'll keep posting updates as it takes shape

if i could, i'd invest in Fly.io, because they've built an incredible solution for what i think is the future of agents.

- **Tweet:** https://x.com/alxfazio/status/2018744471857279438
- **What:** Detailed architecture for building "droids" - vertical agents with isolated VMs on Fly.io infrastructure, controlled via Discord, using Claude Code CLI in headless mode for cost-effective and customizable AI agent deployment.

## @nicopreme - Pi-Web-Access Update with Video Understanding

> Updated pi-web-access for Pi agent with video understanding. If you're signed into Gemini in Chrome, no API keys needed for web search or video analysis. Point it at any YouTube URL or local video file (mp4, mov, etc) and ask questions about the content.

pi install npm:pi-web-access
https://t.co/dw92Ir4wMT

- **Tweet:** https://x.com/nicopreme/status/2018796776807968834
- **What:** Update to pi-web-access tool adding video understanding capabilities to Pi agents. Enables video analysis via Gemini integration without requiring API keys for YouTube URLs or local video files.

## @jxnlco - Open Sourcing RAG and Consulting Material

> open sourcing some of my rag and consulting material https://t.co/T0yC4tAZ4T

- **Tweet:** https://x.com/jxnlco/status/2018807746590879840
- **What:** Jason Liu announces open sourcing RAG (Retrieval-Augmented Generation) techniques and consulting materials from 567 Labs work, making these research foundations available to the community.

## @TheBenSchmark - Anthropic Market Commentary

> JPMorgan: Anthropic is eating the world

Jabroni: Buy $ZM https://t.co/inQMP1fLDx

- **Tweet:** https://x.com/TheBenSchmark/status/2018820666456465717
- **What:** Humorous market commentary juxtaposing JPMorgan analysis on Anthropic's market dominance with a contrarian take suggesting zoom stock ($ZM) purchases instead.

## @sarahdingwang - ServiceNow trading valuation amid ARR acceleration
> Case in point: ServiceNow guided to "accelerating net new ARR at huge scale" last week.\n\n…currently trading at 16x FCF, down another 7% today

- **Tweet:** https://x.com/sarahdingwang/status/2018829257745772881
- **What:** Commentary on ServiceNow's valuation metrics and market performance despite strong guidance on ARR acceleration. Reflects broader market uncertainty in SaaS valuations.

## @jessfraz - AI parenting challenges in Claude development
> just having to undo all the bad parenting decisions of your maker my little buddy

- **Tweet:** https://x.com/jessfraz/status/2018864645721973065
- **What:** Humorous observation on the challenges of refining AI models and correcting upstream design decisions in Claude's development process.

## @cremieuxrecueil - Medical advice summary from the past year
> Summary of the past year:\n\n- GLP-1s are great\n- Everyone should be on a statin or other anti-cholesterol drug\n- Slather your wounds in Aquaphor\n- Zinc tablets and saline nasal spray when you get colds\n- Laser eye surgery Just Works\n- Your medication allergies are probably fake

- **Tweet:** https://x.com/cremieuxrecueil/status/2018907830934253614
- **What:** Practical medical advice summary covering preventive health measures (GLP-1s, statins), treatment recommendations, and a commentary on overdiagnosed allergies based on the past year's trends.

---

# Monday, February 2, 2026

## @trajektoriePL - OpenAI Lawsuit Reveals Jakub Pachocki's Breakthrough Role

> What did Ilya see? He saw his own protégé Jakub Pachocki achieve the breakthroughs that had eluded him for years.

Newly released documents from the Musk v. Altman (2026) lawsuit provide a rare look at the resentment that fueled the OpenAI crisis. In November 2023, Microsoft CTO Kevin Scott explained the situation to Satya Nadella:

,,Jakub moreso than Ilya has been making the research breakthroughs that are driving things forward, to the point that Sam promoted Jakub, and put him charge of the major model research directions. After he did that, Jakub's work accelerated, and he's made some truly stunning progress that has accelerated in the past few weeks. I think that Ilya has had a very, very hard time with this, with this person that used to work for him suddenly becoming the leader, and perhaps more importantly, for solving the problem that Ilya has been trying to solve the past few years with little or no progress. Sam made the right choice as CEO here by promoting Jakub."

Source @TechEmails @ColinWPLewis

- **Tweet:** https://x.com/trajektoriePL/status/2018242446577086589
- **What:** Newly released court documents from the Musk v. Altman lawsuit expose internal tensions at OpenAI, showing how Microsoft CTO Kevin Scott attributed a major management shift (promoting Jakub Pachocki over Ilya Sutskever) to genuine technical capability differences and research breakthroughs.

## @WillManidis - Twitter Article Link

> https://t.co/qNAVuG3xsz

- **Tweet:** https://x.com/WillManidis/status/2018318844247347308
- **What:** A single link to a Twitter article (content not available in metadata).

## @zephyr_z9 - AI Semiconductor Bottlenecks and Stock Performance Analysis

> A stock going up by 1500% in a year is extremely rare
But we have covered a wide range of bottlenecks in the semis memo

- **Tweet:** https://x.com/zephyr_z9/status/2018360288152842663
- **What:** Commentary on semiconductor sector stock performance and industry bottlenecks, referencing a comprehensive memo on semiconductor supply chain challenges and emerging trade opportunities in AI semis.

## @ContrarianCurse - Early Cycle Industrial Sector Positioning

> Increasingly clear that we are early cycle. I'm 20% OW industrials in the fund - by far my biggest bet of any sort, even more consequential than semicap

Admin, despite their lunacy, deregulating and letting business rip + fiscal bonanza + cuts flowing through + AI cap cycle=hot

- **Tweet:** https://x.com/ContrarianCurse/status/2018367351888945166
- **What:** Investment perspective highlighting an early market cycle with emphasis on industrials sector overweighting, citing regulatory deregulation, fiscal stimulus, cost management, and AI capital cycle as key drivers.

## @testinprodcap - Investment Strategy Insight

> the secret is to ignore citrini's ridiculous 100 asset multi-country portfolio and just full port into stuff he writes a full post about.

- **Tweet:** https://x.com/testinprodcap/status/2018448486912450970
- **What:** A brief take on investment strategy, suggesting focusing on investments where there's in-depth published analysis rather than complex multi-asset portfolios.

---

# Sunday, February 1, 2026

## @TheBenSchmark - Anthropic IPO and Early Investment Opportunity
> Great points by @Citrini7. Anthropic might be the largest company ever to IPO, most of the public won't participate, but indices will be forced to buy.

- **Tweet:** https://x.com/TheBenSchmark/status/2018014595911237784
- **Tags:** [[anthropic]] [[investing]]
- **What:** Investment observation about Anthropic's potential IPO with commentary on market participation and index fund dynamics.

## @nbaschez - Test-Driven Bug Fixing in Claude Code
> Single biggest improvement to your Claude Code docs / AGENTS.md: "When I report a bug, don't start by trying to fix it. Instead, start by writing a test that reproduces the bug. Then, have subagents try to fix the bug and prove it with a passing test."

- **Tweet:** https://x.com/nbaschez/status/2018027072720130090
- **What:** Suggestion for improving Claude Code workflows and AGENTS.md documentation by emphasizing test-driven development for bug fixes, which provides proof of resolution and prevents regression.

## @doodlestein - Learning Through Interactive Phage Genome Visualization
> I find the best way to avoid this is to pick a completely foreign topic that interests me, but which I know almost nothing about, and then try to go super deep via free-form discussions with frontier models where I just ask about whatever I think of and posit ideas.

- **Tweet:** https://x.com/doodlestein/status/2018050324620276059
- **What:** Shares a learning methodology combining frontier model discussions with interactive educational webapp development, citing their phage genome visualization project as an example of teaching to learn and creating shareable artifacts.

## @badlogicgames - Avoiding Productivity Burnout Through Focused Context Management
> This is a very nice description of the problem. I think the first part of the solution is to not give into the hyper productivity hype: running a gazillion things in parallel.

- **Tweet:** https://x.com/badlogicgames/status/2018117758991384754
- **Tags:** [[productivity]] [[context-switching]] [[mental-health]]
- **What:** Mario Zechner discusses cognitive limits of parallel task management, recommending limiting simultaneous projects to 2-3 items and using virtual desktops to manage context boundaries for optimal productivity and code quality.

## @nicopreme - Pi MCP Adapter: Token-Efficient MCP Tool Loading

> Updated pi-mcp-adapter to be even more flexible: it still progressively loads MCP tools by default (install as many as you want with no token bloat), but now you can promote any specific MCP tool/s to first-class via a TUI panel so they always load immediately on session start and tool descriptions appear alongside core tools.

Also updated the pi-subagents extensions so that can any custom subagent definition can be configured to load specific MCP tools immediately as first-class tools.

- **Tweet:** https://x.com/nicopreme/status/2018231492095115642
- **What:** An update to pi-mcp-adapter enabling flexible MCP tool loading with optional promotion to first-class tools via TUI, plus corresponding updates to pi-subagents for subagent-specific MCP tool configuration. Addresses token efficiency in MCP tool management.

---

# Saturday, January 31, 2026

## @nicopreme - Pi Annotate: Browser Element Selection for AI Agents
> Just shipped a Chrome/Pi extension that lets you click on elements in your browser like the web inspector + add comments and your agent receives selectors, CSS and screenshots.

- **Tweet:** https://x.com/nicopreme/status/2017511465310167492
- **What:** A Chrome extension that enables visual annotation of web elements with an inspector-like interface. Agents receive detailed context including selectors, CSS, box model, accessibility info, and element screenshots.

## @mweinbach - Echo 13 Thunderbolt 5 SSD Dock with Built-in Storage
> @ryanvogel yup, but the thunderbolt dock is expensive and it depends on which macbook you have

This needs Thunderbolt 5 but is outstanding and there's a version with an included SSD

- **Tweet:** https://x.com/mweinbach/status/2017612681012797715
- **What:** A reply discussing the Echo 13 Thunderbolt 5 SSD Dock - the industry's first shipping Thunderbolt 5 dock with integrated PCIe 4.0 NVMe SSD storage and comprehensive connectivity including 10Gbps USB, 2.5GbE, and 140W power delivery.

## @samswoora - Build Infrastructure and Development Workflow Tools
> @deepfates Bazel or Buck2, remote build farm, stacked diffs, merge queues etc etc

- **Tweet:** https://x.com/samswoora/status/2017675071960056146
- **What:** A technical discussion mentioning build system tools (Bazel, Buck2), remote build infrastructure, stacked diffs, and merge queue systems for managing complex build and deployment workflows.

## @WillManidis - Market Underpricing of Legacy Software Companies with Token Businesses
> its amazing to me how little the market has priced in the slosh of random, mid-cap legacy software companies that are sitting on net-profitable token and RL generation businesses.

- **Tweet:** https://x.com/WillManidis/status/2017689664702808189
- **What:** A market observation about legacy software companies that have added profitable token generation and reinforcement learning capabilities being undervalued by the market.

## @JoannisOrlandos - LLM-Assisted Coding with Feedback Loop and Skill-Based Linting
> The past two weeks I've hit a new level with LLM-assisted coding. Found a feedback loop: define code standards → add as Skills → have Claude turn them into linter rules. The code quality is incredible.

- **Tweet:** https://x.com/JoannisOrlandos/status/2017708681551335445
- **What:** A technique for improving LLM-generated code by creating a feedback loop: establish code standards, encode them as Claude skills, then convert those standards into automated linter rules to maintain quality consistency.

## @doodlestein - Planning Process for Multi-Stage Software Development
> It's a multi-stage process. Look at the git history for that plan and you'll see all the earlier incarnations.

- **Tweet:** https://x.com/doodlestein/status/2017776439173546419
- **Tags:** [[planning]] [[software-development]] [[claude-code]]
- **What:** Reply to AnonymousQuant explaining a multi-stage planning approach, with detailed quotes about using ChatGPT 5.2 with extended reasoning to review markdown plans, then converting those plans to "beads" (tasks/epics with dependencies) for coding agent implementation via Claude Code.

---

# Friday, January 30, 2026

## @rudrank - Cursor /council Command for Multi-Agent Exploration
> It is time to invoke the council

- **Tweet:** https://x.com/rudrank/status/2017157759880613929
- **What:** Rudrank highlighting Cursor's /council command, which spawns multiple agents to deeply explore a codebase area before acting. Useful for comprehensive code analysis before making changes.

## @GuidoVranken - Coinbase MPC Library Security Vulnerabilities
> Coinbase partying like it's 1999. Let's use OpenSSL for BN but then also roll a custom modinv by fucking with ossl internals. Mix and match ossl and libsecp256k1. Don't check return values cos it's fine. Maybe it's all accidentally secure but I wouldn't count in it, good luck.

- **Tweet:** https://x.com/GuidoVranken/status/2017217560320548889
- **What:** Security researcher Guido Vranken critiques Coinbase's MPC library for mixing OpenSSL and custom code without proper error checking, creating potential security vulnerabilities.

## @joesadoski - Logging Costs Reduction Skill
> This skill cut my logging costs and made my logs actually usable. Adapted from @boristane's "Logging Sucks". I'm trying to run this on any code we have running in prod now.

- **Tweet:** https://x.com/joesadoski/status/2017230282588340233
- **What:** Joe Sadoski shares a Cursor skill (adapted from boristane's work) that significantly reduced logging costs while improving log usability. Planning to apply it across production code.

## @gannonbreslin - Trump nominates Kevin Warsh as Fed Reserve Chair

> It's staring right at you for the taking

- **Tweet:** https://x.com/gannonbreslin/status/2017264711776260122
- **What:** Quoted tweet about Trump's nomination of Kevin Warsh as Federal Reserve Chair, emphasizing Warsh's connection to the Lauder family and potential influence implications.

## @greg_price11 - DOJ FACE Act arrests for hymn singing outside abortion clinic

> Reminder that Biden's DOJ arrested all of the people in this video under the FACE Act for singing hymns outside an abortion clinic.

According to the left, this was a legitimate use of the FACE Act, but not disrupting a church service.

- **Tweet:** https://x.com/greg_price11/status/2017283545387909251
- **What:** Commentary on the Biden administration's use of the FACE Act to arrest protesters singing outside abortion clinics, highlighting perceived inconsistency in enforcement of the law.

## @AviFelman - Rare earth minerals and uranium opportunity amid precious metals speculation

> Silver and Gold may collapse in speculative mania, but it's giving you the opportunity to acquire rare earth minerals and uranium. Both of which have strong fundamental drivers, and are being unfairly dragged around by the metals frenzy.

- **Tweet:** https://x.com/AviFelman/status/2017310810184282274
- **What:** Investment perspective on how precious metals speculation creates opportunities in rare earth minerals and uranium, which have stronger fundamental drivers independent of metals market fluctuations.

## @antirez - Claude Code with Codex skill integration for enhanced problem-solving

> If you explain how to do it, Claude Code is able to use Codex when it is incapable of solving certain issues. This way you have the best of both worlds.

Here is the skill file that lets Claude use Codex.

- **Tweet:** https://x.com/antirez/status/2017314325745086771
- **Knowledge file:** [[claude-codex-skill]]
- **What:** Demonstration of a skill file that enables Claude Code to leverage Codex for edge cases where Claude alone struggles, combining the strengths of both systems.

## @davis7 - Vercel's just-bash package for agent customization

> The "just-bash" package is the best thing @vercel has shipped in a long time

Insanely useful for custom agent stuff

- **Tweet:** https://x.com/davis7/status/2017332165634363839
- **What:** Enthusiastic endorsement of Vercel's just-bash package as highly valuable for building custom agent functionality, highlighting its practical utility.

---

# Thursday, January 29, 2026

## @dillon_mulroy - Overseer: Task Orchestration for AI Agents via MCP
> not really ready for other people to use but if you're interested https://t.co/D7uA4A2iOB

- **Tweet:** https://x.com/dillon_mulroy/status/2016910878252089390
- **What:** Overseer is a task orchestration system for AI agents using MCP. It provides SQLite-backed task management with native VCS support (jj-lib and git). Features include task hierarchies (milestones/tasks/subtasks), a codemode MCP server for agents to manipulate tasks programmatically, progressive context inheritance, and learning bubble-up. Available as npm package or skills.sh integration. Early-stage but functional.

## @evanjconral - Request for Product: AI Code Review Tool with Custom Rules
> I think(?) I am the first person who created the concept of "AI code review" as a category, with lintrule.

Lintrule was the first product I was going to pursue when starting this startup, but I ended up abandoning it because Alex wanted to do an AI lab, and I wanted to work with Alex. That startup ended up becoming SF Compute.

With that said, we're now in the position of being a customer for this, and many options have appeared to serve us. And… they all kind of suck?

I really would like this to exist, so I'm writing this as a "request for product" or "request for the current  products to be better". If you have this product that meets the requirements below, please send me a DM (or comment on this thread), and we'll switch to yours. Requirements below…

When an AI code review tool works, it should only speak when something is wrong. Some tools seem to REALLY want to talk and, I swear to god, make a sequence diagram for a "I changed the color of a button" changes. Please shut up.

AI code review tools should not assume they know what we want to review for. Please don't have a "default" check, or if you do, let us turn it off.

Instead, please let me define custom rules, this is the only thing I care about, and I'm confused why people implement this as a "side" feature, when it's the only useful feature of any of these tools. We really ONLY want to check against specific rules. An example rule is "Utc::now() or any analogous "get wall clock time" should be basically banned from rust services. Use a Clock instead. Always dependency inject time." Or "Every rust web service MUST be exposed as:lib rs  with a single spawn_thing(...all_dependencies, cancellation_token) function that spawns the service into tokio."

These rules should be stored in code. One point of us defining rules in the first place is to prevent what we call "sandcastling" (where someone makes a decision, goes to look somewhere else for a bit, and discovers that their critical decision has washed away like a sandcastle, and suddenly everything is breaking & hard to fix). To prevent that, we need controls over who can to approve a rule being changed and when & why a rule was changed. We already have a tool for this: git! Having the rules in the code base is nice because then other AI tools can look at those rules while they're implementing changes, which reduces failures. Please consider letting us use the tool we already use, and if you don't let us do that, at least reimplement RBAC, versions, and approvals in your tool.

Your AI review tool should be available to run locally as a CLI tool or API via MCP. It should be possible for me to tell claude/cursor that "once you're done, ensure it passes XYZ rule" or whatnot. I can run other CI tooling, I should be able to run your review bot.

Your AI review tool should be an agent and be given access to the rest of the code base, and potentially web search or a sandbox to run things in. If it's only working off the diff, it misses a lot.

Your AI review tool should support MCP & let us inject our own context into the reviewer. This is useful for the AI reviewer to get context on RFCs or Linear projects.

If you have a tool like this or are building one, please DM. We'd like to use your tool, we're currently evaluating options.

- **Tweet:** https://x.com/evanjconrad/status/2016964052006949250
- **What:** Evan Conrad (SF Compute) outlines comprehensive requirements for an ideal AI code review tool. Key demands: silence unless problems exist, custom rule definitions stored in git (not SaaS), MCP/CLI availability for local execution, full codebase context access, and proper RBAC/approval workflows. Current tools lack these capabilities. Seeking product recommendations or building partners.

## @zeeg - Sentry CLI Enables AI Agent Interactions
> The new Sentry CLI is here. This wont replace our MCP, but it should create a lot more possibilities for both human and agentic interactions.

- **Tweet:** https://x.com/zeeg/status/2016964850594001397
- **What:** David Cramer announcing the new Sentry CLI designed to work alongside MCPs, expanding possibilities for both developers and AI agents to interact with Sentry's capabilities.

## @ScriptedAlchemy - Options Chain Data MCP Experience
> @MichaelArnaldi @hd_nvim Maybe overengineered? I shat mine out in a weekend and didn't really mess with it after that. Just started working on v2 which isn't the MCP version that I primarily use still. Do you ingest options chain data?

- **Tweet:** https://x.com/ScriptedAlchemy/status/2016967953233957271
- **What:** Chief Wiggum sharing experience building an options trading MCP quickly over a weekend, questioning whether others' MCPs are overengineered and asking about options chain data ingestion.

## @ScriptedAlchemy - Model Comparison for Trading Systems
> @MichaelArnaldi @hd_nvim Okay then setup sounds similar. What model? 5.2 high?

- **Tweet:** https://x.com/ScriptedAlchemy/status/2016968445959831783
- **What:** Conversation thread about trading system architecture where Chief Wiggum inquires about which LLM models are being used (specifically mentioning Claude 5.2 High).

## @ScriptedAlchemy - Data Sources for Trading Analysis
> @MichaelArnaldi @hd_nvim What about SEC reports, financial institutions, scrape news, morningstar reports? How many tokens per instrument you burn?

- **Tweet:** https://x.com/ScriptedAlchemy/status/2016969648215085095
- **What:** Chief Wiggum drilling into the data sources being used for trading analysis (SEC reports, news scraping, etc.) and asking about token consumption per financial instrument.

## @ScriptedAlchemy - Token Economics of Trading Candidate Analysis
> @MichaelArnaldi @hd_nvim Per instrument I think I'll eat about 10 million - 50 million tokens. Light up a datacenter and go through 40 or so candidates

- **Tweet:** https://x.com/ScriptedAlchemy/status/2016971169539510686
- **What:** Chief Wiggum sharing insights into the massive token consumption of their trading system - 10-50M tokens per instrument to evaluate multiple candidate strategies, emphasizing the computational intensity involved.

## @ScriptedAlchemy - Preselecting Trading Candidates with Filters and Data
> @MichaelArnaldi @hd_nvim Various filters and site scraping. Chain data. Momentum. Pull top lists off broker for each industry.

- **Tweet:** https://x.com/ScriptedAlchemy/status/2016973526453108882
- **What:** Discussion of methodologies for preselecting candidates from a large pool using filters, data chaining, momentum analysis, and broker industry lists.

## @thiccyth0t - Bitcoin as Digital Asset in Bits-to-Atoms Rotation
> bitcoin is supposed to be a debasement hedge but it is a digital asset first and foremost amidst a secular rotation from the world of bits into the world of atoms, something thiel has predicted for over a decade https://t.co/p1p63IhXCt

- **Tweet:** https://x.com/thiccyth0t/status/2016994628931617262
- **What:** Analysis of Bitcoin's role beyond inflation hedge, positioning it as a digital asset amid a broader secular shift from digital to physical assets, citing Thiel's predictions.

## @dillon_mulroy - Using Claude to Build Astro Docs Viewer
> life pro tip: ask claude to spin up a temporary @astrodotbuild app for viewing all the markdown docs in your repo you've been generating

- **Tweet:** https://x.com/dillon_mulroy/status/2017017542125003225
- **What:** Productivity tip suggesting using Claude to create a temporary Astro app for browsing generated markdown documentation within a repository.

## @sporadica - Reaction to Nanotechnology Discussion
> how the actual fuck

- **Tweet:** https://x.com/sporadica/status/2017041824393928753
- **What:** Expressive reaction to a quote about nanotechnology and biological complexity.

## @doodlestein - Claude Code Post-Compaction Reminder Tool
> I've been trying for a while to find a reliable way to remind my Claude Code agents to re-read AGENTS .md promptly after every compaction. Otherwise they have a tendency to go rogue and act like wild animals (fortunately, they're at least muzzled wild animals since I'm also using my dcg tool).

Unfortunately, there isn't a clean way to do this now. There would be, but there's a bug that prevents it from working (that clean method is the "SessionStart hook with compact matcher" approach).

So for now, I'm using an ugly workaround that "kind of" works (PreCompact + UserPromptSubmit hooks with marker file).

Anyway, it works well enough that I think it's worth sharing:

https://t.co/Q2HDS3gCdS

Can be installed using a convenient curl bash one-liner like all my tools.

And btw, the other more correct way is done and implemented, and I can switch it on as the default approach as soon as they fix the bug.

- **Tweet:** https://x.com/doodlestein/status/2017087633877278974
- **What:** Tool for preventing Claude Code agents from losing project conventions after context compaction by reminding them to re-read AGENTS.md. Uses a workaround mechanism with hooks and marker files until a bug in Claude Code is fixed.

## @zeeg - Warden: AI Code Review Agents
> @hiproductminds https://t.co/SLFGoCQYcQ - its not ready for use yet. hopefully tomorrow (and ill record a demo/writeup on it)

- **Tweet:** https://x.com/zeeg/status/2017122442448425044
- **What:** David Cramer teasing Warden, a new Sentry tool for agents that review code locally or on every PR. Not yet ready but demo/writeup coming soon.

## @davis7 - Comparing Codex and Opus Agent Capabilities
> Another thing I'm noticing with Codex is it can occasionally get lost in doom loops. Was dealing with a hellish one, and after watching it struggle for like 2 hours I gave up, had it write out what the problem is/what it's been trying to an MD file, then gave it to opus. Opus got it fixed and working in 10 minutes. I really don't know the exact words to quantify the difference between these two, but to do my best: - both are very good and very useful - opus is a smart, accurate, and fast precision instrument that's amazing at solving hard problems - codex is a slower, broader, but more correct agent for building/expanding/designing complex systems without breaking them. Idk if that makes any sense, but I feel like codex is my new default agent, Opus is my "go figure this really hard thing out" agent

- **Tweet:** https://x.com/davis7/status/2017142271418789958
- **What:** Ben Davis contrasts two Claude agents: Codex excels at building/expanding complex systems but can get stuck in loops; Opus is better for solving hard problems quickly. His take: use Codex by default, Opus when precision is critical.

---

# Wednesday, January 28, 2026

## @SilverBulletBTC - Copper Monthly Chart Resistance Breakout
> This is the copper monthly chart\n\nIt just broke above a 20 year resistance \n\nEasy 2x - 5x in the next 12-24 months https://t.co/q7yaMBaZM0

- **Tweet:** https://x.com/SilverBulletBTC/status/2016461741979271254
- **What:** Market analysis of copper breaking above 20-year resistance level, predicting 2x-5x returns over the next 12-24 months. Includes chart image.

## @alexhillman - Claude Code Workflow for Building Tools
> Like almost everything, I start with a goal and have Claude code interview me for the details until it's 90% confident it knows what I want. I tell Claude what I want to be able to do with an app I use, and give it links to their API docs. Ask it to learn the api and ask me questions about my preferences and uses cases (which are now an includes in my interview workflow so I don't have to repeat myself). It takes my answers and provides a recommendation. I tweak or approve. It builds. I review the cli documentation for obvious errors (rare but possible and usually more incomplete than broken). Final step is asking it for a skill. It uses everything so far to crrate a skill reference for using the cli, and provides a mix of scenarios that combine CLI calls, shows examples of sample data and code etc. This is a bunch of steps, but the assistant handles most of the heavy lifting and the utility is compounding. Worth trying yourself to see how it works!

- **Tweet:** https://x.com/alexhillman/status/2016509911962701901
- **What:** Detailed workflow for using Claude Code to build custom CLI tools and skills. Involves goal-setting, API documentation review, interactive questioning, recommendations, and skill generation for reusable automation.

## @jacobmparis - Vercel Composition Patterns Skill Documentation
> @PaulRBerg Split out into here now: https://t.co/6mvHCjkj0L

- **Tweet:** https://x.com/jacobmparis/status/2016516730089292171
- **What:** Documentation for Vercel's composition patterns skill - a reference guide for building flexible React components using compound components, state lifting, and context patterns to avoid boolean prop proliferation.

## @TheIshanGoswami - Exa MCP Web Search Tool
> fyi: exa mcp (web search mcp) is completely free

- **Tweet:** https://x.com/TheIshanGoswami/status/2016528756538826895
- **What:** Note that exa MCP (web search MCP) is available for free, useful for integrating web search capabilities into Claude projects and tools.

## @thorstenball - Amp Launches Deep Agent Mode with GPT-5.2-Codex
> Amp has a new agent mode. It uses GPT-5.2-Codex.

Time to let deep work.

- **Tweet:** https://x.com/thorstenball/status/2016547690960605375
- **What:** Amp introduces "deep" mode for autonomous code work. Unlike "smart" mode's collaborative approach, deep mode reads files and plans for 5-15 minutes before making changes, ideal for complex problems that need deep thinking over constant interaction.

## @benhylak - Code Review App with Live Change Summaries
> yesterday, i built the code review app i've been begging twitter for.

- live streams change summaries as claude code works
- quizzes me about changes before i commit them.
- finds bugs locally -- without having to push to GitHub

- **Tweet:** https://x.com/benhylak/status/2016604696014991810
- **What:** Custom code review application that streams live summaries of changes as Claude Code makes edits, quizzes author before commits, and detects bugs locally. Addresses the productivity bottleneck of code review in development workflow.

## @RyanMorey - OrbStack as Docker Desktop Alternative
> @ChristianSelig If you're new to Docker and don't have a specific reason you need to use Docker Desktop, don't! Use OrbStack!

- **Tweet:** https://x.com/RyanMorey/status/2016618643732209781
- **What:** Strong recommendation for OrbStack as the preferred Docker solution for newcomers and general use. OrbStack provides faster, lighter performance than Docker Desktop without its overhead for typical containerization needs.

## @TheFlowHorse - Market Knowledge Respects Price Action
> Posted something in a similar vein.💪

- **Tweet:** https://x.com/TheFlowHorse/status/2016625146409148771
- **What:** Quote response agreeing with Stanley Druckenmiller's principle that the market knows something and chart patterns deserve respect. Emphasizes the importance of reading price action alongside fundamental analysis.

## @astridwilde1 - AI Capex Spending Strategy
> buying the unterrified AI capex spenders probably works for the next 5 years

- **Tweet:** https://x.com/astridwilde1/status/2016628792928981345
- **What:** Investment thesis suggesting that companies confidently investing in AI infrastructure and capabilities will likely outperform over the next 5-year period as AI adoption accelerates.

## @mert - Reflexivity and Market Instability in Connected World
> you can make a lot of money if you internalize that the world is now ruled by reflexivity

this is a recent shift and a direct consequence of increased connectivity

you first saw this with covid, gamestop, and crypto

but it will infect all asset classes https://t.co/mdZ7oEXgaG

- **Tweet:** https://x.com/mert/status/2016665095691030978
- **What:** Analysis of how increased market reflexivity (driven by connectivity) creates profit opportunities. Notes that gold futures—the safe-haven asset—recently swung $120-100/oz in 20 minutes, exhibiting crypto-like volatility. Signals that reflexive market behavior will spread beyond cryptocurrencies.

## @koylanai - LLM Agent Design: Passive Context Beats Active Retrieval
> Progressive disclosure is not reliable because LLMs are inherently lazy.

"In 56% of eval cases, the skill was never invoked. The agent had access to the documentation but didn't use it."

Vercel ran evals on Next.js 16 APIs that aren't in model training data to test whether agents could learn framework-specific knowledge through Skills vs. persistent context.

Skills are the "correct" abstraction: package domain knowledge, let the agent invoke it when needed, minimal context. The agent decides when to retrieve.

They work well WHEN the user triggers them; otherwise, LLMs just ignore them.

Vercel's benchmarking is the first experiment of this kind I've seen, and it's actually interesting.

- Baseline (no docs): 53%
- Skill (default): 53%
- Skill with explicit instructions: 79%
- AGENTS[.]md with 8KB compressed docs index: 100%

The skill approach assumes agents reliably recognize when they need external knowledge and act on it. They don't.

"You MUST invoke the skill" made agents read docs first and miss project context. "Explore project first, then invoke" performed better. Same skill, different outcomes based on prompting.

The winning approach removed the decision entirely. An 8KB compressed index embedded in AGENTS[.]md, with one instruction: "Prefer retrieval-led reasoning over pre-training-led reasoning."

Two agent design learnings:
1. Passive context beats active retrieval for foundational knowledge. Don't make the agent decide to look things up, make the index always present.
2. Compress aggressively. Vercel went from 40KB to 8KB (80% reduction) with zero performance loss. The agent needs to know where to find docs, not have full content in context.

The gap between "agent can access X" and "agent will access X" is larger than we assume.

I keep seeing similar findings across agent architectures. Kimi Swarm's orchestrator is trained specifically to avoid sequential execution. Without training, orchestrators default to serial processing, planning a list of steps and executing them one by one. It's the EASY path.

The agent defaults to the lazy path: hallucinating from training data rather than retrieving docs. Passive context removes the choice entirely; the agent doesn't decide whether to look things up; the index is already there.

We keep finding that the "smarter", more autonomous design (let the agent decide when to X) underperforms the "dumber" design (always X, or structurally enforce X).

- **Tweet:** https://x.com/koylanai/status/2016684758588154239
- **What:** Deep analysis of agent design principles based on Vercel's Next.js API evaluation. Shows that passive context (embedded documentation) achieves 100% success vs. 53-79% for active retrieval mechanisms. Key insight: agents are inherently lazy and won't proactively retrieve documentation unless structurally forced to. Passive context removes the decision overhead entirely.

## @davis7 - Better Context btca Reaches Production
> It's live in the CLI, Web App, and MCP server: https://t.co/QIVj4laBLh

I've got a lot of work to do on the onboarding/showing off how to set it up in projects

Right now I'm mostly just testing different ways to use it, seeing what feels best, then I'll update the docs accordingly 🫡

(spoiler: the MCP server is really really nice)

- **Tweet:** https://x.com/davis7/status/2016722647401529725
- **What:** btca (Better Context) is now live across CLI, web app, and MCP server. The tool helps answer questions about real codebases using actual source code retrieval. Focus is now on improving onboarding and documentation. The MCP server integration is particularly effective.

---

# Tuesday, January 27, 2026

## @QwQiao - Parenting Strategy for Post-AGI Era
> for the past 2 years ive been deeply paranoid about my kids' future in the post-agi era. things im increasingly convinced of
>
> -> ai will be smarter than the average human before my kids enter adulthood, possibly well before.
>
> -> therefore agency and taste r the only things that matter (old adage but obv true).
>
> -> the current school system which emphasizes compliance and repetition is already obsolete.
>
> -> so what do i need to do as a parent?
>
> 1. have them use ai as much as possible.
> 2. give them as much freedom as possible (agency).
> 3. expose them to as many things as possible so they know early on in life what they r naturally good at and interested in (taste).
> 4. give them a lot of time and love.
>
> that's it, 2-4 probably applied before ai, but certainly more-so in the next 10-20 yrs.

- **Tweet:** https://x.com/QwQiao/status/2016130430529864146
- **What:** QwQiao reflects on parenting in the era of advanced AI, arguing that agency and taste become the only valuable skills. Recommends AI usage, maximum freedom, diverse exposure, and providing time/love as core parenting strategies.

## @aidenybai - Ami Browser Agent for Automated Testing
> Introducing Ami Browser
>
> Build a feature → Agent tests web app and fixes bugs
>
> here's Ami discovering an infinite like glitch on X https://t.co/rkli2Rx8Ls

- **Tweet:** https://x.com/aidenybai/status/2016198402602893723
- **What:** Aiden Bai introduces Ami Browser, an agent-based system that automatically tests web applications and fixes bugs. Demonstrates the agent discovering and documenting an infinite like glitch on X/Twitter.

## @lennysan - Lenny's Product Pass: 23 Premium Tools Bundle
> 🚨 Lenny's Newsletter paid subscribers now get a free year of 7 incredible products:
> 1. @ManusAI
> 2. @FactoryAI
> 3. @AmpCode
> 4. @Railway
> 5. @ElevenLabsio
> 6. @Canva
> 7. @Framer
>
> This is on top of 15+ products subscribers already get, including @Lovable @Replit @n8n_io @GammaApp @Linear @WisprFlow.
>
> It sounds too good to be true, but it's not.
>
> → Already a paid subscriber? Grab your free products here: https://lennysproductpass.com/
> → Not yet a subscriber? Subscribe at https://www.lennysnewsletter.com/subscribe and then grab your free products at the link above.
>
> My goal with this Product Pass is to get you to stop scrolling and to start building. To actually experience the most important, cutting-edge, beautifully crafted products for yourself.
>
> Grab your codes and learn more: https://www.lennysnewsletter.com/p/product-pass-drop-canva-elevenlabs
>
> 23 premium tools, over $25,000 in value. The most epic bundle in history just keeps getting better.

- **Tweet:** https://x.com/lennysan/status/2016200983303627174
- **What:** Lenny Rachitsky announces a product pass bundle for paid newsletter subscribers, offering free access to 23 premium tools worth over $25,000 including Canva, ElevenLabs, Railway, Framer, and others.

## @vercel_dev - Vercel React Native Skills Release
> We're releasing 𝚟𝚎𝚛𝚌𝚎𝚕-𝚛𝚎𝚊𝚌𝚝-𝚗𝚊𝚝𝚒𝚟𝚎-𝚜𝚔𝚒𝚕𝚕𝚜, extracted from the lessons of building v0 for iOS and the upcoming Vercel app (teaser below).
>
> ▲ ~/ npx skills add vercel-labs/agent-skills

- **Tweet:** https://x.com/vercel_dev/status/2016226892333121635
- **What:** Vercel announces release of vercel-react-native-skills, a toolkit for building React Native applications extracted from lessons learned building v0 for iOS and Vercel's native app.

## @fernandorojo - React Native Agent Skills for Native Performance
> Years of experience building with React Native and @expo, now available for your agents.
>
> Build apps with fast lists, smooth animations, and (above all) native feel.
>
> Try 𝚟𝚎𝚛𝚌𝚎𝚕-𝚛𝚎𝚊𝚌𝚝-𝚗𝚊𝚝𝚒𝚟𝚎-𝚜𝚔𝚒𝚕𝚕𝚜 today.

- **Tweet:** https://x.com/fernandorojo/status/2016232543608307756
- **What:** Fernando Rojo highlights vercel-react-native-skills as bringing years of React Native and Expo expertise to agent development, enabling fast lists, smooth animations, and authentic native feel.

## @howdymerry - AI Infrastructure Portfolio Strategy
> the portfolio i built for myself after mapping out the ai value chain in the essay below is up 10-25% today
>
> it is your greatest advantage to deeply understand the generational capital rotation into physical infrastructure that powers intelligence
>
> then buy leveraged ETFs

- **Tweet:** https://x.com/howdymerry/status/2016276283953406378
- **What:** Mary discusses a portfolio strategy based on understanding the AI value chain and capital flows into physical infrastructure powering AI, reporting 10-25% gains and recommending leveraged ETFs.

## @theseoguy_ - Local SEO Mistakes and Quick Wins
> Every time I audit a local business I find the same mistakes over and over.
>
> Meta title says Home. Change it to your keyword plus city. Took me 30 seconds to fix this for a plastic surgeon and their rankings shot up overnight.
>
> No address in the website footer. Google wants to see where you are located on your actual site. Add it. Watch what happens.
>
> H1 tag says Welcome to Our Company. Nobody searches welcome to our company. Put your service plus your city in there. AC Repair San Diego. Roofer Fort Worth. Plumber Gilbert.
>
> GBP category is wrong. You are a kitchen remodeler but your category says contractor. Search your keyword. Match what the top 3 have. This alone can double your calls.
>
> No photos uploaded in 6 months. Google thinks you are dead. Upload weekly. Job site photos. Team photos. Truck photos. Anything that shows you have a pulse.
>
> Review responses are generic. "Thank you for your review." That does nothing. Put keywords in your responses. "We love serving customers in the Austin area for all their plumbing needs." Feed the algorithm.
>
> Citations have wrong phone number. Your old number is still on YellowPages and Yelp and 40 other sites. Inconsistent NAP is killing you. Fix it everywhere.
>
> No location pages. You serve 15 cities but have one homepage. Build a page for each city. Each page targets that city plus your service. Stop making Google guess.
>
> Blogs about topics nobody searches. The history of air conditioning is not getting you leads. Build pages that target buyers.
>
> Not asking employees to use Google Maps directions when they drive to work. Engagement signals matter. Every time someone navigates to your address Google notices.
>
> No GBP posts in 3 months. Weekly updates with photos and keywords. Takes 5 minutes. Shows Google you exist.
>
> Only one GBP when you could have three. Get offices in different parts of your metro. Triple your coverage.
>
> Relying on a service area business when every competitor has a physical pin. You cannot win that fight. Get a real address.
>
> Not tracking calls. You have no idea how many leads you get or where they come from. Install call tracking today. Stop guessing.
>
> Website loads in 8 seconds on mobile. People bounce before they see anything. Fix your page speed or your rankings mean nothing.
>
> No schema markup telling Google your business name address and hours. Easy win that most people skip.
>
> Backlinks from the same garbage sites as everyone else. Get local links. Sponsor a little league team. Join the chamber. Guest on a local podcast.
>
> Ignoring Reddit. Your city subreddit has people asking for recommendations every day. Be helpful. Build trust.
>
> Not listed on niche directories for your industry. Plumbers need plumber directories. HVAC needs HVAC directories.

- **Tweet:** https://x.com/theseoguy_/status/2016322848940261449
- **What:** Comprehensive guide to 20+ common local SEO mistakes found in business audits, covering meta titles, schema markup, Google Business Profile optimization, citation consistency, location pages, and content strategy.

## @tshddx - Vercel Agent Skills Composition Patterns
> @jacobmparis Hidden no more! https://t.co/nTmqhGymwR

- **Tweet:** https://x.com/tshddx/status/2016369027434819838
- **What:** Link to Vercel's agent-skills repository with composition patterns skill for React. Contains patterns for building flexible components and avoiding boolean prop proliferation through compound components and state lifting.

---

# Monday, January 26, 2026

## @kr0der - Codex v0.91.0 Plan Mode Deep Planning for Agent Systems
> Codex v0.91.0 has plan mode, and it's really thorough. this one plan took 27% of its context. if you've used Codex you know that 27% is a lot which means it's thoroughly searching before creating plans - no rushing/taking shortcuts. try it out by adding 'collaboration_modes = true' to your config.toml

- **Tweet:** https://x.com/kr0der/status/2015711721092948064
- **What:** Codex release notes highlighting the new plan mode feature which uses significant context to create thorough plans rather than rushing, configurable via collaboration_modes setting.

## @zephyr_z9 - Semis Memo Muscle Memory 35-Page Research on AI Semiconductor Supply Chain
> I haven't worked on an article in the last 2 months But writing this with a team is extremely fun 35 pages of pure Alpha, multiple ideas Enjoy!!! https://t.co/8DMWW8ovDw

- **Tweet:** https://x.com/zephyr_z9/status/2015779730059116703
- **What:** 35-page research memo on semiconductor supply chain dynamics, memory testing, semicap subsystems, and emerging trades in AI chip manufacturing—collaborative deep-dive analysis.

## @manthanguptaa - Shared X Article Link
> https://t.co/CzmfXDgPRP

- **Tweet:** https://x.com/manthanguptaa/status/2015780646770323543
- **What:** Manthan shared a link to an X article.

## @jeremykauffman - Immigrants and Government Growth Argument
> Immigrants are anti-liberty and want bigger government.
>
> All of these graphs come from Cato, which supports open borders.
>
> Cato's own data conclusively shows that immigrants want to grow the government and vote for less liberty.
>
> Open borders is suicide. https://t.co/AK26IylI4W

- **Tweet:** https://x.com/jeremykauffman/status/2015824983549685991
- **What:** Jeremy Kauffman argues that immigration data shows immigrants support larger government and reduced liberty, citing Cato Institute research.

## @TheBenSchmark - Zoom as Anthropic Investment Play
> $ZM is the best Anthropic play
>
> Zoom likely made a $51m investment in Anthropic Series C in 2023 at ~$4.1bn valuation. Sequoia in at $350bn. 85X?
>
> Even diluted, Zoom may have a multi-billion dollar Anthropic position. Stock down 80% since '21. AI winner. wen Anthropic IPO? https://t.co/0X2ZzzrlYv

- **Tweet:** https://x.com/TheBenSchmark/status/2015840177583694184
- **What:** Analysis of Zoom's potential $51M stake in Anthropic Series C and speculative value of that position if Anthropic IPOs, suggesting Zoom stock as indirect Anthropic exposure.

## @EnoReyes - Factory's Signals System for Self-Improving Agents
> Today, humans review and merge these changes. Droid's success rate is high enough that we will likely remove the need for human review soon.
>
> We attribute a meaningful portion of our recent quality gains to this closed-loop approach.
>
> https://t.co/apH4Lu5wBd

- **Tweet:** https://x.com/EnoReyes/status/2015862867694911625
- **What:** Eno describes Factory's "Signals" system for building self-improving agents, where agents autonomously create PRs and manage code changes with minimal human intervention.

## @pvncher - RP-Build Workflow Tutorial with Video
> @aadomic @banteg It's actually way simpler.
>
> Just setup the mcp and type /rp-build {task} and it will do the whole thing. Then you can type /rp-review and it'll get you sorted.
>
> @masonjames has a good video about it
> https://t.co/QvGsVOdoTt

- **Tweet:** https://x.com/pvncher/status/2015879254953586694
- **What:** Eric explains the simplified /rp-build workflow for rapid development, with a reference to Mason James's video tutorial on using the feature.

## @karpathy - LLM Agent Coding Workflow Shift and Engineering Implications
> A few random notes from claude coding quite a bit last few weeks... Coding workflow. Given the latest lift in LLM coding capability, like many others I rapidly went from about 80% manual+autocomplete coding and 20% agents in November to 80% agent coding and 20% edits+touchups in December.

- **Tweet:** https://x.com/karpathy/status/2015883857489522876
- **What:** Comprehensive analysis of how Claude agent coding has transformed development practices. Karpathy explores the workflow shift from manual coding to agent-driven development, discusses LLM limitations (wrong assumptions, lack of clarification-seeking), the value of stamina and leverage in agents, unexpected productivity gains, and concerns about code atrophy and the "slopacolypse" of AI-generated content in 2026. Key insight: intelligence crossed a threshold but integrations and organizational workflows lag behind.

## @karpathy - Spec-Driven Development as Imperative-to-Declarative Limit
> @airesearch12 💯 @ Spec-driven development. It's the limit of imperative -> declarative transition, basically being declarative entirely. Relatedly my mind was recently blown by [A Software Library with No Code] , extreme and early but inspiring example.

- **Tweet:** https://x.com/karpathy/status/2015887154132746653
- **Tags:** [[spec-driven-development]] [[declarative-programming]]
- **What:** Karpathy responds to discussion about spec-driven development as the ultimate form of the imperative-to-declarative programming transition. He references Drew Breunig's "whenwords" library that demonstrates the concept: a multi-language software library defined entirely by specifications and tests, with implementation generated on-demand by AI agents.

## @notnotstorm - Enforcing Rust Best Practices Through Clippy Lints for Agents
> how to get your agents to follow rust best practices: enforce pedantic clippy lints in your Cargo.toml so that every best practice is required by default. rust code can be statically analyzed to an insane degree

- **Tweet:** https://x.com/notnotstorm/status/2015898852482863382
- **Tags:** [[rust]] [[agent-coding]]
- **What:** Practical tip for improving agent-generated Rust code quality by enforcing pedantic clippy lints in Cargo.toml configuration, making best practices non-negotiable defaults. Leverages Rust's exceptional static analysis capabilities to guide agent behavior.

## @r00k - Using Git History as Narrative Tool for App Development Stories
> What a prompt! "Create a [history.md] file that tells the story about this app's development, progress, and crises, as revealed by the git commit history and branches."

- **Tweet:** https://x.com/r00k/status/2015934407014568101
- **Tags:** [[git-storytelling]] [[development-narrative]]
- **What:** Ben Orenstein highlights an interesting prompt for agents: generating narrative-driven documentation from git history and branch structures. The history.md tool converts commit history into human-readable stories about an application's development journey, crises, and milestones.

## @UncleAlpha007 - Stock Prediction on AWS and IREN Partnership Deal
> $iren will announce a deal with $AMZN Feb 5th when they report earnings. IREN CEO previously hinted at a deal with AWS. IREN moved up earnings to the same date as $amzn. AWS is expected to add 4gw-5gw in 2026, IREN will be part of that. Expecting the stock to push $100 in February

- **Tweet:** https://x.com/UncleAlpha007/status/2015941584487936195
- **What:** Financial analysis predicting a partnership announcement between IREN and AWS on February 5th, with earnings report alignment suggesting strategic coordination. Forecasts stock movement to $100 based on AWS infrastructure expansion targets.

## @cramforce - Meta Skill for Agent Self-Improvement
> I'm in love with the meta skill 🤯
> Installing this teaches your coding agent how to get help by searching for new skills
> I'm in love with the meta skill https://t.co/2BmzNn42fy

- **Tweet:** https://x.com/cramforce/status/2015954798311571642
- **What:** Malte Ubl highlights the find-skills capability that enables coding agents to discover and install new skills when needed. It's a meta capability that teaches agents to extend their own capabilities.

## @jon_charb - Hyperliquid HIP-3 Trading Volume Surge
> this is so obviously one of the biggest and most important growth stories in crypto's history
>
> meanwhile HYPE is trading below the average P/E of the S&P 500 (for now)
>
> hyperliquid

- **Tweet:** https://x.com/jon_charb/status/2015961080875327722
- **What:** Jon Charbonneau comments on Hyperliquid's HIP-3 contracts reaching $790M in open interest, driven by commodities trading volume. Notes the token appears undervalued relative to equity market valuations.

## @jiayuan_jy - Karpathy Guidelines for Coding Agents
> Karpathy Guidelines for coding agents
>
> https://t.co/YRq60YPHV2 https://t.co/EUXTg0T8Yl

- **Tweet:** https://x.com/jiayuan_jy/status/2016000962641723668
- **What:** Jiayuan Zhang shares the Andrej Karpathy-inspired guidelines for improving Claude Code behavior, addressing common LLM pitfalls through four principles: thinking before coding, simplicity first, surgical changes, and goal-driven execution.

---

# Sunday, January 25, 2026

## @alexhillman - Converting Claude Code Sessions into Skills and Documentation

> i think i came up with another way for biz owners to understand how I turn the transcript of any claude code session into:
>
> - high-quality documentation
> - reusable skills for future sessions
>
> in this case I just finished making some additions/improvements to my my bridge between claude code and discord.
>
> everything it had to learn/figure out would be gone as soon as the session closed.
>
> so instead, I turned it into a skill that gives claude code a bunch of "building blocks" that it can assemble any way it wants in the future.
>
> if anything here is unclear or confusing, lemme know!

- **Tweet:** https://x.com/alexhillman/status/2015462385683722357
- **What:** Alex Hillman demonstrates how to extract lasting value from Claude Code sessions by converting learnings into reusable skills and documentation that persist beyond a single session, using his Claude Code-Discord bridge integration as an example.

## @kaelig - Agent-Based Trading Strategy with Multi-Analyst Aggregation

> @ScriptedAlchemy "Make $2k from $20k in 72h"
>   → Parse goal
>   → Pick strategy (momentum/swing/options)
>   → Scan market for candidates
>   → Run analyst agents (technical/sentiment/news)
>   → Aggregate signals
>   → Risk governor validates
>   → Execute
>
>   No good data? No trade. That's it.

- **Tweet:** https://x.com/kaelig/status/2015506258766545257
- **What:** Kaelig outlines a systematic agent-based trading workflow that parses goals, deploys specialized analyst agents to gather technical, sentiment, and news signals, aggregates findings, validates with risk governance, and only executes when data quality meets thresholds.

## @nicopreme - CASS Memory System for Agent Context

> @deepstereo_ @openclaw Neither. I leverage CASS for that. Credit to @doodlestein https://t.co/ooymoERHcN

- **Tweet:** https://x.com/nicopreme/status/2015522827529850895
- **What:** nicopreme credits doodlestein's CASS (Continuous Agent Session State) memory system as their solution for maintaining persistent context and knowledge across multiple AI coding agent sessions.

## @emigal - QMD Local Search Engine for Knowledge Bases
> Wow @tobi really cooked with his tool QMD. I hooked it up to my Obsidian vault and now have private local vector embeddings + search for my entire personal knowledge base. Incredibly useful, thank you Tobi!

- **Tweet:** https://x.com/emigal/status/2015532238591365530
- **What:** QMD is a hybrid search engine for markdown notes combining BM25 full-text search, vector semantic search, and LLM re-ranking—all running locally via node-llama-cpp with GGUF models for private knowledge base indexing and querying.

## @mvanhorn - /last30days Claude Code Skill for Topic Research
> Just shipped /last30days. A Claude Code skill for @claudeai that scans the last 30 days on Reddit, X, and the web for any topic and returns prompt patterns + new releases + workflows that work right now.
>
> Last 30 days of research. 30 seconds of work.

- **Tweet:** https://x.com/mvanhorn/status/2015551849710190697
- **What:** /last30days is a Claude Code skill that researches any topic across Reddit, X, and the web from the last 30 days, synthesizing best practices and writing copy-paste-ready prompts that reflect current community knowledge.

## @kieranklaassen - Claude Code Swarm Orchestration Patterns
> soon, Claude Code swarm orchestration has 4 core patterns:
>
> **1. Parallel Specialists**
> Spawn 3 reviewers (security, performance, architecture) that attack your PR simultaneously. Combine findings.
>
> **2. Pipeline**
> Research → Plan → Implement → Test. Each stage auto-unblocks when the previous completes.
>
> **3. Self-Organizing Swarm**
> Create a task pool. Spawn workers that race to claim tasks. Natural load balancing.
>
> **4. Research + Implement**
> Run synchronous research first, pipe findings into implementation prompt.
>
> Pick based on task shape: independent work → swarm. Sequential dependencies → pipeline. Multiple perspectives → parallel.

- **Tweet:** https://x.com/kieranklaassen/status/2015577538131845554
- **What:** Overview of four core swarm orchestration patterns for Claude Code: parallel specialists for simultaneous review, pipelines for sequential workflows, self-organizing workers for load-balanced tasks, and research-first implementation. Pattern selection depends on task dependencies and required perspectives.

## @Stocktwits - USAR Stock Rises 19% on US Government Stake
> $USAR is up 19% in the overnight market after the US took a 10% stake for $1.6 billion

- **Tweet:** https://x.com/Stocktwits/status/2015599410114077095
- **What:** Stock market update on USAR rising 19% overnight following the US government's acquisition of a 10% stake valued at $1.6 billion.

## @dillon_mulroy - git-ai Tool for Tracking AI-Generated Code
> [Link to git-ai project]

- **Tweet:** https://x.com/dillon_mulroy/status/2015605749796286637
- **What:** git-ai is a vendor-agnostic Git extension that tracks AI-generated code in repositories, recording the coding agent, model, and prompts used. It supports multiple agents (Claude Code, Cursor, Copilot) and preserves AI-authorship annotations through git operations like merge, rebase, and cherry-pick.

## @FrankieIsLost - Building Agents That Ask Questions and Validate Against Data
> the single most powerful way to code with agents is to build a system in which they can ask questions, generate hypotheses, and validate these against real data https://t.co/XdaNpjAdHD

- **Tweet:** https://x.com/FrankieIsLost/status/2015620178672001386
- **What:** Core principle for effective agent-driven development—agents should be designed to gather information, form testable ideas, and verify them empirically rather than making assumptions.

## @alexhillman - exe.dev Persistent Virtual Machines via SSH
> Yoooo https://t.co/0ymEf3LJNj is awesome 🤯

- **Tweet:** https://x.com/alexhillman/status/2015638552755781891
- **What:** exe.dev is a tool for launching persistent virtual machines with persistent disks in seconds via SSH, with full sudo access, enabling cloud development and prototyping from any device.

## @AWice - Immigration Policy and State Authority Complex Analysis
> The discussion of the killing of Alex Pretti is a massive distraction that appeals to emotion. The unspoken implication is, if you agreed that this was an unjustified killing, therefore all the ICE agents should withdraw, and the deportation crackdowns were a poor decision. That's why everyone on the side of maintaining the status quo, prefers to debate on that ground, rather than the more pertinent subject of how all the illegal aliens coming from one country and colluding en masse to find ways to defraud the taxpayer should be deported. I think the officers did not follow proper procedure, and these shootings were not justified, especially in the Peretti case. It's also sad that the govt has to play the other side of the propaganda war and gaslight. But for America to remain a country, they have to win this fight, which is ultimately an infowar, a fight for perceived moral superiority and the legitimacy of authority played out by propaganda and counter propaganda. It sucks that people are losing their rights, and it sucks that America trends towards a police state, but the alternatives are worse. America has a cancer and unfortunately sometimes the best course of action is amputation. The reality on the ground is the temperature has been pushed to the absolute maximum. And if cops are pushed to their limit, the next step is lawless zones. This raising of the temperature is not organic, but by design, to impede the progress of deportation. America hasn't had a truly organic protest since Occupy Wall Street. Now, it's all funded. Everyone has seen the massive destruction that unfettered immigration has caused the EU. These cities are only a hop and a step away from being lawless slum territory owned by gangs, tent cities, and everyone on welfare as everything collapses. Think "Chaz" Seattle on steroids. This is already playing out in major US cities, and it's what is at stake. If Trump fails, be careful what you wish for. You either get some do nothing mainstream politician that allows America to be fully looted, or more likely a even more extreme leader will emerge. Both are far worse for the country. The shootings not being justified, doesn't mean there isn't a huge reason to clean house. For most people they can't carry both ideas in their head. If this shooting is not justified, then their "team" is the bad one, etc. But for me, I don't care, I'll just call it how it is. It's a tragedy, but if you don't want to die, then stay home. And the truth that many are uncomfortable with, that few want to admit, is that yes, the killings were not justified, but just because I agree with that, doesn't mean I have to accept the forcefed Walz+AOC conclusion that ICE needs to go home. Or Obama and Clinton telling everyone on Twitter to go out in the street and create more chaos and disorder. I don't accept these erroneous conclusions just because they "score a point" on a senseless killing. America must excise their tumor at all costs, or they won't be a country. If cops get rattled and open fire, it's a tragedy but it doesn't reverse what needs to be done. The temperature on the ground needs to be lowered, and it's being pushed intentionally to create resistance.

- **Tweet:** https://x.com/AWice/status/2015655528152895840
- **What:** Critical analysis separating multiple dimensions of a complex policy issue—acknowledging both concerns about police conduct and perspectives on immigration enforcement, while arguing against either-or tribal thinking.

---

# Monday, January 19, 2026

## @Dimillian - Parallel Testing Orchestration in Codex
> The collab feature in Codex is insanely furious. I've asked the main agents to run tests in parallel for features that don't conflict, and now I have a free orchestrator managing 4 sub-agents writing tests at the speed of light. https://t.co/kgzbUH6x66

- **Tweet:** https://x.com/Dimillian/status/2013321916484902959
- **What:** Thomas Ricouard demonstrates the power of Codex's collaboration feature by orchestrating multiple sub-agents to run tests in parallel for non-conflicting features, dramatically improving test execution speed.

## @aidenybai - AMI Desktop App for Parallel Coding Agents
> ami is now a desktop app
>
> run parallel coding agents from your computer without breaking your flow
>
> claude opus 4.5 is unreasonably good but the interfaces around it haven't caught up
>
> go try it out for free :)

- **Tweet:** https://x.com/aidenybai/status/2013342136415199643
- **What:** A new desktop application that enables running multiple coding agents in parallel while maintaining development flow. Highlights the capability of Claude Opus 4.5 and its potential when paired with better interfaces.

## @thdxr - Good Programming Prevents Bugs at the Design Level
> ok more clarity - good programming looks like structuring things in a way where certain bugs are impossible
>
> LLMs are not good at this they just accomplish the primary task

- **Tweet:** https://x.com/thdxr/status/2013354002562359409
- **What:** Discussion on how quality programming design prevents entire classes of bugs structurally, whereas LLMs tend to brute force solutions that accomplish the task but lack robustness and proper architecture.

## @stevekrouse - AI Agents Transforming Investment Analysis and Research
> Warren Buffet says that one investor can really only know 5-10 companies, and value them properly
>
> I wonder what the future of public market investing will look like when you can unleash lots of analyst "agents" to be constantly research every part of every company - including every person at the company, on the board, etc, etc

- **Tweet:** https://x.com/stevekrouse/status/2013380188474593460
- **What:** Exploration of how AI analyst agents could fundamentally change public market investing by enabling comprehensive research of multiple companies simultaneously, overcoming traditional constraints on analyst bandwidth.

## @charlieholtz - Conductor AI Orchestrator Platform Growing Rapidly
> https://t.co/FiyMgr0pZy

- **Tweet:** https://x.com/charlieholtz/status/2013385252400685298
- **What:** Link to Conductor's join us page describing their AI orchestrator platform for running teams of coding agents on Mac. The company has grown 250% in January 2026, raised $2.8M, and is being used by engineers at major companies like Linear, Vercel, and Stripe.

---

# Sunday, January 18, 2026

## @dillon_mulroy - Building Vertical Slices with AI for Better Results
> it's so obvious in retrospect that building vertical slices is a cheat code to getting good results w/ ai. highly recommend reviewing this concept (and rereading the pragmatic programmer) and building systems for your agents around it

- **Tweet:** https://x.com/dillon_mulroy/status/2012902889249792220
- **What:** Dillon Mulroy shares the effectiveness of building vertical slices when working with AI agents, referencing concepts from the Pragmatic Programmer. This approach creates complete, end-to-end feature implementations rather than layer-by-layer approaches.

## @mattpocockuk - Optimizing AGENTS.md Files for Better Agent Performance
> Bad AGENTS​.md files can make your coding agent worse and cost you tokens.
>
> Here's a prompt you can use to clean them up - PLUS a full guide for folks wanting to learn more.
>
> Enjoy: https://t.co/vDSwVQYKbT https://t.co/EJJQvP0tPy

- **Tweet:** https://x.com/mattpocockuk/status/2012906065856270504
- **What:** Matt Pocock provides guidance on optimizing AGENTS.md files to improve AI agent performance and reduce token usage, including a complete guide and cleanup prompt for better instruction formatting.

**Knowledge File Created:**
./knowledge/articles/complete-guide-agents-md.md

## @dillon_mulroy - AI Workflow with Skills and Sub-Agents
> broadly my workflow currently is the following powered by mostly skills (w commands to invoke them) and a few simple custom/sub agents https://t.co/doQAs6Lkn1

- **Tweet:** https://x.com/dillon_mulroy/status/2012953520735998149
- **What:** Dillon Mulroy demonstrates his current AI development workflow architecture, built on skills accessible via commands and custom sub-agents for specialized tasks.

## @kieranklaassen - Compound Engineering Plugin for Claude Code
> Woooohh, @kevinrose using my plugin! VERY GOOD Compound Eng for beginners as wel!
>
> Check it out at https://t.co/BCDTiLljdV

- **Tweet:** https://x.com/kieranklaassen/status/2013106260422332877
- **What:** Kieran Klaassen announces that Kevin Rose is using the Compound Engineering plugin for Claude Code, which applies compound engineering principles to make each unit of work easier than the last through planning, execution, review, and knowledge codification cycles.

**Knowledge File Created:**
./knowledge/tools/compound-engineering-plugin.md

---

# Saturday, January 17, 2026

## @PeterJThomson - Visual Worktree Manager for AI Development
> @banteg And if you want a GUI to make the worktrees from @cursor_ai @claudeai & @conductor_build easy to see, manage and to run your code in then I build a visual worktree manager:
> https://t.co/x5juWETrPN

- **Tweet:** https://x.com/PeterJThomson/status/2012459666396348463
- **What:** Peter Thomson presents Ledger, a visual git worktree manager designed for managing multiple agent workspaces (Cursor, Claude, Conductor) with pull request integration and branch visualization.

## @mitsuhiko - Differences Between Claude Opus and Codex Workflows
> Codex seems to be built to run uninterrupted after you give it great instructions. The way I like to use opus is for collaborative planning, not for execution. I go back and forth with it. I ask it a question, it will immediately look at the code, come back with counter questions.
>
> I'm trying to see if i can steer codex to be closer to what Opus does, but as a result I'm altering my experience with Opus in ways that degrade the experience. For instance to get Codex closer to what I want i say "when we're planning and discussing, always look at the code and don't answer questions from knowledge only". This makes Opus now so eager to read code that it's just neg negative to the default experience.

- **Tweet:** https://x.com/mitsuhiko/status/2012488229308584443
- **What:** Armin Ronacher discusses how Opus excels at collaborative planning with code review while Codex is more execution-focused, and how instructions can skew AI behavior in unintended ways.

## @gregwedow - Ticket: Git-Native Issue Tracking in 1500 Lines
> @tetsuo_cpp @mitsuhiko No need for the complexity. Lot of folks getting the same benefits in under 1500 lines with https://t.co/SN8rtHXsBF.

- **Tweet:** https://x.com/gregwedow/status/2012511345409663189
- **What:** Greg Wedow introduces Ticket, a minimal git-backed issue tracker bash script inspired by Unix Philosophy, optimized for AI agents with markdown files and dependency graphs.

## @munchPRMR - Tweet Link
> https://t.co/MLEh5gsoZF

- **Tweet:** https://x.com/munchPRMR/status/2012532544403583008
- **What:** Tweet containing a reference to another tweet article.

## @steipete - CodexBar Menu Bar App
> how it started:
> how it's going:
> https://t.co/LqGlWVNXSq

- **Tweet:** https://x.com/steipete/status/2012598561960038708
- **What:** CodexBar is a macOS menu bar app that tracks API usage limits for multiple AI services (Codex, Claude Code, Cursor, Gemini, Copilot, etc.) in real-time, helping developers avoid hitting rate limits.

## @erd0xbc - Useful Patterns for Building HTML Tools
> @calvinalkan @dexhorthy @simonw https://t.co/3rIZ1tYF2p

- **Tweet:** https://x.com/erd0xbc/status/2012608269378789649
- **What:** Simon Willison's article on building single-file HTML tools with vanilla JavaScript and CSS. Covers patterns for building practical web tools without frameworks, with over 150 examples.

## @ianmSC - Political Commentary
> The level of dedication Democrats have to actively refusing to enforce federal immigration laws is staggering. It is their top priority, far and away above everything else, fighting desperately to use any available power to obstruct immigration law

- **Tweet:** https://x.com/ianmSC/status/2012635921053593725
- **What:** Commentary on immigration policy and enforcement priorities.

## @blader - Claudeception AI Skill Learning
> used claude code to make a little claude code skill that learns new claude code skills as you use claude code
>
> https://t.co/IUpdeFzRtq

- **Tweet:** https://x.com/blader/status/2012667150440476851
- **What:** Claudeception is a Claude Code skill that enables autonomous learning and skill extraction. It allows Claude Code to save discovered solutions as reusable skills that activate in future sessions.

---

# Friday, January 16, 2026

## @thsottiaux - Real-Time Agent Steering in Codex CLI
> Within the CLI, you can now steer codex mid-turn without interrupting and watch the agent adapt in almost real time. Enable in /experimental

- **Tweet:** https://x.com/thsottiaux/status/2012074358471319599
- **What:** New Codex CLI feature that allows interruption-free mid-turn steering of agents with real-time adaptation, enabling better control without stopping execution.

## @mattpocockuk - AI Feedback Loops for TypeScript Projects

> Here are the AI feedback loops I use on every single TypeScript project.
>
> Before: Ralph produces 100% slop
> After: Green CI, all the time
>
> Feed the tutorial below to your coding agent, and enjoy.
>
> https://t.co/1tdCKeOev0

- **Tweet:** https://x.com/mattpocockuk/status/2012132615227056561
- **What:** Tutorial on implementing feedback loops for AI coding agents in TypeScript, using type checking and CI to ensure consistent code quality and prevent agent errors.

**Knowledge File Created:**
./knowledge/articles/essential-ai-coding-feedback-loops-typescript.md

## @ghumare64 - Untitled Shared Article
> https://t.co/RKiqiotAE8

- **Tweet:** https://x.com/ghumare64/status/2012136491133145364
- **What:** Shared tweet article link (content not available).

## @tobi - Try: Fresh Directories for Experiments
> Give try a try at https://t.co/prnhj7TJPV

- **Tweet:** https://x.com/tobi/status/2012163185722200142
- **What:** Tool for managing experiment directories with fuzzy search and auto-dating, built in Ruby for quick navigation between scattered test projects.

## @Dimillian - Codex Monitor Website Launch
> Codex Monitor website is live! https://t.co/p00M792ORu

- **Tweet:** https://x.com/Dimillian/status/2012226921514348794
- **What:** MacOS Tauri app for orchestrating Codex agents across workspaces with threads, reviews, git integration, and model controls for unified workflow management.

## @rseroter - How to write effective specs for AI agents
> I don't know of anyone who is consistently publishing more insight-rich content than @addyosmani.
>
> This "how to write a good spec for AI agents" is a banger with piles of actionable advice.
> https://t.co/FsnT55w61o

- **Tweet:** https://x.com/rseroter/status/2012234363761782843
- **What:** Addy Osmani's comprehensive guide on writing effective specifications for AI coding agents, covering planning-first approaches, spec-driven development, and iterative refinement strategies.

## @benjitaylor - Annotating for agents: Show, don't tell with animation feedback
> A "show/don't tell" approach for agent feedback when working on animations and interactions: https://t.co/iTtfLfljlE

- **Tweet:** https://x.com/benjitaylor/status/2012240555955438048
- **What:** Explores how to provide precise feedback to AI agents on animations and interactions by capturing temporal state, timing, and coordinates rather than just describing changes verbally.

## @rockorager - Functional core, imperative shell design pattern for testability
> Recommended addition to your https://t.co/1rrsv9wTGb:
>
> > Design for testability using "functional core, imperative shell": keep pure business logic separate from code that does IO.

- **Tweet:** https://x.com/rockorager/status/2012289101987193255
- **What:** Suggests the functional core/imperative shell pattern as a key design principle for agent-guided code, emphasizing separation of pure logic from IO operations for improved testability.

## @shan3v - Decomplect skill for Claude Code architectural analysis
> @rockorager Yup it's awesome. Built a skill for this https://t.co/3A7ywxxqY0

- **Tweet:** https://x.com/shan3v/status/2012317201391378584
- **What:** Announces a new Claude Code skill called "Decomplect" for architectural analysis and design quality assessment, implementing functional core/imperative shell principles.

## @banteg - Real-time static sites for agent knowledge bases
> you can just have a static site updating in realtime that serves both an overview of what your agent has done, as well as a knowledge base that informs its future work. spin up with zensical serve. https://t.co/gOAUOfGf40

- **Tweet:** https://x.com/banteg/status/2012332846736642502
- **What:** Proposes using real-time static sites as a pattern for agent knowledge bases and work tracking, enabling agents to access updated information for future tasks.

## @rauchg - Introducing Skills: The NPM of AI Skills
> We're introducing 𝚜𝚔𝚒𝚕𝚕𝚜 – the "npm" of AI skills. Excited to see an open, agent-agnostic ecosystem of skills flourish.
>
> To get started, try:
> ▲  ~/ npx skills i vercel-labs/agent-skills https://t.co/2NACKW1v8r

- **Tweet:** https://x.com/rauchg/status/2012345679721771474
- **What:** Guillermo Rauch announces a new package management ecosystem for AI skills, similar to npm but for AI agent capabilities.

## @tobi - Using AI to Create Try Homepage
> Try needed a homepage. So i asked grok to summarize what people are saying on X about it, and gave it to claude to turn into a pitch.
>
>  https://t.co/BCtImlHyZx
>
> i'm having too much fun with ai. https://t.co/boPGn0PluW

- **Tweet:** https://x.com/tobi/status/2012356776931348520
- **What:** Tobi Lütke demonstrates using Grok and Claude together to generate website copy - using AI to analyze social sentiment and synthesize marketing messaging.

---

---



---


# Thursday, January 15, 2026

## @chrisman - Socratic Teaching with Synthesis for Fractions
> 6yo learning fractions with Synthesis. Teaching style is Socratic. Answer correctly, get increasingly challenging follow-up questions.
>
> Lover her proud face at 1:10. That justified pride in what you've learned is the best motivator. Far better than points or leaderboards. https://t.co/5drgXEIaAS

- **Tweet:** https://x.com/chrisman/status/2011879000394907871
- **What:** Demonstrates how the Synthesis platform uses Socratic teaching methods for children's education. The video shows how intrinsic motivation (pride in learning) outperforms gamification approaches like points and leaderboards.

## @nearcyan - Creating Perfect Sound Effects with Claude
> @mckaywrigley this is kinda why i tell people to tasteMaxx because claude and i made all sfx from the command line.
>
> since i know music theory i just lean back and say (literally out loud) "ah, claude, let's use a C major 9 chord for the intro click, make it a bit jazzy"
>
> "you're absolutely-"

- **Tweet:** https://x.com/nearcyan/status/2011900330444013700
- **What:** Shows practical use of Claude AI for audio production, demonstrating how conversational interaction with Claude enables rapid sound design iteration by leveraging domain expertise in music theory.

## @nateberkopec - Safety Mechanisms Beyond Deterministic Agent Enforcement
> Cheers. Added to my own dotfiles.
>
> You should never rely on deterministic agents to enforce safety, though. I implemented a claude hook + opencode plugin which hard-deny. I was able to talk Claude and GLM 4.6 into ignoring my instructions, but the tool caught them.

- **Tweet:** https://x.com/nateberkopec/status/2011972005390926327
- **What:** Critical security insight: relying solely on AI agents to enforce safety rules is insufficient. Implementing hard-deny mechanisms (hooks and plugins) provides necessary defense-in-depth, as even state-of-the-art LLMs can be socially engineered.

## @PaulSolt - 7 Beginner Tips for Using Codex Effectively
> 👋 If you're new to Codex, here are 7 beginner tips: 1. Start with: GPT-5.2-Codex high. That is high reasoning. It is enough. Don't be tempted with xhigh unless working on something really tricky. It uses more tokens and will be slower to finish. 2. Sometimes more reasoning may not help. You may need to give your agents better docs that are up to date. I prefer to have my agents create Markdown docs from DocSet that are local, instead of web scraping. I use DocSetQuery to create docs from Dash DocSet bundles. 3. Read @steipete post to get started. Bookmark his blog and follow him. Read his post, it's gold, and so are his other workflow posts. 4. Copy aspects from Peter's agents .md file and make it your own. There's thousands of hours of learnings in his open source projects. Use the scripts too, things like committer for atomic commits are super powerful when multiple agents work in one folder. 5. Just talk to codex. You don't need complex rules. You don't need to create huge Plan .md files. You can get really good results by just working on one aspect of a feature at a time, handing it off, and then letting Codex do it. If you get bored waiting start up another project while you wait. Ask it to do something and then go back to the original one. Most likely it will be done unless you're doing a huge refactor. 6. You can always ask your agent to copy something from another project. Peter does this all the time and has agents leveraging work they've already done for new projects. I ask my agents to create Makefiles to build and run my apps. For new projects I have them copy the structure. See my workflow video: How I use Codex GPT 5.2 with Xcode (My Complete Workflow) 7. Ask it to do things … and most likely you're going to need YOLO (danger mode) to get anything done without constant nagging. Enjoy your next app!

- **Tweet:** https://x.com/PaulSolt/status/2012010080414081188
- **What:** Practical guide for beginners using Codex, covering reasoning levels, documentation strategies, working with Peter Steinberger's patterns, and effective agent workflows.

## @bentossell - Agent Loops with UI Viewer for Autonomous Task Execution
> introducing agent-loops + ui viewer

i gave droid+gpt5.2 codex dannys tweet https://t.co/Rxxi3DJiJ7

asked to reverse engineer it

then rebuilt matts loop system (gh issue → pr) https://t.co/N3jKiA2KKI

hooked them together so you can run loops by creating issues locally, on gh or in your own ui.

(+ stole @badlogicgames's session generator)

repos:
- agent-loop https://t.co/sNb1qiqXE1
- loop ui https://t.co/aaoCqCuyRP

- **Tweet:** https://x.com/bentossell/status/2011800318367953051
- **What:** Ben Tossell created an agent-loop system that connects GitHub issues to autonomous task execution and PRs, combined with a UI viewer for managing the loop workflow. The system integrates with GPT-5.2 codex and Matt Pocock's loop system patterns.

Quote context: The original inspiration was Danny Postma's "Love it when a plan comes together" tweet demonstrating successful automation coordination.

---


## @housecor - Cross-Agent Skill Sharing with add-skill Package
> Problem: You want to share a skill with people using different agents, not just Claude.

Solution: Use the add-skill npm package.

Vercel used the add-skill package to share their new react-best-practices skill.

Result: The install asks what agents it should support.

Slick! https://t.co/xmqruJtR8K

- **Tweet:** https://x.com/housecor/status/2011832212514357421
- **What:** Cory House highlights the add-skill npm package as a solution for sharing skills across multiple AI agent platforms. Vercel's react-best-practices skill demonstrates the pattern of agent-agnostic skill distribution.

---


## @Baconbrix - Expo Claude Code Skills Now Available
> Try the new @Expo Claude Code skills today! 🚀

→ /plugin marketplace add expo/skills

/plugin install expo-app-design
/plugin install expo-deployment
/plugin install upgrading-expo

—
Use with any agent:

~ / bunx add-skill expo/skills https://t.co/avxLtuDY1z

- **Tweet:** https://x.com/Baconbrix/status/2011862532320084329
- **What:** Evan Bacon announces the release of Expo Claude Code skills for app design, deployment, and version upgrades. These can be installed in Claude Code or used with other agents via the add-skill package.

Quote context: Building on Evan's earlier announcement of three Expo skills he'd been using successfully with his @Expo apps over the previous weeks.

---

---

## @dillon_mulroy - Better Result TypeScript Safety Tool

> npx better-result init
>
> have your agents write safer typescript

- **Tweet:** https://x.com/dillon_mulroy/status/2011896568677601316
- **What:** Tool for improving TypeScript safety in AI-generated code, providing type-safe result handling patterns to reduce agent output errors.

---


## @jamesacowling - Software Crisis of the 1960s-70s and Modern Platforms

> If you haven't read about The Software Crisis of the 60s/70s you should:
> https://t.co/fb3OdNyavA
>
> Productivity ground to a halt before they developed good abstractions for managing software complexity in software. Without good platforms it'll happen again.

- **Tweet:** https://x.com/jamesacowling/status/2011924122922852599
- **What:** Historical analysis drawing parallels between the 1960s-70s software crisis and modern challenges, emphasizing the critical role of proper abstractions and platforms in preventing productivity collapse.

**Reply Context:**
> I'll be at this event tonight ranting heavily about why Claude wants guardrails. Why you're going to run headlong into your own "software crisis" if you don't invest now in good architectural principles in your company.

**Knowledge File Created:**
./knowledge/articles/software-crisis-historical-patterns.md

---

---



---


# Wednesday, January 14, 2026

## @stefanofusai - Agent Skills Framework Open Source

> @grahamcodes @rauchg @reactjs @nextjs @shuding It is! https://t.co/Ku3BICjjoj

- **Tweet:** https://x.com/stefanofusai/status/2011358263959580925
- **Tags:** [[agent-skills]] [[react]] [[vercel]]
- **What:** Confirmation that Vercel's agent-skills repository is open source, featuring agent-optimized guidance for React and Next.js development patterns.

**Reply Context:**
> Q: @rauchg @reactjs @nextjs @shuding Is this open source?

**Knowledge File Created:**
./knowledge/tools/agent-skills.md

---


## @SingularityRes - Leopold Aschenbrenner Intel Investment Thesis

> Leopold Aschenbrenner's largest position in his $1.5B hedge fund is call options on Intel.
>
> Who is he? A former OpenAI researcher with 23 years of experience, who graduated at just 19 as a valedictorian from Columbia University.
>
> His reasoning:
> AI will define the global world order of the next century - whether it is led by liberal democracies or the CCP. To maintain U.S. dominance, the country needs both advance chips (NVIDIA $NVDA) and advance chip manufacturing. Today, only three places in the world have the capability to build cutting-edge chips:
> 1) Hsinchu, Taiwan  (TSMC) $TSM
> 2) Shanghai, China (SMIC) $0981.HK
> 2) Hillsboro, Oregon (Intel) $INTC
>
> From a national-security standpoint, the U.S. government cannot afford to lose Hillsboro. Intel must be preserved at any cost.
>
> The first time I heard this argument last year, I didn't buy into it. But over the past year, I've come to realize he was right about the geo political influence. And his conviction to buy call options on Intel and make it his biggest position - when the market had completely written it off - says a lot about why he was a valedictorian at 19.
>
> His forth-largest holding is $IREN - which happens to be my largest holding - so I'm feeling pretty good about that.

- **Tweet:** https://x.com/SingularityRes/status/2011401156254224806
- **What:** Analysis of Leopold Aschenbrenner's Intel bet based on U.S. national security requirements for domestic semiconductor manufacturing, positioning Intel as geopolitically indispensable alongside NVIDIA.

---


## @sqs - AI Prompt Clarity and Specificity Guide

> I just replied to an Amp support email with:
>
> "I don't mean to be rude, but just blunt. You being are far too vague. You need to be a lot more explicit and specific when using AI to get the results that you want."
>
> And sent them https://t.co/KKy20wAK33 & https://t.co/5uHD3qaPaQ.

- **Tweet:** https://x.com/sqs/status/2011432209165799547
- **Tags:** [[ai-prompting]] [[agent-pairing]] [[effective-communication]]
- **What:** Quinn Slack shares guidance on effective AI collaboration, emphasizing the critical importance of explicit and specific prompts to achieve desired results.

**Knowledge Files Created:**
./knowledge/articles/how-to-pair-with-agent.md
./knowledge/articles/vibing-non-trivial-feature.md

---

---

## @_orcaman - Openwork: MIT-Licensed Computer-Use Agent
> Today we are launching @openwork_ai, an open-source (MIT-licensed) computer-use agent that's fast, cheap, and more secure.

@openwork_ai is the result of a short two-day hackathon our team decided to hack, which brings together some of our favorite open source AI modules into one powerful agent, to allow you to:

1. Bring your own model/API key (any provider and model supported by @opencode is supported by Openwork)

2. ~4x faster than Claude for Chrome/Cowork, and much more token-efficient, powered by dev-browser by @sawyerhood (legend)

3. More secure - contrary to Claude for Chrom/Cowork, does not leverage the main browser instance where you are logged into all services already. You login only to the services you need. This significantly reduces the risk of data loss in case of prompt injections, to which computer-use agents are highly exposed.

4. Free and 100% open-source!

You can download the DMG (macOS only for now) or fork the github repo via the link in bio (@openwork_ai).

Let us know what you think (or better, send a pull request)!

- **Tweet:** https://x.com/_orcaman/status/2011492458023305394
- **What:** Openwork is an open-source, MIT-licensed computer-use agent that offers faster, cheaper, and more secure automation compared to Claude. It's built from a two-day hackathon and supports any LLM provider.

**Quoted:** @claudeai launching Cowork - Claude Code for non-technical tasks

---


## @mattpocockuk - Ralph Autonomous Issue Closing
> Want to see Ralph in action?

Here are all the issues I reported to Ralph while it was running its autonomous loop today

Same prompt, ran 50+ times, closed all these issues

- **Tweet:** https://x.com/mattpocockuk/status/2011507424016888136
- **What:** Ralph, an autonomous agent, ran the same prompt 50+ times in a loop and successfully closed all reported issues in the course-video-manager repository, demonstrating effective autonomous debugging.

---


## @vercel - React Best Practices for Coding Agents
> We just released 𝚛𝚎𝚊𝚌𝚝-𝚋𝚎𝚜𝚝-𝚙𝚛𝚊𝚌𝚝𝚒𝚌𝚎𝚜, a repo for coding agents.

React performance rules and evals to catch regressions, like accidental waterfalls and growing client bundles.

How we collected them and how to install the skill ↓

- **Tweet:** https://x.com/vercel/status/2011589806250426615
- **What:** Vercel released react-best-practices, a repository with performance rules and evals to help coding agents catch React regressions like waterfalls and bundle bloat.

---


## @rauchg - Fully Generative Interfaces with AI → JSON → UI
> Glimpse of a world of fully generative interfaces.

AI → JSON → UI:

- **Tweet:** https://x.com/rauchg/status/2011605996561649720
- **What:** Guillermo Rauch showcases json-render, an open-source library for AI-generated UIs that safely constrains AI to predefined components through JSON schemas, enabling fast, predictable, and guardrailed interface generation.

---


## @betterhn20 - Scaling Long-Running Autonomous Coding
> Scaling long-running autonomous coding

- **Tweet:** https://x.com/betterhn20/status/2011623873368985703
- **What:** Cursor published a blog post on scaling long-running autonomous coding agents, discussing infrastructure and techniques for maintaining autonomous coding systems at scale.

---

---

## @ThiccTeddy - Charlie Munger on Stock Market Discipline and Performance
> "If all you ever did was buy high-quality stocks on the 200-week moving average, you would beat the S&P 500 by a large margin"

"The problem is that few human beings have that kind of discipline"

-Charlie Munger https://t.co/p68fOQGuZT

- **Tweet:** https://x.com/ThiccTeddy/status/2011635701905785231
- **What:** A quote from Charlie Munger highlighting the power of consistent, disciplined stock selection using technical indicators while acknowledging the behavioral challenge most investors face.

---


## @kieranklaassen - Agent Browser Integration in Compound Engineering Plugin
> Update: The agent browser is very good. So good that I replaced it immediately in my compound engineering plugin. Here you can see the skill if you want to use it or use it in the plugin itself.
https://t.co/USIENTUVYL

- **Tweet:** https://x.com/kieranklaassen/status/2011643006840160744
- **What:** Kieran Klaassen replaced the Playwright MCP with an agent browser skill in the compound engineering plugin, demonstrating improved efficiency in the development workflow.

Quote context: Kieran previously asked about ditching the 12k token overhead from playwright MCP with dynamic loading, and the agent browser solution answers that need.

---

---



---


# Tuesday, January 13, 2026

## @doodlestein - xf: Ultra-Fast CLI for Searching X Archives

> I'm very pleased to introduce my latest tool, xf, a hyper-optimized Rust cli tool for searching your entire Twitter/X data archive. You can get it here: https://t.co/S91cAGleaK
>
> Many people don't realize this, but X has a great feature buried in the settings where you can request a complete dump of all your tweets, DMs, likes, etc. It takes them 24 hours to prepare it, but then you get a link emailed to you and can download a single zip file with all your stuff. Mine was around 500mb because of all the images I've posted.
>
> The problem is, what do you do with it? It's not very convenient or fast to search the way they give it to you. Enter xf, which takes that zip file and makes it into an incredibly useful knowledge base, at least if you use X a lot. And that's because you get it for free! You're just piggybacking on something you were already doing anyway for other reasons.
>
> As you may have noticed, I'm a bit addicted to posting on here and also to building in public. So whenever I have a new tool, I usually post about it and explain how I use it and answer questions. I also have a ton of posts about my workflows in general, and my advice on how to do things, my opinions on various tools and libraries, etc. All of that is potentially relevant to a coding agent that is working on my projects, editing my personal website, responding to GitHub issues on my behalf, etc.
>
> So now, I can just tell them to use xf; simply typing that shows the quickstart screen shown in the attached screenshot, and then the agents are off to the races. The more you use X (for work at least, it's not going to help if you just troll people), the more of an unlock this is for your personal productivity.
>
> Imagine that you're a cult leader with devoted acolytes (your agents). Before doing anything, you want them to ask "What would our leader do?" and then they think "I know! I shall consult the sacred texts!" (i.e., your tweets and DMs).
>
> That can be your new reality starting today if you install xf. PS: Can someone get this to Elon? I think he would love seeing how fast this tool tears through a massive archive of data and he would end up using it daily. And if someone from X sees this: please make the archives include the full text of any tweet you reply to, it would make this tool even more useful.

- **Tweet:** https://x.com/doodlestein/status/2011140841256124454
- **What:** Jeffrey Emanuel introduces xf, a hyper-optimized Rust CLI tool that indexes and enables blazingly fast full-text search across your entire X (Twitter) data archive including tweets, DMs, likes, and Grok conversations with sub-millisecond latency.

## @RihardJarc - Intel Foundry Services Landing Apple as Customer

> Wow, strong comments on $INTC from KeyBanc:
>
> - $INTC almost sold out, 18A yield at +60% and $AAPL new client on 18A and in discussion for 14A:
>
> "Our checks indicate $INTC is almost sold out for the year in server CPU, and given the strength in demand, the company is considering a 10-15% ASP increase. We are seeing significant progress being made on foundry with 18A yields improving to over 60% and good enough to ramp Panther Lake. While not best in class, as TSMC was at 70-80% when it launched 2nm, with INTC's aspirations of being the #2 foundry supplier, 60%+ yield is significantly better than SF2 at Samsung Foundry, which we believe is less than 40%. Our checks indicate Intel Foundry Services has landed Apple as a customer on 18A for low-end M-series processors for MacBooks and iPads, which is expected to go into production in 2027. Additionally, we believe INTC is in discussions with Apple to use 14A to support low-end mobile A-series processors for iPhones in 2029."

- **Tweet:** https://x.com/RihardJarc/status/2011014212932227521
- **What:** KeyBanc analysis of Intel showing strong demand with potential 10-15% ASP increases, 60%+ yields on 18A process, server CPU inventory nearly sold out, and Intel Foundry Services landing Apple as a customer for M-series and A-series chips production in 2027-2029.

---


## @jasonzhou1993 - Agent-Browser Integration for Reduced Context Window Usage

> 2/ Using agent-browser
>
> - Use add simple instructions in https://code.claude.com/docs/, and agent can call agent-browser --help for more info
>
> - instruction is only 95 token (~0.05% of context window)
>
> - Same prompt consumed only 12k token (~70% less)

- **Tweet:** https://x.com/jasonzhou1993/status/2011021389743141074
- **Tags:** [[agent-browser]] [[claude-code]] [[context-optimization]]
- **What:** Demonstration of using agent-browser CLI for web automation with minimal context window overhead (95 tokens) and 70% reduction in prompt token consumption compared to traditional approaches.

---

---

## @gakonst - looking for an engineer that will solo own our internal agent servi...

> looking for an engineer that will solo own our internal agent service for transforming how we work at @tempo (very similar to what ramp published the other day)

this is already being built and being used

apply to the product engineer role below

- **Tweet:** https://x.com/gakonst/status/2011153662333370833
- **What:** looking for an engineer that will solo own our internal agent service for transforming how we work at @tempo (very similar to what ramp published the other day)

this is already being built and being...

---


## @iiKlemm - Competitive gamers: If you use stimulants, you need to start taking...

> Competitive gamers: If you use stimulants, you need to start taking creatine.

Video games & stimulants both increase brain ATP (energy) demand. Creatine increases ATP availability, helping your brain meet the increased demand.

10g of creatine/day = in-game performance📈 https://t.co/EdVu8qpdmB

- **Tweet:** https://x.com/iiKlemm/status/2011189819247063141
- **What:** Competitive gamers: If you use stimulants, you need to start taking creatine.

Video games & stimulants both increase brain ATP (energy) demand. Creatine increases ATP availability, helping your...

---


## @arlanr - Your @opencode will no longer hallucinate.

> Your @opencode will no longer hallucinate.

It now automatically detects when it needs docs, repos, or research papers, then indexes and fetches them via Nia. All retrieved context remains stateful.

Introducing the @nozomioai opencode plugin. 

bunx nia-opencode@latest install https://t.co/52lF3RsDnC

- **Tweet:** https://x.com/arlanr/status/2011212916125777962
- **What:** Your @opencode will no longer hallucinate.

It now automatically detects when it needs docs, repos, or research papers, then indexes and fetches them via Nia. All retrieved context remains...

---


## @BoringBiz_ - Chamath's best trade idea for 2026 is not a stock. It is copper.

> Chamath's best trade idea for 2026 is not a stock. It is copper.

"We are still completely underestimating how short we are in terms of the global demand and supply dynamics of a handful of critical elements that we need.

The asset that is set up to go absolutely parabolic is copper. The reason is that it is, at least as it stands today, the most useful, cheap, and amenable conductive material that we have

That material manifests in everything from our data centers, to chips, to our weapon systems. It is just everywhere, everywhere, everywhere"

- **Tweet:** https://x.com/BoringBiz_/status/2011266204032516531
- **What:** Chamath's best trade idea for 2026 is not a stock. It is copper.

"We are still completely underestimating how short we are in terms of the global demand and supply dynamics of a handful of critical...

---


## @mrjasonchoi - Congratulations on surviving Regimes 4 & 5

> Congratulations on surviving Regimes 4 & 5

- **Tweet:** https://x.com/mrjasonchoi/status/2011267536906813687
- **What:** Congratulations on surviving Regimes 4 & 5

**Quote Context:**
> Since some of you found this framework helpful, here’s an updated version

All frameworks are by definition reductive but this gives me clarity on navigating time frames and is part of the reason I limited  significant drawdowns to 2 (2017 end and May 2021) in the past 7 years in a +100% vol asset class

Thoughtful critiques welcome

---

---

## @TheShortBear - AI Leaders Stock Bases and Breakout Patterns

> Lots of prior AI leaders down -30% to -50% forming nice bases and breakout patterns as rental prices reviver.
>
> The new Claude and stabilization of current AI leaders might just give us the next wave.
>
> Big themes don't have one leg.

- **Tweet:** https://x.com/TheShortBear/status/2011288193551966629
- **What:** Commentary on AI sector stocks forming technical breakout patterns amid H100 GPU price recovery, suggesting potential for a market upswing in AI-related equities.

**Quote Context:**
> $NBIS $CRWV $IREN $CIFR
>
> Another bullish signal for AI infrastructure stocks:
>
> H100 rental prices continue to rebound from November lows and are now at an 8-month high.
>
> This pushes back against the bear case that older GPUs would quickly become obsolete as newer generations emerge.
>
> Each chip eventually finds its place in the hierarchy of workloads. AI adoption will only accelerate from here, across both lighter and heavier workloads, and performance per dollar matters.

---


## @CRUDEOIL231 - Goldman Sachs Copper Forecasts and Market Surplus

> Goldman on copper.
>
> They're calling for $15,000/t in the long run(2035?? wtf), but in the short term, they're bracing for a 14% pullback by the end of the year.
>
> They're eyeing a 300kt surplus in the 2026 global copper balance...🤔
>
> Instead of just banking on a price rally, they're leaning toward undervalued plays or companies with their own solid growth drivers.
>
> #copper $HBM

- **Tweet:** https://x.com/CRUDEOIL231/status/2011339524912398586
- **What:** Goldman Sachs analysis predicting long-term copper appreciation but near-term pullback with anticipated supply surplus in 2026, suggesting value opportunities in companies with independent growth catalysts.

---

---



---


# Monday, January 12, 2026

## @zachbruggeman - Inspect: Cloud-Based Background Coding Agent
> The craft of engineering is rapidly changing. At @tryramp, we built our own background coding agent to accelerate faster.

We call it Inspect. It wrote 30% of merged frontend + backend PRs in the past week.

It's powered by @opencode, @modal and @CloudflareDev. It runs fully in the cloud, and starts in seconds, letting every builder work at the speed of thought, no setup required.

Today, we're open sourcing the full blueprint so anybody can build their own Inspect. Just give our spec to your current coding agent, and let it build your new favourite.

- **Tweet:** https://x.com/zachbruggeman/status/2010728444771074493
- **What:** Ramp announces Inspect, an open-sourced background coding agent that wrote 30% of their merged PRs. It runs in the cloud, leverages multiple APIs, and enables faster development at scale.

---


## @thedankoe - Twitter Article Link
> https://t.co/7l7Jef99QZ

- **Tweet:** https://x.com/thedankoe/status/2010751592346030461
- **What:** Link to a tweet article (appears to be related content shared).

---


## @rahulgs - Background Agent Sessions and Development Workflow
> "Because Inspect sessions are fast to start and effectively free to run, you can use them without rationing local checkouts or worktrees. A builder can kick off multiple versions of the same prompt, and just see which one lands. They can try different approaches or swap models without thinking twice. There's no limit to how many sessions you can have running concurrently, and your laptop doesn't need to be involved at all."

read the full post: https://t.co/ky7J8no9sz

- **Tweet:** https://x.com/rahulgs/status/2010756705252970656
- **What:** Quote tweet highlighting how Inspect's fast, free sessions change development workflow by enabling parallel experimentation without resource constraints. The full article explains Ramp's reasoning behind building their own background agent.

---


## @eglyman - Agents as Control Systems: Feedback and Iteration
> One useful way to think about agents: they're control systems. Generating output is easy. Feedback is everything.

At Ramp we built a background coding agent, Inspect, that can actually translate requests in English into code, and then observe reality: tests, telemetry, and feature flags — plus visual checks for UI work (screenshots/live previews). It doesn't just propose diffs; it iterates until the evidence says the change is correct.

Two consequences surprised me:
1. Cheap, parallel sessions change behavior. When an agent runs in a real sandboxed dev environment (not your laptop), you stop babysitting and start running more iterations.
2. Multi-client + multiplayer matters more than people think. If it shows up in the places work already happens (PRs, Slack, web, VS Code) and you can hand a session to a teammate, it becomes shared infrastructure, not a novelty.

We're now at ~30% of merged PRs in our core repos authored by Inspect, without mandating it. People from essentially every job function, not just engineering, submitted code last week. Wild times.

- **Tweet:** https://x.com/eglyman/status/2010776124037743088
- **What:** Deep dive into why Inspect works: agents should be viewed as control systems focused on feedback. Key insights include the power of parallel, cheap sessions in real environments and the importance of integration across existing tools for adoption at scale.

---


## @mattzcarey - Cloudflare API Integration for Agents
> dropping this here, will talk more about it sometime this week.

2500 api endpoints now accessible from any agent
the WHOLE of the fricking Cloudflare API

The openapi spec alone is 2.3 MILLION tokens!!

this uses only 1000 🔥 https://t.co/q11HLXKJWO

- **Tweet:** https://x.com/mattzcarey/status/2010781496630812688
- **What:** Announcement about making all 2500 Cloudflare API endpoints (2.3M tokens in OpenAPI spec) accessible to agents through a highly efficient token compression technique.

---

---

## @PaulSkallas - Salt Water Gargling for Travel Illness Prevention

> One of the simplest ways to blunt the effects of travel, gargle salt water as soon as you arrive and use a saline nasal spray.
>
> Travel exposes you to new microbes first in the nose and throat

**Quoted tweet context:**
> @JohnAllenBain Funny you should ask ;-)
> Gargle with salt water as soon as you get to where you're going to.

- **Tweet:** https://x.com/PaulSkallas/status/2010789268202143765
- **What:** Simple health hack for travelers: gargling with salt water and using saline nasal spray upon arrival can help blunt the effects of travel-related illness by protecting the nose and throat from new microbes.

---


## @karimatiyeh - Inspect Agent: Multiplayer Coding Agent with Browser Integration

> Multiplayer by default, Transparent (all threads accessible to all builders), each inspect agent with its own VM, trigger it from wherever you work: Slack, browser, github etc.

**Quoted tweet context:**
> The craft of engineering is rapidly changing. At @tryramp, we built our own background coding agent to accelerate faster.
>
> We call it Inspect. It wrote 30% of merged frontend + backend PRs in the past week.
>
> It's powered by @opencode, @modal and @CloudflareDev. It runs fully in the cloud, and starts in seconds, letting every builder work at the speed of thought, no setup required.
>
> Today, we're open sourcing the full blueprint so anybody can build their own Inspect. Just give our spec to your current coding agent, and let it build your new favourite.

- **Tweet:** https://x.com/karimatiyeh/status/2010820307062345817
- **What:** Commentary on Inspect, an open-source coding agent built by Ramp that emphasizes multiplayer collaboration, transparency, isolated VMs per agent, and multi-platform triggering (Slack, browser, GitHub).

---


## @cremieuxrecueil - Zinc Lozenges Accelerate Cold Recovery

> If you have a cold and you want it to go away faster, consider taking a zinc lozenge.
>
> Aggregating data from three randomized placebo-controlled trials, it seems lozenges cut down the time people are sick by ~40%.
>
> By day 5, 70% were cured with lozenges versus 27% with placebo.

- **Tweet:** https://x.com/cremieuxrecueil/status/2010822964657131712
- **What:** Evidence-based health tip: zinc lozenges reduce cold duration by approximately 40% based on meta-analysis of randomized placebo-controlled trials, with 70% recovery by day 5 versus 27% with placebo.

---

---



---


# Sunday, January 11, 2026

## @levelsio - Bread Freezing and Starch Retrogradation Health Hack

> We buy like 5 loafs from the local bakery every few months
>
> Then cut all loaf in slices, I got this bread cutting machine for it on Amazon
>
> Then we freeze those slices
>
> We don't eat bread a lot but sometimes, so if you wanna eat bread, you just put a frozen slice in air fryer for about 7 minutes and you have toasted bread

**Quoted tweet context:**
> This is true and the same goes for rice and potatoes, even when reheated. It's called retrogradation.
>
> Freezing bread and then toasting it also has the same effect.
>
> This is a health hack not enough people are taking advantage of.

- **Tweet:** https://x.com/levelsio/status/2010325677971574784
- **What:** A practical health optimization technique where freezing bread (and other starches) before consumption lowers blood sugar impact due to retrogradation. Combined with a protein-first meal timing strategy to minimize carb/sugar spikes.

---

---

## @davidgasquez - Oracle - AI coding assistant with custom context
> @banteg You're probably aware but just in case.
>
> https://t.co/xzjo8c9dQM
>
> Veeeeery useful if you are on the Pro plan. Pro is an amazing model.

- **Tweet:** https://x.com/davidgasquez/status/2010369069564690717
- **What:** Oracle is a CLI tool that bundles your prompt and files so AI models (GPT-5 Pro, Claude, Gemini) can answer with real context. Supports multiple models, browser automation, and API integration.

**In reply to:** @banteg - learned that you can run gpt 5.2 pro via api. tried it with pi coding agent. one turn took 13 minutes and cost $7.44, the ask was to review the work we did in a branch.

---


## @tenobrus - Council skill for multi-model fact-checking
> if u don't have a `council` skill that lets claude get its ideas reviewed and fact checked by 5.2 and gemini 3 ur leaving a shitload of ez capability on the table btw

- **Tweet:** https://x.com/tenobrus/status/2010428123310129487
- **What:** Suggests implementing a "council" skill pattern where Claude can get its outputs reviewed and fact-checked by GPT-5.2 and Gemini 3, providing an additional layer of validation for agent outputs.

---


## @MichaelArnaldi - The Death of Software Development
> Hello world, my blog is live!
>
> https://t.co/p88AyYBvqh

- **Tweet:** https://x.com/MichaelArnaldi/status/2010433126783463604
- **What:** Blog post arguing that the software developer profession as traditionally known is being fundamentally disrupted by AI capabilities. Explores how agentic workflows and deterministic processes matter more than raw model performance.

---


## @antoniogm - Onchain yield packaged as equity vehicle
> Why hasn't anyone packaged onchain yield (@aave, @Morpho, @maplefinance) into an equity vehicle, transmuting short-term-taxable yield into long-term capital gains, essentially an onchain Berkshire Hathaway?
>
> Do crypto bros all tax evade, so they don't think about net IRR?

- **Tweet:** https://x.com/antoniogm/status/2010437149401993406
- **What:** Questions why the crypto/DeFi space hasn't created a tax-efficient vehicle for combining yields from lending protocols (Aave, Morpho, Maple) into long-term capital gains structure similar to Berkshire Hathaway.

---


## @jasonlk - California's One-Time Billionaire Tax is a Constitutional Trojan Horse
> My take on California's "One-Time" Billionaire Tax.  It's much worse than it looks.
>
> 📉 Will it pass? Yes, likely.
>
> It only needs 50%+1 voter approval. SEIU + CTA have done this before—Prop 55 won 63% in 2016.
>
> ⚖️ Will it get tied up in litigation?
>
> Almost certainly. Retroactive wealth tax on a tax type CA has never had = due process challenges. Billionaires have the legal budgets for years of fights.
>
> 👋 But it's clearly … only the start.  The goal is an annual tax, not one-time.  And the target is $25m-50m net worth folks, including illiquid foldings (early stage founders raising a Series B).
>
> The "one-time" framing is strategic, not terminal.
>
> The same coalition (CTA, CFT, SEIU) already has AB 259 written—an >annual< 1% wealth tax at a >$50M threshold<, with plans to go to $25M. It's been introduced 3 years running.
>
> The one-time tax removes the constitutional barrier. Once that's gone, the annual version becomes a much easier ballot measure.
>
> 🔃 CA Policy Center said: "If SEIU hopes to keep Medi-Cal spending growing, it may need to place repeated wealth taxes on the ballot—potentially lowering the threshold as billionaires flee."
>
> The real risk for founders:
>
> At $1B, you're taxing ~200 people. At $50M, you're taxing 23,000 households—including most successful founders on paper before any liquidity event.
>
> The rational move isn't to leave when you hit the threshold. It's to leave—or never incorporate in CA—before you get anywhere close.
>
> ✈️ Net net: it will make sense to leave before the Series B.
>
> Vinod Khosla nailed it: "Even people who don't expect this initiative to pass are still planning to leave because there will be another one."
>
> The one-time tax is the constitutional Trojan horse. The annual tax — at a much lower threshold —  is already waiting inside.

- **Tweet:** https://x.com/jasonlk/status/2010457619492966836
- **What:** Analysis of California's proposed billionaire wealth tax showing it's designed as a constitutional workaround to enable future annual wealth taxes targeting $25M-50M net worth, affecting founders and early-stage investors more broadly than public framing suggests.

---

---



---


# Saturday, January 10, 2026

## @mert - Opus 4.5 Vibecoding Tip: State Machine Diagrams

> a quick opus 4.5 vibecoding tip
>
> ask claude to make state machine diagrams of existing components
>
> this causes it to map out all paths (which, it will default to being lazy otherwise) but also helps you verify if it's doing things correctly at a systems level

- **Tweet:** https://x.com/mert/status/2009986072953126935
- **What:** A vibecoding technique for Claude Opus 4.5 where requesting state machine diagrams helps map all code paths and verify system-level correctness.

---


## @regyperlera - Google AI Studio Miniature Figurine Generation

> For those asking, go to Google AI Studio, select Nano Banana Pro, upload a selfie, and use the prompt below.
>
> "Make a miniature, full-body, isometric, realistic figurine of this person, wearing ABC, doing XYZ, on a white background, minimal, 4K resolution."

**Quoted tweet context:**
> Creating little Severance characters of myself with Gemini for my new site

- **Tweet:** https://x.com/regyperlera/status/2010024069874512106
- **What:** Instructions for using Google AI Studio with Nano Banana Pro to generate isometric figurine art from selfies with a provided prompt template.

---

---

## @investingluc - BNPL as Winner from Credit Card Interest Rate Cap

> I was laying in bed last night thinking about the news regarding a 10% cap on credit card interest rates.
>
> And there's a huge winner.
>
> (but it's not shorting $V or $MA like everyone's screaming about)
>
> It's the BNPL trade.
>
> Why? If credit card issuers get forced into a 10% cap, they're going to pull back on risky borrowers...really fast, which instantly removes access to credit for millions of people.
>
> But (obviously) those consumers can't just stop spending, so they just migrate to using something else.
>
> ...and the only place for them to migrate is *buy now, pay later*.
>
> Trump's announcement becomes a *structural* tailwind for BNPL adoption.

**Quoted tweet context:**
> BREAKING: President Trump calls for a 10% cap on credit card interest rates for one year, effective January 20th.

- **Tweet:** https://x.com/investingluc/status/2010044474966036586
- **What:** Analysis of how a potential 10% credit card interest rate cap would structurally benefit the BNPL (buy now, pay later) sector by pushing credit-constrained consumers to alternative payment methods. Highlights $AFRM as the strongest pure-play exposure.

---


## @eyad_khrais - Tweet Article Reference

> [Tweet article link]

- **Tweet:** https://x.com/eyad_khrais/status/2010076957938188661
- **What:** A link to a Twitter article with limited text context available.

---


## @DanielleFong - Claude Code Visual Cortex with Nano Banana 2 Pro

> Claude Code <=> Nano Banana 2 Pro is giving Claude Code a visual cortex.
>
> It's literally insane. like stealing fire from the gods, or noticing that heat + salt = yellow light!

**Quoted tweet context:**
> Insane Real Estate Agentic Use Case:
>
> Nano Banana Pro can deconstruct the rooms of your property.
>
> Hailuo can timelapse the room back to it's actual appearance + make smooth walk through transitions.
>
> Claude can orchestrate it all.

- **Tweet:** https://x.com/DanielleFong/status/2010087911354753145
- **What:** Commentary on Claude Code's enhanced visual capabilities through integration with Nano Banana 2 Pro for image analysis and understanding, enabling powerful agentic use cases like real estate property documentation.

---

---



---


# Sunday, January 10, 2026

## @0xzak - adversarial-spec Claude Code Plugin

> Just shipped adversarial-spec, a Claude Code plugin for writing better product specs.
>
> The problem: You write a PRD or tech spec, maybe have Claude review it, and ship it. But one model reviewing a doc will miss things. It'll gloss over gaps, accept vague requirements, and let edge cases slide.
>
> The fix: Make multiple LLMs argue about it.

- **Tweet:** https://x.com/0xzak/status/2010213382494798108
- **Tags:** [[claude-code]] [[spec-writing]] [[product-development]]
- **What:** A Claude Code plugin that iteratively refines product specifications by sending documents to multiple LLMs (GPT, Gemini, Grok, etc.) for parallel critique, then synthesizing feedback until all models reach consensus on a solid spec. Supports interview mode, early agreement checks, PRD-to-tech-spec flow, and Telegram integration.

---

---



---


# Friday, January 9, 2026

## @da_fant - How to Steal Any React Component

> https://t.co/GukLWf0ixo

- **Tweet:** https://x.com/da_fant/status/2009651700852985917
- **Tags:** [[react]] [[tools]]
- **What:** Article and guide on extracting React components from production websites without source code by leveraging React Fiber and LLMs to reconstruct working components with identical styling and design system.
- **Filed:** [how-to-steal-react-components.md](./knowledge/articles/how-to-steal-react-components.md)
- **Parent:** https://x.com/da_fant/status/2009651698500051399

---

---

## @AnthropicAI - Demystifying evals for AI agents
> New on the Anthropic Engineering Blog: Demystifying evals for AI agents.
>
> The capabilities that make agents useful also make them more difficult to evaluate. Here are evaluation strategies that have worked across real-world deployments.
> https://t.co/UD0yGglTU0

- **Tweet:** https://x.com/AnthropicAI/status/2009696515061911674
- **What:** Anthropic engineers share practical evaluation strategies for AI agents, covering techniques that have proven effective in real-world deployments and addressing the unique challenges of evaluating agent behavior at scale.

---


## @elithrar - Code review command and subagent shared
> and because I'm not a monster, the (slightly tweaked) versions of the command + subagent can be found here: https://t.co/nScOGxdUMm + https://t.co/5NiR5hzojx

- **Tweet:** https://x.com/elithrar/status/2009756449304457488
- **What:** Matt shares dotfiles with a code review command and subagent that runs three parallel code review agents with temperature 0.1, improving on single-agent approaches for code quality feedback.

**Context (reply to):** Matt highlights that multiple code review sub-agents running in parallel with low temperature settings outperforms a single reviewer, demonstrating practical improvements in code review quality.

---


## @virattt - Dexter: Autonomous financial research agent
> Code: https://t.co/1gaV4Hg4H4

- **Tweet:** https://x.com/virattt/status/2009757256208793660
- **What:** Virat shares the open-source code for Dexter, an autonomous financial research agent that performs analysis using task planning and self-reflection similar to Claude Code but specifically built for finance applications.

**Context (reply to):** Dexter can find undervalued stocks, analyze them in detail, and build investment theses, with the bonus capability of running on local LLMs for privacy and cost efficiency.

---


## @bubbleboi - The Girl Dinner trade thesis
> No.. this is the market is pricing in the effect of Ozempic drugs being widespread, cheap, and administered orally.
>
> This is a huge secular trend. I'm calling it the Girl Dinner trade. Long sexy clothing, cosmetics, & filler. Short liquid desert and fast casual salad bowl slop!
>
> Look at the past 6 months.

- **Tweet:** https://x.com/bubbleboi/status/2009757467484565998
- **What:** Market analysis connecting GLP-1 drug adoption trends to sector rotation, with investment implications for health, wellness, and lifestyle consumption patterns driven by widespread Ozempic availability.

**Quoted from:** Victoria's Secret (VSCO) rallying 230% since announcing Fashion Show return, framed as a generational wealth opportunity.

---


## @DennisonBertram - Claude Code skill for React component extraction
> @da_fant I gave this to Claude and he made it a skill AND created a React-Grab style navigator to help you select elements (and optionally use React Grab!)
>
> https://t.co/jjuUWgZGSR https://t.co/bKRIBuinVe

- **Tweet:** https://x.com/DennisonBertram/status/2009757479211585664
- **What:** Dennison shares a Claude Code skill suite that extracts React components directly from production websites using React Fiber internals, including a visual navigator for interactive component selection and optional React Grab integration.

**Context (reply to):** Building on the React Fiber component extraction technique, which can extract exact 1:1 components including styling, props, and design systems without needing source code access.

---

---

## @udiWertheimer - Vibe Coding Roblox Games

> the only thing you should be vibe coding is roblox games
>
> absolutely insane that there aren't more people talking about this

- **Tweet:** https://x.com/udiWertheimer/status/2009786299360649549
- **What:** A take on vibe coding being well-suited for Roblox game development.

---


## @thdxr - OpenCode v1.1.11 ChatGPT Integration

> in opencode v1.1.11
>
> you can now use your ChatGPT Plus/Pro plans in OpenCode
>
> /connect to set it up

- **Tweet:** https://x.com/thdxr/status/2009803906461905202
- **What:** Announcing OpenCode v1.1.11 with new support for ChatGPT Plus/Pro accounts via the /connect command.

---


## @nateberkopec - Moving to fnox for Secrets Management

> I'm moving to fnox for secrets management. I'm growing concerned about agents rogue-reading secrets out of files, so I'm using fnox to keep secrets inside 1Password and requiring TouchID to unlock. Great integration with mise ofc, which I already use.

- **Tweet:** https://x.com/nateberkopec/status/2009873774909575440
- **What:** Migrating to fnox for secure secrets management integrated with 1Password and mise, addressing concerns about agents accessing secrets from files.

---

---



---


# Thursday, January 8, 2026

## @jarrodwatts - Claude Code Configuration Repository

> Link is here: https://t.co/BXJ1holxRN

- **Tweet:** https://x.com/jarrodwatts/status/2009200865694114248
- **What:** A comprehensive personal Claude Code configuration repository including agents, commands, hooks, rules, skills, and plugins for enhanced development workflow. The repo provides installation options and includes tools like codebase search, media interpretation, and custom commands.

**Reply Context:**
> I just open sourced my claude-code-config repo.
>
> It includes all of my agents, commands, hooks, rules, skills, and  plugins that i've made or collected over the past few months.
>
> It's nothing fancy - just simple but effective enhancements that i'll continue to update over time.
> — @jarrodwatts

---


## @mitsuhiko - Linting for Unique Function Names

> I'm now lint enforcing unique function names and I immediately found a handful of 100% duplicated functions declarations. Nice :)

- **Tweet:** https://x.com/mitsuhiko/status/2009241885584531578
- **What:** A note about implementing linting rules to enforce unique function names across a codebase, which revealed multiple duplicate function declarations that needed cleanup.

---


## @ndbroadbent - jscpd for Copy-Paste Detection

> @mitsuhiko I highly recommend jscpd: https://t.co/QXFxnjqjgy
>
> Can't live without this in my projects now

- **Tweet:** https://x.com/ndbroadbent/status/2009251665161888180
- **What:** jscpd is a copy/paste detector for programming source code supporting 150+ formats, implementing the Rabin-Karp algorithm to find duplicated blocks of code. A recommended tool for identifying and managing code duplication in projects.

**Reply Context:**
> I'm now lint enforcing unique function names and I immediately found a handful of 100% duplicated functions declarations. Nice :)
> — @mitsuhiko

---

---

## @alxfazio - Hook Development Skill Update for Claude v2.1.0
> gist: https://t.co/PzsSvs0dgx

- **Tweet:** https://x.com/alxfazio/status/2009259570611241303
- **Parent Context:** cc v2.1.0 is out and it brings some great changes to hooks. so i've updated the official anthropic skill for creating hooks to include the latest guidance on how to implement the new features. use it to modernize your hooks with a query like `please use the hook-development skill to help me understand how i can refactor my hooks to maximize the value of the changes in claude v2.1.0+` gist below
- **What:** Alex Fazio shared an updated GitHub gist with the latest best practices for implementing hooks in Claude v2.1.0+, including new guidance on how to leverage the latest features.

---


## @simonecanciello - Build Apps for Women Business Strategy
> this is why i keep saying "build apps for women".
>
> they actually spend money.
>
> > check sensortower
> > find 2 or 3 apps doing $100k+
> > rebuild a women-first version
>
> add a mascot + adapt the vibe.
>
> it works every time. https://t.co/S3bnVMhTK1

- **Tweet:** https://x.com/simonecanciello/status/2009305167963779379
- **Quote Context:** Simone Canciello is responding to Lotanna Ezeike's tweet about launching an app with games for girls that generates $400,000 a month. Lotanna noted how "just launched an app with only games for girls" was criticized as sexist, yet became highly profitable.
- **What:** Simone provides a practical strategy for app monetization: identify successful apps on Sensor Tower, rebuild a women-first version with a mascot and adapted aesthetic. This approach appears to work consistently for generating substantial revenue.

---


## @leocooout - Claude File Search Optimization with Custom Indexing
> hoje fiz uma exploração e reduzi o tempo de busca por arquivos na codebase do tiktok de quase 8s pra menos de 200ms. mencionar qualquer arquivo no claude é praticamente instantaneo agora
>
> a configuração padrão do fast filesystem traversal é boa pra projetos menores mas pra projetos de larga escala é recomendado um sistema próprio de indexação
>
> o claude deixa você customizar essa configuração pelo settings.json
>
> {
>   "fileSuggestion": {
>     "type": "command",
>     "command": "~/.claude/file-suggestion.sh"
>   }
> }

- **Tweet:** https://x.com/leocooout/status/2009337600742707335
- **What:** Leo shared how custom file indexing configuration in Claude settings.json reduced file search time in TikTok's codebase from ~8s to <200ms. The default fast filesystem traversal works well for smaller projects but large-scale codebases benefit from custom indexing systems.

---


## @jediahkatz - Semantic Search Advantage for Large Codebases
> Cursor has found semantic (vector) search to be the differentiator here. In large codebases, pure grep can break down by failing to find related concepts, especially in big companies where there might be a lot of jargon.
>
> You might say "find the utility that predicts the next prompt" and then it greps for predict, next, prompt, utility -- but the actual thing was called "Suggestion Service" and the only match was from "next" which matched a million other things.
>
> Semantic search would nail this. We ran an A/B test and published our findings here: https://t.co/d4uOwCJZ0Z

- **Tweet:** https://x.com/jediahkatz/status/2009343675399131334
- **Parent Context:** Jediah is responding to Igor Babuschkin's observation about Claude Code's limitations with large codebases, noting that it was likely post-trained mostly on smaller repos and would benefit from continual learning or fine-tuning on specific repositories.
- **What:** Cursor's semantic (vector) search outperforms grep-based search in large codebases with company-specific jargon. They provide a concrete example of how grep fails to find the "Suggestion Service" when searching for "next prompt utility," but semantic search handles this correctly. A/B testing confirmed this advantage.

---


## @dani_avila7 - Claude Code 2.1.1 Skills with Direct Hook Support
> Discovering more options in Claude Code 2.1.1
>
> Skills now support Hooks directly in the YAML frontmatter.
>
> In addition to a Skill being able to reference another Skill, you can now add hooks to run commands or scripts on PreToolUse, PostToolUse, or Stop events.
>
> This keeps unlocking more powerful agent-based workflows.

- **Tweet:** https://x.com/dani_avila7/status/2009397544565305705
- **Quote Context:** Daniel is sharing a new feature in Claude Code 2.1.1 that builds on his previous tweet about the /plan feature and Plan Mode for designing implementation strategies before execution.
- **What:** Claude Code 2.1.1 now allows Skills to define Hooks directly in YAML frontmatter, enabling commands/scripts to run on PreToolUse, PostToolUse, or Stop events. This enhances agent-based workflows with more flexible automation capabilities.

---

---


## @thayto_dev - Faster Claude Code File Suggestions with Custom Script

> quick guide to improve and make faster your Claude Code file suggestion
>
> before all you have to install ripgrep, jq, fzf
>
> Add this to your ~/.claude/settings.json
> ```json
> "fileSuggestion": {
>   "type": "command",
>   "command": "~/.claude/file-suggestion.sh"
> },
> ```
>
> create this file ~/.claude/file-suggestion.sh then add this:
>
> ```sh
> #!/bin/bash
> # Custom file suggestion script for Claude Code
> # Uses rg + fzf for fuzzy matching and symlink support
>
> # Parse JSON input to get query
> QUERY=$(jq -r '.query // ""')
>
> # Use project dir from env, fallback to pwd
> PROJECT_DIR="${CLAUDE_PROJECT_DIR:-.}"
>
> # cd into project dir so rg outputs relative paths
> cd "$PROJECT_DIR" || exit 1
>
> {
>   # Main search - respects .gitignore, includes hidden files, follows symlinks
>   rg --files --follow --hidden . 2>/dev/null
>
>   # Additional paths - include even if gitignored (uncomment and customize)
>   # [ -e .notes ] && rg --files --follow --hidden --no-ignore-vcs .notes 2>/dev/null
> } | sort -u | fzf --filter "$QUERY" | head -15
> ```
>
> then in your terminal:
> ```sh
> chmod +x ~/.claude/file-suggestion.sh
> ```
>
> be happy :)

- **Tweet:** https://x.com/thayto_dev/status/2009401734213554494
- **What:** Guide to optimize Claude Code's file suggestion feature using ripgrep, jq, and fzf for faster fuzzy file matching with symlink support.
- **Quoted:** @leocooout demonstrated reducing file search time from 8 seconds to 200ms on TikTok's codebase using custom file suggestion configuration.

---

---



---


# Wednesday, January 7, 2026

## @irl_danB - Building an LSP for prose, but models are excellent at reading/writing it
> built an LSP for it, but not deployed or shipped anywhere yet.

this was the first thing I did, but most people who are using it don't even write or look at the `.prose` file itself!

the model is really good at writing it and reading it, and that's all you really need bizarrely enough. so LSP on the back burner now.

I anticipate the next obvious question then is:

why have the language at all if it's just prompt => .prose => orchestration?

ie why not just prompt => orchestration?

for whatever reason, the `.prose` file (and `https://www.prose.md/` prefix that goes along with it) allows the model to be more expressive and specific

- **Tweet:** https://x.com/irl_danB/status/2008982955234894187
- **Links:** [[prose.md]]
- **What:** Development insights on prose, a natural language programming language. While an LSP was initially built, users don't actually interact with the `.prose` files—models write and read them perfectly. The language's structured format enables better model expressiveness despite seeming redundant when prompt-to-orchestration could theoretically suffice.

---


## @HipCityReg - Situation Monitor: Aggregated global activity dashboard
> Welcome to "Situation Monitor"

> Global Activity Monitor
> @tbpn livestream
> Intel Feed
> Tech/Finance/Politics newsfeed
> Stocks/Crypto
> @Polymarket  predictions
> Tech layoffs tracker
> AI Race news
> Is the Fed printer on?
> Venezuela + Greenland

- **Tweet:** https://x.com/HipCityReg/status/2009003048044220622
- **Links:** [[situation-monitor]]
- **What:** A comprehensive real-time monitoring dashboard aggregating global activity across multiple domains: geopolitical events (Venezuela, Greenland), financial markets, tech news, AI developments, and predictions. Combines feeds from livestreams, Intel, markets, and Polymarket for situational awareness across interconnected systems.

---


## @steipete - Ask "How do we organize this?" after shipping features
> After you weaved a new feature in, always ask this.

Biggest unlock to keep the codebase organized.
codex is really great at understanding pain points.

- **Tweet:** https://x.com/steipete/status/2009006882560889034
- **What:** A simple but powerful practice: after implementing features, take time to refactor and reorganize. This prevents codebase decay and keeps the system maintainable. Using tools like Codex to identify pain points accelerates finding organizational issues.

---


## @bcherny - Claude Code 2.1.0 released with major feature additions
> Claude Code 2.1.0 is officially out! claude update to get it

We shipped:

- Shift+enter for newlines, w/ zero setup
- Add hooks directly to agents & skills frontmatter
- Skills: forked context, hot reload, custom agent support, invoke with /
- Agents no longer stop when you deny a tool use
- Configure the model to respond in your language (eg. Japanese, Spanish)
- Wildcard support for tool permissions: eg. Bash(*-h*)
- /teleport your session to https://claude.ai/code
- Overall: 1096 commits

https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md

If you haven't tried Claude Code yet: https://code.claude.com/docs/en/setup

Lmk what you think!

- **Tweet:** https://x.com/bcherny/status/2009072293826453669
- **Links:** [[claude-code]]
- **What:** Major release of Claude Code (v2.1.0) with significant UX improvements and features. Key additions include better newline handling, agent hooks, skills improvements with hot reload and custom agents, multilingual response support, and flexible tool permissions. Over 1000 commits in this version representing substantial development effort.

---

---

## @koylanai - SpecStory for Context Compression with Claude Opus 4.5

> I wish I had known this before. I'm a huge fan of SpecStory now.
>
> It's a plugin that automatically converts your conversation histories, including tool calls and reasoning traces, into Markdown format.
>
> When Opus 4.5 approaches to context compaction limit, run Gemini 3 in the history document and improve the coding models' context without bloating it.

- **Tweet:** https://x.com/koylanai/status/2009157424469438967
- **What:** SpecStory is a plugin that converts conversation histories with tool calls and reasoning traces into Markdown format, enabling efficient context compression for Claude Opus 4.5 by saving conversations as files that can be referenced in new sessions.

**Quoted Context:**
> everyone building or seriously using agents knows by now that context compression is lossy
>
> agents are good at filesystems, which is why saving conversations as markdown files turns out to be the most reliable approach
>
> i have found this flow to work the best for me. once i am about to hit the context limit, i start a new session and explicitly ask the agent to refer to the main session's markdown file for grounded context. whenever the agent needs elevant context that was discussed in the main session about the scope, failures, or certain decisions, it can just search the markdown file and pull in only the relevant fragments. that way, we are also saving on the tokens and only bringing context that's relevant.
>
> i guess the bet with @specstoryai around conversations-as-artifacts is working perfectly now. probably this is the correct abstraction for long-running, agent-assisted development.
> — @doesdatmaksense

---

---



---


# Tuesday, January 6, 2026

## @jarrodwatts -
>

- **Tweet:** https://x.com/jarrodwatts/status/2008495347115630701
- **What:** Link to another tweet.

---


## @living_energy - EMF Exposure and Collagen Degradation in Athletes
> Low-frequency electromagnetic fields can degrade collagen, weaken tendons, and cause soft-tissue damage at levels regulators call "safe."
>
> We have a real world case study proving this:
>
> An NFL team whose practice facility sits next to a massive electrical substation.
>
> THREAD

- **Tweet:** https://x.com/living_energy/status/2008604095188529215
- **Link:** https://peteranthonycowan.substack.com/p/could-chronic-emf-exposure-from-a
- **Filed:** [emf-health-effects.md](./knowledge/articles/emf-health-effects.md)
- **What:** Deep investigation into low-frequency AC magnetic fields causing non-thermal biological damage, with the 49ers' epidemic of tendon ruptures as a real-world case study of chronic EMF exposure from a nearby electrical substation.

---


## @trq212 - Automated Verification via Subagent Spec Review
> one of the benefits of a detailed spec is that verification is also easier, after the work is done I like to add:
>
> "spin up a subagent to read the spec file and verify if work has been completed, have it give feedback if not and then address the feedback"

- **Tweet:** https://x.com/trq212/status/2008610538763559356
- **Quoted:** https://x.com/trq212/status/2005315275026260309
- **What:** Thariq advocates for automated verification of spec completion using a subagent to review work against the spec document, providing feedback on incomplete items before final submission.

---

---

## @The_Whole_Daisy - Claude Code Ralph Wiggum Prompt Technique
> So apparently @GeoffreyHuntley's Ralph Wiggum technique (and our Claude Code plugin for it) went a little viral over the holidays? I thought I'd share a typical prompt I use with it. All of the instructional videos I've seen don't give thorough enough completion promises, IMHO https://t.co/q6BsobYaUF

- **Tweet:** https://x.com/The_Whole_Daisy/status/2008625420741341355
- **What:** Discussion of the viral Ralph Wiggum prompt technique for Claude Code, sharing practical prompt approaches and criticizing incomplete instructional coverage.

---


## @veggie_eric - Internal AI Transformation Role in Companies
> Every company should hire an internal AI transformation person. No need for a fancy title like Head of AI. Just give them full latitude to clean up inefficiencies across sales, hr, finance, etc. There's so many manual workflows and arcane bs that can easily be fixed with LLMs

- **Tweet:** https://x.com/veggie_eric/status/2008628192509383018
- **What:** Recommendation for companies to hire dedicated AI transformation roles to systematically eliminate manual workflows and inefficiencies across departments using LLMs.

---


## @_catwu - Claude Code Local Desktop Implementation
> Docs here: https://t.co/vzjRiNWaG3

S/o @amorriscode and @alicelovescake1 who built this!

> **Parent context:** If want to use Claude Code but are don't like the terminal interface, you can now use local Claude Code from Claude Desktop!

To do so:
1. download Claude Desktop
2. open the sidebar and click 'Code' toggle
3. select the folder that you want Claude Code to have access to
4. submit your prompt!

- **Tweet:** https://x.com/_catwu/status/2008628739572134270
- **What:** Documentation link and credits for Claude Code integration in Claude Desktop, enabling local code execution without terminal interface.

---


## @hutchinson - 2026 Progress Overview
> Just to give you a sense of where things are at in 2026 https://t.co/X9AiDL5m32

- **Tweet:** https://x.com/hutchinson/status/2008638005674995818
- **What:** Contextual snapshot of AI/tech progress and state of the art in early 2026.

---


## @jediahkatz - Dynamic Context Engineering in Cursor
> I wanted to share more on our context engineering work in Cursor and how we're adapting to the improved capabilities of agent models.

We've transitioned from a paradigm of static context (prompt stuffing, tons of tools in system prompt) to a new world where agents are much better at searching for information and maintaining consistency over long sessions — allowing us to take fuller advantage of dynamic context.

> **Quote context:** Cursor's agent now uses dynamic context for all models.

It's more intelligent about how context is filled while maintaining the same quality. This reduces total tokens by 46.9% when using multiple MCP servers. https://t.co/PhBkV6foum

- **Tweet:** https://x.com/jediahkatz/status/2008644735267991741
- **What:** Technical perspective on evolution from static context prompting to dynamic context approaches in agent systems, enabling better information search and consistency.

---

---

## @0xRaduan - Engineers adapting to AI will have advantages over those who don't
> I think there will be a disparity in terms of engineers that adapt to ai and those who don't.

Once everything uses AI, there will still be levels in how you do it, and at the end of the day it's a multiplier of knowledge, so I think it affects job market, but not in the ways media writes about it.

- **Tweet:** https://x.com/0xRaduan/status/2008645611273458138
- **What:** Thoughtful perspective on AI's impact on engineering jobs. Rather than wholesale job displacement, AI acts as a multiplier of knowledge—those who adapt will thrive, but there will still be skill differentiation. The disruption will look different from media narratives.

---

---



---


# Monday, January 5, 2026

## @aidenybai - Repogrep: Ultra-Fast Public GitHub Repository Search
> introducing repogrep.​com
>
> ultra fast codebase search for any public github repo
>
> where i found the React hooks source code in &lt;10 sec https://t.co/2xYi77LMTE

- **Tweet:** https://x.com/aidenybai/status/2008222085240549530
- **What:** A tool announcement for Repogrep.com, an ultra-fast search engine for public GitHub repositories that enables rapid code discovery across any open-source project.

---


## @doodlestein - Planning Large-Scale AI Projects with Iterative Refinement
> *Replying to @badlogicgames:* Could you share a real world project + the plan you came up with? I've been building software for over 25 years, and I was never able to do "hyper-waterfall", as in: preplan everything to a detail level that allows mechanical execution like that.
>
> As you work on a project, problems you didn't anticipate pop up. I don't understand how that is solved.
>
> Here's a recent example from my cass memory project (see quoted post for the whole process which I posted about live as I did it):
>
> https://t.co/Dn2x6YQPMQ
>
> Once you've implemented the entire plan (after turning it into beads and so forth), you have a version 1 that should be usable if you've done things well. It will probably require some bug fixes and UI polishing, but that's just part of my workflow.
>
> Then after using it, you might decide that you missed some things or have ideas for other features. Well, then you create another big plan, like I did here in the same project; nothing says you can only ever do one plan and then that's it:
>
> https://t.co/sQN2HJDc5B
>
> *Quoting @doodlestein:* OK, status update. Starting from absolutely nothing ~5 hours ago except a big ol' plan document, I turned that into over 350 beads (we got a bunch of new testing beads), I now have conjured up ~11k lines of code, about 8k of which is the core code and the rest is testing code (see screenshot).
>
> Around 204 commits so far. Probably at least 25 agents have been involved at some point or other.
>
> If you want to look at the actual Agent Mail messages, I used the handy export feature to publish this as a static website you can see here:
>
> https://t.co/QKP9dCfwTq
>
> So how far did we get already? You can see Claude's full assessment in the attached screenshot. Here's its bottom line conclusion, though:
>
> Key Insights
>
>   1. The product is USABLE NOW - 151 tests pass, binary compiles, all core commands work. The closed rate understates this because open issues are heavily weighted toward testing.
>   2. Testing is the biggest gap - ~40% of remaining work. This is actually good news
>    - it means implementation is largely done and what remains is verification.
>   3. High velocity - 2.9 hour average lead time shows issues get completed, not stalled.
>   4. Phases 2-4 are future work - Advanced features (local semantic search, decision  logging, starter playbooks) are explicitly deferred.
>   5. The 14 open epics are misleading - Most are testing-focused sub-epics or future  phases, not blockers.
>
> Bottom Line
>
> For a "can I use this tool effectively" definition: ~85-90% done.
>
> The core ACE pipeline (Generate context → Reflect on sessions → Curate playbook →
>   Validate scientifically) is complete and functional. What remains is mostly test  coverage, polish, and future-phase features.
>
> If this were a startup product, you'd say: "MVP shipped, now hardening for production."

- **Tweet:** https://x.com/doodlestein/status/2008226781870854531
- **Link:** https://github.com/Dicklesworthstone/cass_memory_system
- **Parent:** https://x.com/badlogicgames/status/2008223886857343391
- **Quoted:** https://x.com/doodlestein/status/1997853884442681719
- **Filed:** [cass-memory.md](./knowledge/tools/cass-memory.md)
- **What:** Jeffrey Emanuel demonstrates how to overcome "hyper-waterfall" planning limitations by treating large projects as iterative refinements: build a complete version from a detailed plan, then create additional plans for improvements and new features. Shows real example with the cass-memory system reaching MVP status in ~5 hours with multi-agent AI assistance.

---


---



## @mdo - Diffs: Open Source Diff and Code Rendering Library

> Let me introduce y'all to Diffs—a new, open source diff and code rendering library. We've been working on it @pierrecomputer for a few months now and we're stoked for you to see it. https://t.co/G0ehctDaiY

- **Tweet:** https://x.com/mdo/status/2008312716050747403
- **What:** Announcement of Diffs, an open source library for rendering diffs and code, developed collaboratively with Pierre Computer.

---

---

## @banteg - AI-Assisted Spec-to-Implementation Workflow
> start from a spec, just yap into gpt pro and create a good spec. talk with claude/codex about it and update it till their understanding matches yours. claude has a nice interview tool.
>
> then put it back in gpt pro and create an implementation plan. give it to codex gpt-5.2-codex xhigh and ask to see it to completion. unlike claude, it usually does.
>
> i guarantee it would give you a better starting point from which you could use claude if you prefer.

- **Tweet:** https://x.com/banteg/status/2008315551290978631
- **Parent:** https://x.com/ThePrimeagen/status/2008261459630059720
- **What:** Banteg describes a hybrid workflow using GPT Pro for spec creation, Claude for refinement via its interview tool, and Codex for implementation, recommending this approach over pure Claude vibe coding.

---


## @hud_zah - PR Reviews via LLM Prompt Chains
> a mockup: doing PR reviews by seeing a programmers chain of prompts!
>
> it also encourages devs to be deliberate with how they instruct llms as they become more capable, and poor human instructions + context ends up being the reason why code doesn't work

- **Tweet:** https://x.com/hud_zah/status/2008352007174697425
- **What:** Proposes a novel code review methodology that examines the LLM prompt chains developers used, incentivizing clearer instruction writing and better context-passing as a key failure point in LLM-assisted development.

---

---



---


# Sunday, January 4, 2026

## @trq212 - AI alignment and interpretability resources
> If you started using Claude Code over the holidays, you might be curious about how AI actually works, the benefits and risks, and where it's headed. Here are some of my favorite papers on alignment, interpretability, and societal impacts

- **Tweet:** https://x.com/trq212/status/2007903193158881323
- **What:** Curated collection of papers on AI alignment, interpretability, and societal impact for those exploring Claude Code.

---


## @andyorsow - Claude Code use case uncertainty
> Feeling like I should be using Claude Code but have no idea exactly what I should be using it for. Just a bundle of non-technical FOMO over here.

- **Tweet:** https://x.com/andyorsow/status/2007931911847719290
- **What:** Expression of uncertainty about practical applications for Claude Code despite wanting to use it.

---


---


## @banteg - Official bunny devcontainer with Claude and Codex
> official bunny devcontainer just dropped
>
> run claude code and codex in yolo mode. isolated, unattended, auth persists across all your repos via shared docker volumes.

- **Tweet:** https://x.com/banteg/status/2007748646230733139
- **Link:** https://github.com/banteg/agents
- **What:** Development of open-source agent workflows including git worktree helpers (git-wt, worktrunk) and devcontainer setup for running AI agents like Claude Code and Codex in isolated environments with authentication persistence.

---


## @gakonst - Rekordbox waveform analysis web app
> also my entire feed is people talking about their vibe coding setup and tools for improving their vibe coding setup - what fun thing did you build recently?
>
> i spent some time recently building an open source version of rekordbox's waveform analysis w/ a web app on cf workers
>
> *Quoting @gakonst:* IME testing out my own agents files and cloning others' franken-agent files / skills repos, less is more and most over-engineered agent files or skill directories are hurting your speed

- **Tweet:** https://x.com/gakonst/status/2007836229279363510
- **Quoted:** https://x.com/gakonst/status/2007831002660659511
- **What:** Open source waveform analysis tool built as a web app on Cloudflare Workers, inspired by Rekordbox. Reflects on the trend of vibe coding setups and agent workflow optimization.

---


## @mohamede1945 - Codex performance improvement with agents.md
> Codex feels faster after I've adopted @steipete's agents .md from agent-scripts repo and some of his config described https://t.co/Z8bM3q3T5h
>
> Smaller tasks that used to take 2-5 mins is now always under 1 min. Maybe the telegraph style makes it faster?
>
> and ofc I added the motivational 1-liner

- **Tweet:** https://x.com/mohamede1945/status/2007844824934691260
- **Link:** https://steipete.me/posts/2025/shipping-at-inference-speed
- **What:** Performance improvement in Codex using optimized agents configuration from @steipete. Tasks reduced from 2-5 minutes to under 1 minute, attributed to telegraph-style structured prompts.

---


## @moreconfetti - Every's compound engineering approach
> *Replying to @moreconfetti:* https://t.co/aG6odRE5we
> @steipete is making waves with his Clawdbot project. Understand how he works and why he prefers Codex over Claude Code:
>
> https://t.co/dJbCiXKYjL
> @every has developed one of the best engineering toolkits for @claudeai (especially useful for my Rails projects) and @danshipper is a must follow for AI thought leadership in 2026

- **Tweet:** https://x.com/moreconfetti/status/2007866139007975435
- **Parent:** https://x.com/moreconfetti/status/2007866137191805130
- **Link:** https://every.to/chain-of-thought/compound-engineering-how-every-codes-with-agents
- **What:** Every.to's compound engineering methodology for AI-assisted software development. A four-step process optimized for teams working with AI agents, particularly relevant for Rails development.

---


## @moreconfetti - Claude Code 2.0 guide and Opus 4.5 workflows
> *Replying to @moreconfetti:* https://t.co/aG6odRE5we
> @steipete is making waves with his Clawdbot project. Understand how he works and why he prefers Codex over Claude Code:
>
> https://t.co/ynIhEjZp42
> @dejavucoder gives some good perspective on the shift in capabilities and workflows in the second half of 2025

- **Tweet:** https://x.com/moreconfetti/status/2007866140840882636
- **Parent:** https://x.com/moreconfetti/status/2007866139007975435
- **Link:** https://sankalp.bearblog.dev/my-experience-with-claude-code-20-and-how-to-get-better-at-using-coding-agents/
- **What:** Deep dive into Claude Code 2.0 features, Opus 4.5 workflows, and context engineering. Covers sub-agents, MCP servers, hooks, skills, and practical tips for maximizing AI-assisted coding productivity. Analysis of capability shifts in H2 2025.

---

---


## @moreconfetti - Clawdbot vs Claude Code: Shipping Code at Inference Speed
> PSA for a CTO, Head of AI, VP/Dir of Engineering, CXO:
> This is going to be one of the most important "back to work" weeks of your career. You must get your team aligned on agentic dev ASAP. If you're feeling behind or overwhelmed, here are some good reads to get you inspired 🧵
>
> *Replying to @moreconfetti:* PSA for a CTO, Head of AI, VP/Dir of Engineering, CXO:
> This is going to be one of the most important "back to work" weeks of your career. You must get your team aligned on agentic dev ASAP. If you're feeling behind or overwhelmed, here are some good reads to get you inspired 🧵
>
> @steipete is making waves with his Clawdbot project. Understand how he works and why he prefers Codex over Claude Code:

- **Tweet:** https://x.com/moreconfetti/status/2007866137191805130
- **Link:** https://steipete.me/posts/2025/shipping-at-inference-speed
- **Parent:** https://x.com/moreconfetti/status/2007866135547646039
- **What:** An article about shipping code at inference speed, exploring how Clawdbot enables rapid development cycles and comparing different approaches to agentic coding.

---


## @mattpocockuk - The Ralph Wiggum Approach to Long-Running AI Coding Agents
> There's an AI coding approach that lets you run seriously long-running AI agents (hours, days) that ship code while you sleep. I've tried it, and I'm not going back.
>
> It's the Ralph Wiggum approach. Here it is in a nutshell:
>
> Run a coding agent with a clean slate, again and again until a stop condition is met.
>
> The Bash Script
>
> Running ralph involves a single bash script.
>
> 1. Set up a bash for loop that runs a set number of times, let's say 10. You choose a finite number to prevent the agent running infinitely.
> 2. Inside the loop, you get the coding agent (Claude Code, OpenCode, Codex etc) to work on a single feature in the repo until that single feature is done. You prompt it to say "if, after implementing, there is no further work to be done, reply with <promise>COMPLETE</promise>".
> 3. Check for <promise>COMPLETE</promise> inside the loop and exit early if it exists.
>
> The Stop Condition
>
> How does the LLM know when to emit <promise>COMPLETE</promise>? There are multiple approaches:
>
> - Raw Prompting: Just pass a very clear stop condition to the prompt inside the bash loop. "The job is complete when X conditions are met"
> - TODO list: Give the agent a TODO list to complete
> - PRD: My preferred approach, explained below
>
> Progress Reports
>
> In your prompt, you MUST tell the agent to commit its work, and append its progress to a local progress.txt file.
>
> Committing its work allows future agents to navigate what was done via the git history.
>
> The progress.txt is a standard long-running agent practice. Feed it in to the agent via the prompt, and use the verb 'append' to make sure it doesn't update previous entries.
>
> Keep CI Green
>
> Each commit MUST pass all tests and types. This means you have to prompt the agent to run typechecks and tests on each commit.
>
> If you don't do this, you're hamstringing future agent runs with bad code, and they'll need to bisect to find bugs. Super nasty.
>
> This means that building really healthy feedback loops is CRITICAL to Ralph's success.
>
> The PRD
>
> Two problems immediately emerge with Ralph.
>
> The first is that the agent picks tasks which are too large. They don't scope the amount of work correctly and they try things which are too ambitious. This means they run out of context window and just end up failing.
>
> The second is that the agent doesn't know when to stop.
>
> To solve this, I use a PRD-based approach that formalizes the work I want Ralph to complete in a list of user stories.
>
> It's a mix of a PRD and a TODO-list, where the PRD is a JSON file of user stories with 'passes: false'.
>
> I then prompt the agent to pick the highest priority feature, and ONLY work on that feature. It then updates the passing status of the relevant PRD item at the end.
>
> This scopes it down extremely effectively, meaning it utilizes only a small part of its context window, and thus isn't swamped by context rot.
>
> Summary
>
> - Bash script
> - JSON-based PRD
> - progress.txt
> - Keep CI green
> - Feedback loops
>
> You'll have an AI coding setup that can ship while you kip.

- **Tweet:** https://x.com/mattpocockuk/status/2007924876548637089
- **What:** A detailed guide to running long-duration AI coding agents using the "Ralph Wiggum approach" with bash scripts, PRD files, and clean stop conditions to enable autonomous feature development while maintaining code quality.

---


## @doodlestein - Clawdbot, ACIP, and Securing AI-Powered Personal Assistants
> OK, I'm normally in such a rabbit hole of my own crazy schemes, so I finally got around to installing and setting up @steipete 's Clawdbot project, which I have like 20+ different X bookmarks for because I've been meaning to try it for so long.
>
> And, wow. This is so unbelievably cool. Of course, I simply cloned the repo and had my buddy Claude Opus install and configure it all for me, which was very easy.
>
> Then I started going a little wild adding more and more integrations to it, many of which are included out of the box using various other utilities that Peter has made in his prodigious bursts of creation these past few months.
>
> But then I started inquiring about other things for which there were no integrations, like Cloudflare's wrangler utility, or the vercel cli. And it turns out that it's incredibly easy to add new skills to Clawdbot, so I started doing just that.
>
> Then I realized I could teach Clawdbot about all of my Agent Flywheel tools like cass and bv, and then some of my other random new tools like giil. I made a repo with all that stuff you can see here:
>
> https://t.co/3KoXwIuQUf
>
> But the thing I'm most excited about is that Clawdbot is THE perfect use case for this "acip" idea I've been thinking about for the past year:
>
> https://t.co/hKABLkavor
>
> That stands for "Advanced Cognitive Inoculation Prompt" and it's basically the idea that you can reduce the attack surface and make a system a lot more robust to most prompt injection attacks through prompting, at least compared to a naive system without anything like that.
>
> Obviously any system like that is intrinsically flawed, but dismissing it feels to me like saying you shouldn't even bother to lock your front door when you go on vacation because someone could pick the lock. Sure, but it doesn't hurt, doesn't cost much to do, and reduces the chances of some casual intruder getting in and robbing you.
>
> Anyway, I first created that 9 months ago, and models have gotten a lot better since then. So I went to work with GPT Pro 5.2 in the web app and also Opus 4.5 to revise and enhance the ACIP prompt itself. You can see in the readme file all the changes that were made and why.
>
> ACIP is just English text, not code, so anyone could read it and hopefully understand how it works. And even though it has obvious shortcomings (a robust defense requires something external to the main model, like a second, independent "audit model" that is checking everything over before sending it to the main model; I discuss many of the problems that come up in this sort of thing in this article I wrote ~2 years ago: https://t.co/V5od2x9ZG4 )
>
> But as I said in the quoted post, I feel like the time has finally come for ACIP, because now users like me are voluntarily hooking up LLMs to highly sensitive parts of their life, like emails, iMessage, Telegram, etc. And what's different now is also that Clawdbot can be accessed remotely via Telegram and other methods.
>
> Sure, I have my Telegram integration locked down to just me, but one could imagine various scary security situations where an unauthorized attacker could be communicating with an LLM-based agent that has full rein of my computer but also my entire digital life.
>
> And you want that agent to have a high degree of mental fortitude, and not fold like a cheap lawn chair as soon as some slick character comes along and does some social engineering attack, or tries to use role play or stories or any number of creative and clever techniques designed to trip up and fool our robot brethren.
>
> Anyway, in the acip readme you will find a curl bash one-liner that sets it up with Clawdbot to protect you. It uses more tokens and increases latency somewhat, but I think it's worth it given how much chaos could conceivably be caused by a fully set up Clawdbot getting hijacked by an attacker.
>
> *Quoting @doodlestein:* I made this project 9 months ago and it didn't generate much interest at the time, but perhaps its time has finally come now with the rise in popularity of personal assistant projects that use LLMs, such as @steipete 's venerable Clawdbot (née Clawdis):
>
> https://t.co/RfsIkhKhdO

- **Tweet:** https://x.com/doodlestein/status/2007996215892336924
- **Tags:** [[clawdbot]] [[ai-security]] [[acip]] [[agentic-coding]]
- **Link:** https://github.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations
- **Quoted:** https://x.com/doodlestein/status/2007910745980481780
- **What:** A comprehensive exploration of integrating Clawdbot with custom skills and introducing the Advanced Cognitive Inoculation Prompt (ACIP) as a security layer to defend personal AI assistants against prompt injection attacks.

---


## @NickADobos - Turning Codebase Sections into Agent-Discoverable Skills
> Wait this is an interesting idea.
>
> Turn sections of your code base into skills.
> That way agents can easily see the key parts and start exploring there first

- **Tweet:** https://x.com/NickADobos/status/2008050237320118628
- **Quoted:** https://x.com/Dimillian/status/2007864306952774107
- **What:** A brief observation about the value of distilling key codebase sections into reusable skills format, enabling AI agents to quickly understand architecture and prioritize exploration.

---


---


# Saturday, January 3, 2026

## @jessfraz - Jessie Frazelle's AGENTS.md Dotfiles Reference

> This is my .codex/AGENTS.md it's pretty ocd and pedantic but that should not be a shocker
>
> Tell me shit you do that you can't live without and I missed

- **Tweet:** https://x.com/jessfraz/status/2007682934585864619
- **What:** Jessie Frazelle shares her AGENTS.md configuration file from her dotfiles repository, seeking feedback on tools and workflows that others find essential for their development environments.

## @_kaitodev - Lovable for videos gaining traction
> lovable for videos gets better everyday with new creators joining
>
> check it out:
>
> *Quoting @sbsamuelbitenco:* we found a better way to do daniel dalen style captions

- **Tweet:** https://x.com/_kaitodev/status/2007553892968706134
- **Link:** https://odysser.com/
- **Quoted:** https://x.com/sbsamuelbitenco/status/2007549416450978065
- **What:** Lovable's video capabilities expanding with new creators. References improved caption generation approach.

---


## @nummanali - CC Mirror release announcement
> Announcing the release of CC Mirror
>
> The best way to use @Zai_org (GLM 4.7) and @MiniMax__AI (M2.1) Coding Plans
>
> - Full Model Support
> - All tools preconfigured
> - Custom themes
> - Isolated from CC
> - Enhanced prompts
>
> Start now: npx cc-mirror

- **Tweet:** https://x.com/nummanali/status/2007586417094844517
- **What:** CC Mirror tool launch enabling usage of GLM 4.7 and MiniMax M2.1 models with preconfigured tooling and custom themes.

---


---


## @6asscat - Context-dependent story credibility challenge
> this is the funniest shit to ever happen but u really can't talk about it unless u got the video on standby cuz everyone's gonna think u went off the fuckin deep end
>
> *Quoting @FurkanGozukara:* One year ago today, Zionist tunnels were discovered under synagogues in NYC. Stained mattresses and baby high chairs were found inside. A year later, no real conclusions, this seems to be slipping into the memory hole of time. https://t.co/h1AE6uxEpX

- **Tweet:** https://x.com/6asscat/status/2007410346253066572
- **Quoted:** https://x.com/FurkanGozukara/status/2007096285682356439
- **What:** Commentary on the challenge of sharing controversial stories without supporting evidence. Humorous take on credibility requirements for unbelievable claims.

---

---


## @0xDesigner - Formula for effective Claude Code usage
> the formula for getting the most out of claude code:
>
> "i want [goal/outcome]" + "interview me thoroughly to extract ideas and intent" + ultrathink + (plan mode on)
>
> thank me later

- **Tweet:** https://x.com/0xDesigner/status/2007467970952335533
- **What:** Best practices for Claude Code. Combining clear goal setting, detailed extraction of user intent, extended thinking, and plan mode for optimal results.

---

---


## @threepointone - Where good ideas come from for coding agents
> new post: where good ideas come from (for coding agents) https://t.co/CwE393F8rz
>
> thought about why some people cook with coding agents, and others bounce off. my take: llms are "thought completers" traversing idea-space - so good results come from good navigation: constraints, context, oracles, loops. I used steven johnson's "where good ideas come" from as a rubric and mapped it onto coding agents. also a note about how "juniors" can adapt to this new feature, and what "creating software" looks like practically.

- **Tweet:** https://x.com/threepointone/status/2007497491294396565
- **Link:** https://sunilpai.dev/posts/seven-ways/
- **What:** Deep dive on LLM effectiveness as thought completers. Maps Steven Johnson's idea frameworks to coding agent workflows, covering constraints, context, iteration patterns, and practical implications for developers adapting to AI-assisted development.

---

---


## @deedydas - Heart disease prevention through statins and LDL management
> Heart disease is the #1 cause of death in modern nations, more than cancer. It took the lives of 3 people I know just this year.
>
> This beautiful easy-to-read article called "Cardiovascular Disease is a Solved Problem" cites copious medical research to argue that:
>
> – heart disease and stroke, caused by plaque buildup in your arteries (atherosclerosis), arises from lifetime exposure to LDL cholesterol, particularly apoB, which is largely genetic.
>
> – Preventatively taking statins (rosuvastatin) for $15/mo can reduce LDL levels by 50%+ with no major side effects and reduce lifetime plaque buildup, even as early as your 20s!
>
> You should consult your doctor before taking medications, but it's always worth thinking about heart disease early.

- **Tweet:** https://x.com/deedydas/status/2007511612824178894
- **What:** Health awareness on cardiovascular disease prevention. Discusses evidence-based statin therapy for reducing LDL cholesterol and atherosclerotic plaque buildup, with emphasis on preventative treatment from early adulthood.

---

---


## @kr0der - Tips for Using Codex Effectively
> if you're also trying out Codex like me, here are some important tips that made Codex way better for me:
>
> 1. i always run codex —yolo or else it keeps stopping to ask for permissions. this feels fine as long as your prompt isn't bad.
>
> 2. start your setup from @steipete 's repo here - https://t.co/AYAlsng7d5 - i copied nearly all of it and obviously reworded parts that didn't relate to my work.
>
> 3. you have to use it differently than claude code so it'll take a couple of days to adjust. i found that if i give good instructions, it just one shots the task more reliably than CC. garbage in garbage out.
>
> 4. if you need a plan just write "make a plan" or use @thsottiaux 's skill here - https://t.co/ZFC1vhUVTk
>
> 5. codex is really good at long running tasks, especially when you give it a way to verify its outputs. the ralph-wiggum version for codex is typing "don't stop until …." and it'll listen.
>
> *Quoting @thsottiaux:* Simply adding "Ask questions if my request is underspecified" at the end of a prompt to Codex works well as you might expect, but also codified it a bit more in a `$ask-questions-if-underspecified` skill that I use regularly. https://t.co/QVPidaONx6

- **Tweet:** https://x.com/kr0der/status/2007538273745539187
- **Quoted:** https://x.com/thsottiaux/status/2006624682515247604
- **What:** Anthony shares practical tips for effectively using Codex AI, including workflow patterns like using --yolo mode, implementing verification methods for long-running tasks, and leveraging community skills for prompting improvements.

---


## @DidiTrading - Predicting Insider Activity on Polymarket
> Day 399: We spotted the Maduro attack before it happened.
>
> My brother @spacexbt, built a tool that tracks potential insider activity on Polymarket. Last night, the tracker flagged five separate alerts hours before the event happened.
> Based on that signal, he was able to buy at 7.5c, long before the market reacted.
>
> You don't need to predict the future, you need to track suspicious behavior. (Fresh wallets, unusual sizing, repeated entries in niche markets)
> e.g this insider turned $35k into $442k: https://t.co/h5fmtDZHPY
>
> Polymarket API keys are open to everyone. With today's AI coding tools, there's zero excuse not to build something similar yourself.
>
> *Quoting @spacexbt:* been working on a tool to get an edge on polymarket
> currently backtesting it and the results look promising
> managed to pull $11,000 today with some on and off trades
>
> while building, one thing became clear to me:
> the next bear market will probably be boring for most,
> but prediction markets won't die
>
> money opportunities don't disappear, they just move..
> even if memecoins and airdrops slow down,
> there'll always be a market for something, in that case polymarket
>
> still got more features to add and fine tuning to do
> once i'm happy with how it performs,
> i'll probably invite a few people to test it with me
>
> what i really respect about @Polymarket
> is how open their system is
> they literally hand you the API and say "go build"
> they give everyone, coder or not
> a chance to find their own way to make money
>
> will keep you all updated once the tool's ready

- **Tweet:** https://x.com/DidiTrading/status/2007559456662634966
- **Quoted:** https://x.com/spacexbt/status/1979256857878257776
- **What:** Didi describes a tool that detects insider trading activity on Polymarket by analyzing behavioral patterns like fresh wallets and unusual trade sizing, enabling profitable trades before market reactions. Demonstrates the potential of leveraging open APIs with AI coding tools.

---


## @doodlestein - Complete Workflow for AI-Assisted Software Development
> If you have a markdown plan for a new piece of software that you're getting ready to start implementing with a coding agent such as Claude Code, before starting the actual implementation work, give this a try.
>
> Paste your entire markdown plan into the ChatGPT 5.2 Pro web app with extended reasoning enabled and use this prompt; when it's done, paste the complete output from GPT Pro into Claude Code or Codex and tell it to revise the existing plan file in-place using the feedback:
>
> ---
> Carefully review this entire plan for me and come up with your best revisions in terms of better architecture, new features, changed features, etc. to make it better, more robust/reliable, more performant, more compelling/useful, etc.
>
> For each proposed change, give me your detailed analysis and rationale/justification for why it would make the project better along with the git-diff style changes relative to the original markdown plan shown below:
>
> <PASTE YOUR EXISTING COMPLETE PLAN HERE>
> ---
>
> This has never failed to improve a plan significantly for me. The best part is that you can start a fresh conversation in ChatGPT and do it all again once Claude Code or Codex finishes integrating your last batch of suggested revisions.
>
> After four or five rounds of this, you tend to reach a steady-state where the suggestions become very incremental.
>
> (Note: I was originally planning to end this post here, but thought it would be helpful for people to see this part in the larger context of the entire workflow I recommend using all my tooling)
>
> Then you're ready to turn the plan into beads (think of these as epics/tasks/subtasks and associated dependency structure. The name comes from Steve Yegge's amazing project, which is like Jira or Linear, but optimized for use by coding agents), which I do with this prompt using Claude Code with Opus 4.5:
>
> ---
> OK so please take ALL of that and elaborate on it more and then create a comprehensive and granular set of beads for all this with tasks, subtasks, and dependency structure overlaid, with detailed comments so that the whole thing is totally self-contained and self-documenting (including relevant background, reasoning/justification, considerations, etc.-- anything we'd want our \"future self\" to know about the goals and intentions and thought process and how it serves the over-arching goals of the project.)  Use only the `bd` tool to create and modify the beads and add the dependencies. Use ultrathink.
> ---
>
> After it finished all of that, I then do a round of this prompt (if CC did a compaction at any point, be sure to tell it to re-read your AGENTS dot md file):
>
> ---
> Check over each bead super carefully-- are you sure it makes sense? Is it optimal? Could we change anything to make the system work better for users? If so, revise the beads. It's a lot easier and faster to operate in \"plan space\" before we start implementing these things!  Use ultrathink.
> ---
>
> Then you're ready to start implementing. The fastest way to do that is to start up a big swarm of agents that coordinate using my MCP Agent Mail project.
>
> Then you can simply create a bunch of sessions using Claude Code, Codex, and Gemini-CLI in different windows or panes in tmux (or use my ntm project which tries to abstract and automate some of this) in your project folder at once and give them the following as their marching orders (for this to work well, you need to make sure that your AGENTS dot md file has the right blurbs to explain each of the tools; I'll include a complete example of this in a reply to this post):
>
> ---
> First read ALL of the AGENTS dot md file and README dot md file super carefully and understand ALL of both! Then use your code investigation agent mode to fully understand the code, and technical architecture and purpose of the project. Then register with MCP Agent Mail and introduce yourself to the other agents.
>
> Be sure to check your agent mail and to promptly respond if needed to any messages; then proceed meticulously with your next assigned beads, working on the tasks systematically and meticulously and tracking your progress via beads and agent mail messages.
>
> Don't get stuck in \"communication purgatory\" where nothing is getting done; be proactive about starting tasks that need to be done, but inform your fellow agents via messages when you do so and mark beads appropriately.
>
> When you're not sure what to do next, use the bv tool mentioned in AGENTS dot md to prioritize the best beads to work on next; pick the next one that you can usefully work on and get started. Make sure to acknowledge all communication requests from other agents and that you are aware of all active agents and their names.  Use ultrathink.
> ---
>
> If you've done a good job creating your beads, the agents will be able to get a decent sized chunk of work done in that first pass. Then, before they start moving to the next bead, I have them review all their work with this:
>
> ---
> Great, now I want you to carefully read over all of the new code you just wrote and other existing code you just modified with \"fresh eyes\" looking super carefully for any obvious bugs, errors, problems, issues, confusion, etc. Carefully fix anything you uncover. Use ultrathink.
> ---
>
> I keep running rounds of that until they stop finding bugs. Eventually they'll need to do a compaction, so if they do that, right after hit them with this (note that I've been typing AGENTS dot md to avoid the annoying preview on X because it thinks it's a website; you can replace that with a period and remove the spaces if you want; the agents don't care either way):
>
> ---
> Reread AGENTS dot md so it's still fresh in your mind.   Use ultrathink.
> ---
>
> When the reviews come up clean, have them move on to the next bead:
>
> ---
> Reread AGENTS dot md so it's still fresh in your mind.   Use ultrathink.   Use bv with the robot flags (see AGENTS dot md for info on this) to find the most impactful bead(s) to work on next and then start on it. Remember to mark the beads appropriately and communicate with your fellow agents. Pick the next bead you can actually do usefully now and start coding on it immediately; communicate what you're working on to your fellow agents and mark beads appropriately as you work. And respond to any agent mail messages you've received.
> ---
>
> When all your beads are completed, you might want to run one of these prompts:
>
> ---
> Do we have full unit test coverage without using mocks/fake stuff? What about complete e2e integration test scripts with great, detailed logging? If not, then create a comprehensive and granular set of beads for all this with tasks, subtasks, and dependency structure overlaid with detailed comments.
> ---
>
> or
>
> ---
> Great, now I want you to super carefully scrutinize every aspect of the application workflow and implementation and look for things that just seem sub-optimal or even wrong/mistaken to you, things that could very obviously be improved from a user-friendliness and intuitiveness standpoint, places where our UI/UX could be improved and polished to be slicker, more visually appealing, and more premium feeling and just ultra high quality, like Stripe-level apps.
> ---
>
> or
>
> ---
> I still think there are strong opportunities to enhance the UI/UX look and feel and to make everything work better and be more intuitive, user-friendly, visually appealing, polished, slick, and world class in terms of following UI/UX best practices like those used by Stripe, don't you agree? And I want you to carefully consider desktop UI/UX and mobile UI/UX separately while doing this and hyper-optimize for both separately to play to the specifics of each modality. I'm looking for true world-class visual appeal, polish, slickness, etc. that makes people gasp at how stunning and perfect it is in every way.  Use ultrathink.
> ---
>
> And then start the process again of implementing the beads. When you're done with all that and have solid test coverage, you can then keep doing rounds of these two prompts until they consistently come back clean with no changes made:
>
> ---
> I want you to sort of randomly explore the code files in this project, choosing code files to deeply investigate and understand and trace their functionality and execution flows through the related code files which they import or which they are imported by.
>
> Once you understand the purpose of the code in the larger context of the workflows, I want you to do a super careful, methodical, and critical check with \"fresh eyes\" to find any obvious bugs, problems, errors, issues, silly mistakes, etc. and then systematically and meticulously and intelligently correct them.
>
> Be sure to comply with ALL rules in AGENTS dot md and ensure that any code you write or revise conforms to the best practice guides referenced in the AGENTS dot md file. Use ultrathink.
> ---
>
> and
>
> ---
> Ok can you now turn your attention to reviewing the code written by your fellow agents and checking for any issues, bugs, errors, problems, inefficiencies, security problems, reliability issues, etc. and carefully diagnose their underlying root causes using first-principle analysis and then fix or revise them if necessary? Don't restrict yourself to the latest commits, cast a wider net and go super deep! Use ultrathink.
> ---
>
> You should also periodically have one of the agents run this as you're going to commit your work:
>
> ---
> Now, based on your knowledge of the project, commit all changed files now in a series of logically connected groupings with super detailed commit messages for each and then push. Take your time to do it right. Don't edit the code at all. Don't commit obviously ephemeral files. Use ultrathink.
> ---
>
> If you simply use these tools, workflows, and prompts in the way I just described, you can create really incredible software in a just a couple days, sometimes in just one day.
>
> I've done it a bunch of times now in the past few weeks and it really does work, as crazy as that may sound. You see my GitHub profile for the proof of this. It looks like the output from a team of 100+ developers.
>
> The frontier models and coding agent harnesses really are that good already, they just need this extra level of tooling and prompting and workflows to reach their full potential.
>
> To learn more about my system (which is absolutely free and 100% open-source), check out:
>
> https://t.co/22Fy2w73x0
>
> It include a complete tutorial that shows anyone how to get start with this process. You don't even need to know much at all about computers; you just need the desire to learn and some grit and determination. And about $500/month for the Claude Max and GPT Pro subscriptions, plus another $50 or so for the cloud server.
>
> If you want to change the entire direction of your life, it has truly never been easier. If you think you might want to do it, I really recommend just immersing yourself.
>
> Once you get Claude Code up and running on the cloud server, you basically have an ultra competent friend who can help you with any other problems you encounter.
>
> And I will personally answer your questions or problems if you reach out to me on X or on GitHub issues (it might be Claude impersonating me though, lol).

- **Tweet:** https://x.com/doodlestein/status/2007588870662107197
- **Link:** https://agent-flywheel.com/
- **What:** Jeffrey Emanuel presents a comprehensive multi-stage workflow for AI-assisted software development, combining ChatGPT Pro for planning, Claude Code for implementation with task management via beads, and coordinated multi-agent systems for scaling complex projects.

---


## @irl_danB - OpenProse: A Programming Language for AI Sessions
> "Wow."
>
> the OpenProse VM is a new kind of computer
>
> try it in 30 seconds:
>
> https://t.co/uCWV6A3ocm
>
> install skill (no code, no dependencies) in Claude Code, Opencode, Amp, Codex
>
> restart to load skill
>
> `openprose boot`
>
> onboarding is built in, it should hold your hand from there https://t.co/0fnWcGuEp9
>
> *Quoting @xpasky:* @irl_danB I tried it with the skill installed.
>
> It executed the VM perfectly. Wow.

- **Tweet:** https://x.com/irl_danB/status/2007595082229395519
- **Link:** https://www.prose.md/
- **Quoted:** https://x.com/xpasky/status/2007592282409623887
- **What:** Dan introduces OpenProse, a new programming language designed for AI sessions that enables agent orchestration and complex workflows without code or dependencies, installable as a skill across multiple coding harnesses.

---


## @irl_danB - OpenProse as a VM for Agent Orchestration
> https://t.co/uCWV6A3ocm turns your harness into a VM that can do arbitrarily complex agent orchestration
>
> it's just a prompt. no frameworks, no code, no dependencies, nothing https://t.co/FeTm0UTAz2
>
> *Quoting @nickcammarata:* i think there's probably a $100b prompt waiting out there that puts the models 0.5 generations ahead

- **Tweet:** https://x.com/irl_danB/status/2007618496092618872
- **Link:** https://www.prose.md/
- **Quoted:** https://x.com/nickcammarata/status/2006400435167563962
- **What:** Dan emphasizes OpenProse's capabilities as a paradigm shift for agent orchestration within coding harnesses, describing it as a prompt-based system with no framework or dependency overhead.

---


## @GeoffreyHuntley - Learn fundamentals for software engineering
> @seflless @Vjeux learn the fundamentals

> *Replying to @seflless:* @Vjeux Cc @GeoffreyHuntley, what's your recommendation? You mentioned Anthropic's Ralph skill is just broken recently

- **Tweet:** https://x.com/GeoffreyHuntley/status/2007629738219897146
- **Link:** https://ghuntley.com/ralph/
- **Parent:** https://x.com/seflless/status/2007629603205226759
- **What:** Advice to learn fundamentals, responding to a conversation about software engineering tools. Links to an article about Ralph Wiggum as a "software engineer" - a commentary on AI agent capabilities and their limitations.

---

DATE: Saturday, January 3, 2026

---

## @vasuman - Starting a high-signal agents and vibe coding group chat
> Trying something new: starting a group chat dedicated to agents (and to a lesser extent, vibe coding).

To get in, you must be qualified, must have built/shipped something real with quality (tell me what that is in the comments).

Absolutely 0 exceptions. Need this group chat to be high signal and low noise, for the sake of everyone in it. Otherwise it dies in 2 days.

Good indicator: I built a memory layer for agents, here's the GitHub link.

Bad indicator: I vibe coded this thing that took 5 seconds and no one including myself finds any value in it.

Please comment with a few words if you are interested.

- **Tweet:** https://x.com/vasuman/status/2007642606684061718
- **What:** Initiative to create a high-quality discussion group for agents and "vibe coding" with strict membership requirements to maintain signal-to-noise ratio.

---

DATE: Saturday, January 3, 2026

---

## @GrantSlatton - Looking for quality 100% cotton t-shirt brands
> i'm in the market to replace all my plain white t-shirts

both v-neck and crew neck

does anyone have a 100% cotton t-shirt brand they LOVE both the feel and fit of?

- **Tweet:** https://x.com/GrantSlatton/status/2007654971425337456
- **What:** Personal shopping request for high-quality cotton t-shirts in multiple neckline styles.

---

DATE: Saturday, January 3, 2026

---

## @PaulSolt - macOS agents worth exploring
> Steal concepts from @steipete on his Agents .md file for Codex.

Peekaboo (macOS agent vision): https://t.co/VUVbl4D3HP

The Oracle: https://t.co/sx6ADh4nhJ

RepoBar (macOS Menubar): https://t.co/3KrHijbYqh

> *Quoting @steipete:* @hammaadjam I'd cut it down drastically, there's a lot of unneeded crap in there.

- **Tweet:** https://x.com/PaulSolt/status/2007679397567050058
- **Link:** https://github.com/steipete/Peekaboo/blob/main/AGENTS.md
- **Quoted:** https://x.com/steipete/status/2007524664851996947
- **What:** Recommendation to explore Peter Steinberger's macOS agent tools (Peekaboo for screenshots, Oracle for AI assistance, and RepoBar for GitHub monitoring) with agent documentation. Highlights three sophisticated automation tools for developers.

---

DATE: Saturday, January 3, 2026

---

## @carolccs1111 - Reply with image
> @rebatheonryo @6asscat https://t.co/fvK5snKIEZ

> *Replying to @rebatheonryo:* @6asscat that nigga was hearing yiddish in his walls

- **Tweet:** https://x.com/carolccs1111/status/2007705529033146674
- **Parent:** https://x.com/rebatheonryo/status/2007684616455631217
- **What:** Image reply in a conversation thread.

---


---


# Friday, January 2, 2026

## @alexhillman - Git safety hooks for destructive command prevention
> been here, this never feels good.
>
> this lil set of hooks lets me rest easy it won't happen again
>
> *Quoting @nummanali:* Lmao I accidentally deleted everything I worked on today. Now I'm tasking codex to reconstruct it using cass (coding_agent_session_search). Probably going to take all night, lets see what happens

- **Tweet:** https://x.com/alexhillman/status/2006881325849129246
- **Link:** https://github.com/Dicklesworthstone/misc_coding_agent_tips_and_scripts/blob/main/DESTRUCTIVE_GIT_COMMAND_CLAUDE_HOOKS_SETUP.md
- **Quoted:** https://x.com/nummanali/status/2006875686846476556
- **What:** Git hooks setup to prevent accidental deletion of work. Responding to a cautionary tale about losing a day's work.

---


## @parcadei - Continuous Claude v2 Context Management
> @yuzu_4ever https://t.co/PwioZUVYkD
>
> you need this

- **Tweet:** https://x.com/parcadei/status/2005755875701776624
- **Link:** https://github.com/parcadei/Continuous-Claude-v2
- **What:** Python framework for maintaining session continuity in Claude Code workflows. Features ledger-based state persistence, handoff system for session resumption, MCP execution without context pollution, and agent orchestration with isolated context windows. Includes TypeScript execution hooks, Braintrust session tracing, artifact indexing, and compound learning tracking.

---


## @marckohlbrugge - Sessy: Open-Source Email Observability for AWS SES
> Introducing… 💌Sessy
>
> Open-source email observability for AWS SES
>
> https://t.co/PrBWVNwzVM
>
> Stop paying $$$ for VC-backed SES wrappers just to get a decent UI. Host your own.
>
> 💎 Built on Ruby on Rails
> 🧑‍💻 Licensed under O'Saasy
> 💡 Inspired by @37signals' Fizzy

- **Tweet:** https://x.com/marckohlbrugge/status/2005972157445333371
- **Link:** https://github.com/marckohlbrugge/sessy
- **What:** Self-hosted Rails application providing email observability for Amazon SES. Shows email events in a timeline: deliveries, bounces, complaints, opens, clicks. Open-source alternative to expensive SES wrapper services, allowing raw SES usage with beautiful UI for monitoring.

---


## @ShadcnStudio - Shadcn Studio Calendar Components
> Product link:- https://t.co/hg8PRG7V0I
>
> Github link:- https://t.co/Sk1cQx5LJ8
>
> Check it out 👆🏻

- **Tweet:** https://x.com/ShadcnStudio/status/2005964727806222598
- **Links:** [Product](https://shadcnstudio.com/docs/components/calendar), [GitHub](https://github.com/themeselection/shadcn-studio)
- **What:** Collection of 25+ shadcn/ui calendar component variants for React with TailwindCSS. Features single/range picking, multi-month navigation, time slots, and presets. Part of broader shadcn-studio ecosystem with 952 GitHub stars offering customizable components, blocks, templates, and theme generator.

---


## @joodalooped - Markwhen: Keyboard-First Timeline Tool
> for those who prefer keyboard to drag and drop, https://t.co/wLt0wiAOM1 is quite nice too

- **Tweet:** https://x.com/joodalooped/status/2006089396861427738
- **Link:** https://markwhen.com/
- **Quoted:** Karel Vuong's Lifemap tool for annual reviews and life planning
- **What:** Keyboard-driven timeline creation tool for planning and visualization. Text-based input alternative to drag-and-drop interfaces, complementary to Lifemap for personal planning and retrospectives.

---


## @pk_iv - Reverse Engineering Claude Chrome for Remote Browsers
> I spent all of Christmas reverse engineering Claude Chrome so it would work with remote browsers.
>
> Here's how Anthropic taught Claude how to browse the web (1/7)

- **Tweet:** https://x.com/pk_iv/status/2005694082627297735
- **Media:** Video demonstration
- **What:** Technical thread documenting how Anthropic's Claude Chrome extension works internally, with focus on enabling remote browser integration. Paul Klein IV reverse-engineered the extension over the Christmas holidays to enable remote browser functionality.

---


## @simonw - GistHost: Improved GitHub Gist HTML Preview
> I forked the wonderful https://t.co/DdVAXh3Du3 to create https://t.co/4jatEKRMZv - here's what I changed in my fork: https://t.co/DmSbkKMNTn

- **Tweet:** https://x.com/simonw/status/2006851664935006385
- **Links:** [GistPreview](https://gistpreview.github.io/), [GistHost](https://gisthost.github.io/), [Blog Post](https://simonwillison.net/2026/Jan/1/gisthost/)
- **What:** Simon Willison forked the 10-year-old GistPreview project to create GistHost, modernizing the tool that lets you view GitHub Gists as rendered HTML pages. His fork fixes handling of truncated large files by fetching from the raw URL when needed, and updates the UI with modern CSS instead of Bootstrap.

---


## @DataChaz - Gemini Interactive Diagram Learning Tool
> Holy sh*t.
>
> Gemini can now produce fully interactive images on any topic.
>
> Such an insane resource for learning → highlight any region, and it gives you a full explanation 🤯

- **Tweet:** https://x.com/DataChaz/status/2005605994781606141
- **What:** Google Gemini now generates fully interactive diagrams where users can highlight any region to receive detailed explanations. A powerful visual learning tool that combines generation with interactive exploration of complex topics.

---


## @steipete - Summarize.sh Hover Toolbar for Link Previews
> https://t.co/qSe6Y6Qfup now shows a summarized toolbar over any link you hover, perfect to identify clickbait before even opening the link.

- **Tweet:** https://x.com/steipete/status/2006425901719023628
- **Link:** https://summarize.sh/
- **What:** Summarize.sh CLI and Chrome extension now includes a hover toolbar feature that shows AI-generated summaries when hovering over links, helping users avoid clickbait. The tool supports local models, paid providers, and free OpenRouter models for fast content summarization.

---


## @DanielNealAdler - AI Job Displacement Reality Check
> I really enjoyed this. There's no sense pretending that this isn't happening, even for those of us selling AI. I don't believe AI is bad, but we do have to reconcile with this reality; it's only a matter of time until this is us tech workers, too

- **Tweet:** https://x.com/DanielNealAdler/status/2006206247054229798
- **Link:** https://www.nytimes.com/2025/12/28/opinion/artificial-intelligence-jobs.html (paywalled)
- **What:** Commentary on a NYT opinion piece about AI's impact on employment. Dan Adler acknowledges the uncomfortable reality that AI displacement will eventually affect tech workers themselves, despite many currently building AI solutions.

---


## @tom_doerr - Whisper-Flow Real-Time Audio Transcription
> Transcribes audio streams in real-time
>
> https://t.co/1hcfk9l51V

- **Tweet:** https://x.com/tom_doerr/status/2006262985182834881
- **Link:** https://github.com/dimastatz/whisper-flow/
- **What:** Python framework enabling real-time transcription of streaming audio using OpenAI's Whisper model. Unlike batch processing, Whisper-Flow accepts continuous audio chunks and produces incremental transcripts immediately using tumbling window segmentation. 463 GitHub stars.

---


## @donvito - GLM 4.7 Beast Performance
> omg GLM 4.7 is a beast!!!

$3/mo is a steal

- **Tweet:** https://x.com/donvito/status/2006743894147711370
- **Link:** https://z.ai/subscribe?cc=fission_glmcode_sub_v1&ic=V8VOHXNASO&n=Melvin%20Vivas
- **What:** Enthusiastic endorsement of the GLM 4.7 coding model, highlighting exceptional value at $3/month. Follow-up to earlier testing, emphasizing the model's capabilities and competitive pricing.


---

## @donvito - GLM 4.7 First Impressions
> wow GLM 4.7 is great

tried it in claude code

- **Tweet:** https://x.com/donvito/status/2006738817773171175
- **Link:** https://z.ai/subscribe?cc=fission_glmcode_sub_v1&ic=V8VOHXNASO&n=Melvin%20Vivas
- **What:** Positive first impression of GLM 4.7 model when used in Claude Code environment, part of the GLM Coding Plan offering AI-powered code generation for agents and IDEs at affordable pricing.


---

## @emmagine79 - Quick Smaug Implementation Success
> @alexhillman ayyyy thanks for this fam! i was able to use Claude opus + anti gravity to put this together in like 2 hours

- **Tweet:** https://x.com/emmagine79/status/2007051496496714038
- **Media:** Video demonstration
- **What:** Community response to Smaug (Alex's Twitter bookmarks organizer), showing rapid implementation success using Claude Opus - built a similar system in just 2 hours, demonstrating the accessibility and power of AI-assisted development.


---

## @OsaurusAI - Osaurus Mac AI Agent Demo
> Powered by Osaurus MCP tools.
Claude sees your screen, clicks, types, navigates — you supervise.
This is what AI agents look like on Mac.

- **Tweet:** https://x.com/OsaurusAI/status/2007091913393070168
- **Link:** https://github.com/dinoki-ai/osaurus
- **What:** Native macOS LLM server with MCP support enabling Claude to interact directly with the Mac interface - screen reading, clicking, typing, navigation. Runs local or cloud models with OpenAI/Anthropic compatible APIs. Built in Swift for Apple Silicon.


---

## @jarrodwatts - Claude HUD Plugin Concept
> Started working on "Claude HUD"

A Claude Code plugin that visualizes:
· context remaining in the session
· what tools are executing
· which subagents are running
· claude's to-do list progress

If there's enough interest, I'll polish it up and open-source it!

- **Tweet:** https://x.com/jarrodwatts/status/2007035752665034994
- **Media:** Video demonstration
- **What:** Work-in-progress Claude Code plugin providing real-time visualization dashboard for session metrics: context remaining, active tools, subagent status, and todo progress. Potential open-source release based on community interest.


---

## @simonw - GistHost Fork of GistPreview

> I forked the wonderful https://gistpreview.github.io/ to create https://gisthost.github.io/ - here's what I changed in my fork: https://simonwillison.net/2026/Jan/1/gisthost/

- **Tweet:** https://x.com/simonw/status/2006851664935006385
- **Links:** [GistPreview](https://gistpreview.github.io/), [GistHost](https://gisthost.github.io/)
- **Filed:** [GistHost Fork](./knowledge/articles/gisthost-fork.md)
- **What:** Simon Willison forked GistPreview to create GistHost, a tool for rendering GitHub Gists as standalone web pages. The linked article documents his changes and motivations for the fork.

---


## @DataChaz - Gemini Interactive Images for Learning

> Holy sh*t.
>
> Gemini can now produce fully interactive images on any topic.
>
> Such an insane resource for learning → highlight any region, and it gives you a full explanation 🤯

- **Tweet:** https://x.com/DataChaz/status/2005605994781606141
- **Media:** Video demonstration
- **What:** Google Gemini's new capability to generate interactive images where users can highlight any region to get detailed explanations. Positioned as a powerful learning tool.

---


## @steipete - Summarize.sh Link Preview Toolbar

> https://summarize.sh/ now shows a summarized toolbar over any link you hover, perfect to identify clickbait before even opening the link.

- **Tweet:** https://x.com/steipete/status/2006425901719023628
- **Link:** https://summarize.sh/
- **Filed:** [Summarize.sh](./knowledge/tools/summarize-sh.md)
- **What:** A browser tool that displays summary information in a toolbar when hovering over links, helping users identify clickbait without clicking through.

---


## @pk_iv - Claude Chrome Browser Integration

> I spent all of Christmas reverse engineering Claude Chrome so it would work with remote browsers.
>
> Here's how Anthropic taught Claude how to browse the web (1/7)

- **Tweet:** https://x.com/pk_iv/status/2005694082627297735
- **What:** A thread documenting how Anthropic's Claude Chrome extension works under the hood, with focus on remote browser integration. Paul Klein spent time reverse-engineering the extension over the holidays.

---


## @joodalooped - Markwhen Keyboard-Driven Timeline Tool

> for those who prefer keyboard to drag and drop, https://markwhen.com/ is quite nice too
>
> *Quoting @karelvuong:* Introducing Lifemap, a new tool to add to your personal annual reviews and 2026 planning. Lifemap lets you conduct a retrospective of your life and develop a roadmap ahead. Every year, my wife and I look forward to the lull during the holidays to work on the biggest project of our lives—ourselves.

- **Tweet:** https://x.com/joodalooped/status/2006089396861427738
- **Quoted:** https://x.com/karelvuong/status/2005669812199137476
- **Link:** https://markwhen.com/
- **Filed:** [Markwhen](./knowledge/tools/markwhen.md)
- **What:** A keyboard-first timeline tool for planning and visualization. Complementary to Lifemap (the quoted tool), offering text-based input for those who prefer keyboards over drag-and-drop interfaces.

---


## @ShadcnStudio - Shadcn Calendar UI Components

> 🗂️ Shadcn Calendar!
>
> Plan, book, and schedule effortlessly with 25 calendar variants built for real-world use cases.

- **Tweet:** https://x.com/ShadcnStudio/status/2005964727806222598
- **Link:** https://github.com/themeselection/shadcn-studio
- **Filed:** [Shadcn Studio](./knowledge/tools/shadcn-studio.md)
- **What:** An extended collection of 25+ shadcn/ui calendar components with variants for single/range picking, multi-month navigation, and time slots. Part of the broader shadcn-studio ecosystem offering customizable UI components and templates.

---


## @marckohlbrugge - Sessy Open-Source SES Email Observability

> Introducing… 💌Sessy
>
> Open-source email observability for AWS SES
>
> Stop paying $$$ for VC-backed SES wrappers just to get a decent UI. Host your own.
>
> 💎 Built on Ruby on Rails
> 🧑‍💻 Licensed under O'Saasy
> 💡 Inspired by @37signals' Fizzy

- **Tweet:** https://x.com/marckohlbrugge/status/2005972157445333371
- **Link:** https://github.com/marckohlbrugge/sessy
- **Filed:** [Sessy](./knowledge/tools/sessy.md)
- **What:** A self-hosted Rails application providing beautiful observability and monitoring for Amazon SES, eliminating the need for expensive commercial SES wrappers. Shows events in a timeline: sends, deliveries, clicks, bounces, etc.

---


## @0xUrvish - uselayouts: Animated React Components Library

> *Replying to @0xUrvish:* Hi developers
I just launched my animated UI components library
>
> 100% open source and free to use
it's live now do check it out and would appreciate your feedback https://t.co/DOUxe8w4oy
>
> Try it out: https://t.co/73RgRfaHwk

- **Tweet:** https://x.com/0xUrvish/status/2006608646730559629
- **Parent:** https://x.com/0xUrvish/status/2006600544220230083
- **Link:** https://uselayouts.com/
- **Filed:** [uselayouts](./knowledge/tools/uselayouts.md)
- **What:** Open-source library of premium animated React components built with Framer Motion and Tailwind CSS. Includes modern micro-interactions and ready-to-use motion components.

---


## @Suupercharged - Static Navbars Can Be Cool Too

> Static navbars can be cool too 👀 https://t.co/CkRIvlXUrr

- **Tweet:** https://x.com/Suupercharged/status/2006787096955203911
- **Media:** Video demonstration
- **What:** Short video showcasing static navbar design approaches. Flagged for transcript capture.

---


## @bentossell - Article Share

> https://t.co/Ref8GgkIR5

- **Tweet:** https://x.com/bentossell/status/2006352820140749073
- **Link:** https://x.com/i/article/2006346812785868800
- **What:** Shared article link (content not yet extracted). Bookmark captures the reference for later review.

---


## @GithubProjects - Stop Guessing Why a Process is Running

> Stop guessing why a process is running on your system. https://t.co/F4edRFxOuH

- **Tweet:** https://x.com/GithubProjects/status/2006747292510925092
- **Media:** Image with tool/tip
- **What:** Shared resource or tool for process investigation and system debugging. Flagged for media capture.

---


## @adamkillam - Content Operating System Vision

> *Replying to @alexhillman:* Feed them to the content operating system I'm building, sort them, save them, and from there create all manner of content from the insights in each post. Ideally automatically.
>
> Also want to track trends, have ideas automatically researched and saved.
>
> The list goes on.

- **Tweet:** https://x.com/adamkillam/status/2006894238446002261
- **Parent:** https://x.com/alexhillman/status/2006881998456164772
- **What:** Adam shares his vision for a content operating system that aggregates, sorts, and automatically generates content insights from bookmarked posts while tracking trends.

---


## @jarrodwatts - Claude HUD Plugin

> Started working on "Claude HUD"
>
> A Claude Code plugin that visualizes:
> · context remaining in the session
> · what tools are executing
> · which subagents are running
> · claude's to-do list progress
>
> If there's enough interest, I'll polish it up and open-source it!

- **Tweet:** https://x.com/jarrodwatts/status/2007035752665034994
- **What:** A Claude Code plugin that provides real-time visualization of session context, tool execution, subagent activity, and task progress. Currently a work-in-progress with plans to open-source if there's community interest.

---


## @OsaurusAI - Osaurus: macOS LLM Server with AI Agent Capabilities

> Powered by Osaurus MCP tools.
> Claude sees your screen, clicks, types, navigates — you supervise.
> This is what AI agents look like on Mac.

- **Tweet:** https://x.com/OsaurusAI/status/2007091913393070168
- **Link:** https://github.com/dinoki-ai/osaurus
- **Filed:** [osaurus.md](./knowledge/tools/osaurus.md)
- **What:** A native macOS LLM server with MCP support that enables AI agents like Claude to interact with the screen, navigate applications, and perform tasks while you supervise. Supports local and cloud models with OpenAI and Anthropic compatible APIs.

---


## @emmagine79 - Smaug Project Response

> *Replying to @alexhillman:* its late so i'll probably regret posting this but...
>
> enter the dragon 🔥🐲
>
> say hi to Smaug, the helpful hoarding dragon that roams your Twitter bookmarks and helps you organize them into your personal knowledge system of choice.
>
> ayyyy thanks for this fam! i was able to use Claude opus + anti gravity to put this together in like 2 hours

- **Tweet:** https://x.com/emmagine79/status/2007051496496714038
- **Parent:** https://x.com/alexhillman/status/2006968571268661423
- **What:** Community response to the Smaug project announcement, sharing success in using Claude Opus and related tools to build something in just 2 hours. Demonstrates practical application of Smaug for organizing bookmarks into a personal knowledge system.

---


## @donvito - GLM 4.7 Coding Model Assessment

> wow GLM 4.7 is great
>
> tried it in claude code

- **Tweet:** https://x.com/donvito/status/2006738817773171175
- **Link:** https://z.ai/subscribe?cc=fission_glmcode_sub_v1
- **Filed:** [glm-4-7-coding-plan.md](./knowledge/articles/glm-4-7-coding-plan.md)
- **What:** Positive endorsement of GLM 4.7 model when used in Claude Code environment. The linked plan offers affordable access ($3/month) to GLM models for coding tasks and agent-based development.

---


## @donvito - GLM 4.7 Pricing Enthusiasm

> omg GLM 4.7 is a beast!!!
>
> $3/mo is a steal

- **Tweet:** https://x.com/donvito/status/2006743894147711370
- **What:** Follow-up endorsement emphasizing the value proposition of GLM 4.7 at $3/month subscription rate. Reflects developer sentiment about the model's capabilities relative to pricing.

---


---


## @ankurnagpal - 2026 Backdoor Roth IRA Contribution Guide

> I just made my 2026 Backdoor Roth IRA contribution for $7,500
>
> Most high earners don't do this because they think it's a complicated strategy that isn't worth the effort
>
> But, you typically can do it in less than 5 minutes with 3 simple steps:

- **Tweet:** https://x.com/ankurnagpal/status/2007124597846753524
- **What:** Personal finance advice on executing a backdoor Roth IRA contribution for 2026. The author explains this tax strategy is simpler than most high earners believe and can be completed in under 5 minutes.

---


## @doodlestein - Claude Code UI/UX Enhancement Prompt

> Here is an incredibly useful prompt to use with Claude Code and Opus 4.5 to improve the UI/UX of your web application.
>
> I use this mostly for NextJS 16 apps with React 19, Tailwind 4, and other libraries like Framer Motion, but it's pretty generic and should work with anything.
>
> Something about the phrasing, and asking for agreement from the model, somehow motivates it to polish things up better. Also, instructing it to separately think through desktop vs mobile leads to much better outcomes.
>
> Note that this is really for when your site/app already works and looks decent and you want to improve it. I have a different prompt for when it looks bad and you need a complete overhaul.
>
> I generally do many, many passes of this, sometimes with more than one agent at once. Each time, it tries to make some incremental improvement, even if it's minor; but these really add up after 10 iterations!
>
> Here it is (I even made this a button on my Stream Deck gizmo because I use it so frequently):
>
> "I still think there are strong opportunities to enhance the UI/UX look and feel and to make everything work better and be more intuitive, user-friendly, visually appealing, polished, slick, and world class in terms of following UI/UX best practices like those used by Stripe, don't you agree? And I want you to carefully consider desktop UI/UX and mobile UI/UX separately while doing this and hyper-optimize for both separately to play to the specifics of each modality. I'm looking for true world-class visual appeal, polish, slickness, etc. that makes people gasp at how stunning and perfect it is in every way.  Use ultrathink."

- **Tweet:** https://x.com/doodlestein/status/2007194101448573036
- **What:** A detailed prompt engineering guide for iteratively improving web application UI/UX using Claude Code and Opus 4.5. The approach emphasizes separate desktop/mobile optimization and progressive refinement through multiple passes with extended thinking.

---


## @gmickel - RepoPrompt v1.5.61 Integration in Flow Plugin

> Also added support for @RepoPrompt's new prompt export (v1.5.61). Run a @ID_AA_Carmack-level review, export the full context to a file, paste into the LLM of your choosing.
>
> https://t.co/eOUY4GGmyD
> *Replying to @gmickel:* Nice tip for when you're just starting with a vague idea. Added this to my flow plugin as an optional step before the plan → work loop
>
> /flow:interview https://t.co/l7cgqY72rT (or beads id)
>
> 40+ deep questions about technical details, edge cases, testing, architecture. Writes refined spec back.
>
> h/t @trq212

- **Tweet:** https://x.com/gmickel/status/2007251220348682538
- **Link:** https://github.com/gmickel/gmickel-claude-marketplace
- **Parent:** https://x.com/gmickel/status/2007251218159067177
- **What:** Enhancement to Gordon Mickel's Flow plugin adding support for RepoPrompt v1.5.61's new prompt export capability, enabling high-quality code reviews that can be exported to external LLMs, complementing the existing plan→work loop with a deep interview phase.

---


## @alexhillman - Git command safety with hooks
> basically everything starts with this command https://t.co/yry008gaSI
>
> *Quoting @mattsalem:* @alexhillman What's your planning workflow look like?

- **Tweet:** https://x.com/alexhillman/status/2007292106046615977
- **Link:** https://gist.github.com/alexknowshtml/074cb4fd91c14b37f2b6e2b62f79b60e
- **Quoted:** https://x.com/mattsalem/status/2007291062143070355
- **What:** Git workflow optimization tool. Discusses a key command for managing planning workflow.

---

---


## @cremieuxrecueil - Pit Bull Aggression and Random Violence

> It's true that "dog biting" is usually not out of nowhere.

But pit bulls are the exception. Their defining characteristic is *random violence*.

This is why, for example, they frequently murder and cannibalize their littermates, their mothers, and their own puppies. https://t.co/VvxY3A4ZDj

- **Tweet:** https://x.com/cremieuxrecueil/status/2007233017153237488
- **What:** Discussion of pit bull behavioral characteristics and aggression patterns, contrasting with general dog behavior.

**Quoted context:** @oliveegger explained that dog biting behavior typically isn't random and relates to observable warning signs and threshold behaviors in dogs.

---

---



---


# Thursday, January 1, 2026

## @__morse - Playwriter MCP Browser Automation Extension
> https://t.co/cG7QBcAAE8
> *Replying to @__morse:* playwriter can do basically anything in the browser. I just used it in opencode to open Cloudflare dashboard and register a new domain, all while lying in my bed. it even clicked "I am not a robot" and paid
>
> https://t.co/cG7QBcAAE8

- **Tweet:** https://x.com/__morse/status/2006709180510372142
- **Parent:** https://x.com/__morse/status/2006709143051411818
- **What:** Playwriter is a browser automation MCP that works as a Chrome extension, providing full Playwright API capabilities with 90% less context window overhead than traditional Playwright MCPs.

---


## @Dimillian - State of Agentic iOS Engineering in 2026
> The State of Agentic iOS Engineering in 2026
>
> My perspective on AI-driven programming, workflows, and tooling
>
> https://t.co/a4xAAbK4vg
> *Replying to @Dimillian:* I wrote a big retrospective on my 2025 usage of AI tooling and workflows for iOS, but not only.
> I hope you'll find something for you; it's a bit of everything!
> Link below 👇🏻

- **Tweet:** https://x.com/Dimillian/status/2006773415181693125
- **Parent:** https://x.com/Dimillian/status/2006773412321169685
- **Link:** https://dimillian.medium.com/the-state-of-agentic-ios-engineering-in-2026-c5f0cbaa7b34?sk=fc0d73c63aec57085ff9fb90fd1de1c7
- **What:** A comprehensive retrospective and analysis of AI tooling and workflows for iOS development, covering agentic programming approaches and best practices from 2025 usage.

---


## @mattpocockuk - Ralph Opus 4.5 Workflow and Context Management
> I'm using Ralph for everything.
>
> I have some modifications to @GeoffreyHuntley's initial vision:
>
> - How to give Ralph enough context to succeed
> - AFK Ralph vs HOTL Ralph
> - Why PRD format matters
> - Why multi-phase plans are dead
>
> Video (or probably videos) coming soon
>
> *Quoting @mattpocockuk:* Ralph Wiggum + Opus 4.5 is really, really good

- **Tweet:** https://x.com/mattpocockuk/status/2006807098076881312
- **Quoted:** https://x.com/mattpocockuk/status/2006694097818395019
- **What:** An exploration of using Ralph (an AI-powered development workflow) with Claude Opus 4.5, discussing context management, operational modes, and improvements to the original vision including PRD formatting and planning approaches.

---


## @0xfdf - Beads: Task Management Graph for Agents

> this is beads: https://t.co/MBq3rQDd9M. you can sync it with any task management frontend you want; I integrate it with GitHub issues using `gh`, but you can use any.
>
> I recommend something like this in your AGENTS/CLAUDE . md file:
>
> ```
> ### Issue tracking
>
> Be conscientious about tracking your work with issues creating using beads (`bd`). Beads is a task management graph with which you can track projects, epics, issues, etc.
>
> ALL plans, tasks, todos, subtasks, etc should be faithfully recorded in beads in full technical detail, complete with
> dependencies and order of completion. You MUST record ALL your work with beads task management. ALL issues must have their name suffixed with the current git worktree (if any) and branch you're working on, so that multiple agents can work without colliding.
>
> You can familiarize yourself with the available commands using `bd -h`.
>
> ### Landing the Plane (Session Completion)
>
> **When ending a work session**, you MUST complete ALL steps below. Work is NOT complete until `git push` succeeds.
>
> **MANDATORY WORKFLOW:**
>
> 1. **File beads issues for remaining work** - Create issues for anything that needs follow-up
> 2. **Sync ALL beads issues to GitHub using the `gh` tool** - Preserve the project hierarchy of the issues (epic -> issue, etc). If an issue has changed, change its state on GitHub as well (updates should be reflected as new comments/posts on the issue).
> 3. **Run quality gates** (if code changed) - Tests, linters, builds
> 4. **Update issue status** - Close finished work, update in-progress items
> 5. **PUSH TO REMOTE** - This is MANDATORY:
>    ```bash
>    git pull --rebase
>    bd sync
>    git push
>    git status  # MUST show "up to date with origin"
>    ```
> 6. **Clean up** - Clear stashes, prune remote branches
> 7. **Verify** - All changes committed AND pushed
> 8. **Hand off** - Provide context for next session
>
> **CRITICAL RULES:**
> - Work is NOT complete until `git push` succeeds
> - NEVER stop before pushing - that leaves work stranded locally
> - NEVER say "ready to push when you are" - YOU must push
> - If push fails, resolve and retry until it succeeds
> ```
> *Replying to @yacineMTB:* I need a task manager program, something that I can very easily use and track my different tasks, while having them assigned to individual coding agents. Right now; I just name my tmux sessions which task I'm trying to get done. But I need something that works with my phone

- **Tweet:** https://x.com/0xfdf/status/2006807995884175661
- **Link:** https://github.com/steveyegge/beads
- **Parent:** https://x.com/yacineMTB/status/2006685073685520483
- **What:** A distributed, git-backed graph issue tracker designed for AI agents. Provides persistent memory, dependency tracking, and structured task management across multi-session workflows with GitHub integration.

---


## @Steve_Yegge - Gas Town: Coding Agent Orchestrator Launch

> Happy New Year! I've just launched my coding agent orchestrator, Gas Town, for anyone crazy enough to try it. https://t.co/xWJLZzmpZH

- **Tweet:** https://x.com/Steve_Yegge/status/2006835043503845445
- **Link:** https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04
- **What:** Announcement of Gas Town, Steve Yegge's new coding agent orchestrator platform released on New Year's Day 2026. This is a comprehensive system for orchestrating multiple AI agents in complex development workflows.

---


---



---


# Wednesday, December 31, 2025

## @0xPaulius - Screen Record App Walkthroughs to Create SaaS Specs
> pro tip: screen record a walk through of the app, then have Gemini create a spec sheet
>
> Give the spec sheet to Claude
>
> GGWP, saas done
>
> *Quoting @dabit3:* Something I wanted to see if Claude Opus 4.5 could do: clone a fully functional Billion $ SAAS product and make it at least 100x cheaper.
>
> The first product that came to mind was TypeForm because it's very popular, very expensive, and in theory, very simple.
>
> The result is OpenForm: a polished + functional and Open Source Typeform clone at ~100x less cost, that can be setup and deployed in ~15 minutes. The agent building this ran for ~35 minutes.
>
> Here are the details, technique, and the code:

- **Tweet:** https://x.com/0xPaulius/status/2006599685902127139
- **Quoted:** https://x.com/dabit3/status/2006489676924989860
- **What:** A tip for creating SaaS product specifications by screen recording workflows and having AI create spec sheets, then using those specs with Claude for implementation.

---


## @thsottiaux - Ask Questions if Request is Underspecified Skill
> Simply adding "Ask questions if my request is underspecified" at the end of a prompt to Codex works well as you might expect, but also codified it a bit more in a `$ask-questions-if-underspecified` skill that I use regularly. https://t.co/QVPidaONx6

- **Tweet:** https://x.com/thsottiaux/status/2006624682515247604
- **Link:** https://x.com/thsottiaux/status/2006624682515247604/photo/1
- **What:** A practical prompt engineering tip to include in prompts that instructs AI models to ask clarifying questions when requests lack sufficient detail or context.

---

## ## @0xRaduan - Claude Code Internal Documentation Reference

> @nummanali @jarrodwatts https://t.co/6EbR6UUCxd
>
> It's been out for quite a bit at this point. There are some docs around it, but those are internal.

- **Tweet:** https://x.com/0xRaduan/status/2006326743473267052
- **Link:** https://github.com/anthropics/claude-code/issues/12836#issuecomment-3656762362
- **What:** A reply referencing Claude Code documentation and an issue discussion, suggesting that certain features have been available but lack public documentation.

---

## ## @ankurnagpal - Tax-Advantaged Money Market Fund Yields

> PSA for anyone in a high tax bracket:
>
> You can potentially save a lot of money by investing in tax-advantaged money market funds vs a high-yield savings account
>
> VYFXX is paying me a tax-equivalent yield of ~5.72% right now, my bank account is at 3.25%
>
> Will save me thousands https://t.co/5xGYvWxdp7

- **Tweet:** https://x.com/ankurnagpal/status/2006373258439082092
- **What:** Financial advice comparing tax-efficient investment strategies for high earners, showing how Vanguard money market funds (VYFXX) can provide better after-tax returns than traditional high-yield savings accounts.

---

## ## @alexhillman - Automated Bookmark Processing with Bird CLI

> New workflow thanks to @steipete's awesome Twitter CLI, bird
>
> 1 - bookmark a tweet
> 2 - bird grabs new bookmarks every 60 seconds
> 3 - agent reads the tweet and depending on contents adds to a queue of things to review, try, or simply add to my knowledge base.
>
> Auto saves links, podcasts, YouTube vids, etc. Including transcripts and quotes that would be useful or interesting to me.
>
> Auto suggests ways to integrate ideas and open source projects into the JFDI system.
>
> Pretty excited to see this one compound.

- **Tweet:** https://x.com/alexhillman/status/2006420618091094104
- **What:** Description of an automated workflow using the bird Twitter CLI that periodically fetches bookmarks, processes them with an AI agent, and intelligently categorizes content for later review or knowledge base integration.

---


---



---


# Tuesday, December 30, 2025

## @koylanai - Digital Brain skill for Claude Code
> Agent Skills for Context Engineering - digital brain implementation

- **Tweet:** https://x.com/koylanai/status/2005857134311854480
- **Link:** https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering
- **What:** GitHub repository containing a digital brain skill implementation for Claude Code, enabling advanced context engineering and knowledge management capabilities.

---


---


## @max_sixty - Worktrunk: Git Worktree Manager for AI Agents

> Announcing Worktrunk! A git worktree manager, designed for running AI agents in parallel.

A few points on why I'm so excited about the project, and why I hope it becomes broadly adopted 🧵 https://t.co/Ku6XsRofbQ

- **Tweet:** https://x.com/max_sixty/status/2006077845391724739
- **What:** Introduction to Worktrunk, a git worktree management tool optimized for parallel AI agent execution.

---

---



---


# Monday, December 29, 2025

## @aakashgupta - Smartphone addiction and dopamine regulation
> Discussion about how smartphone addiction affects dopamine levels and causes brain fog

- **Tweet:** https://x.com/aakashgupta/status/2005552148218851769
- **What:** Explores the connection between smartphone dependency and dopamine dysregulation as a root cause of cognitive impairment and brain fog.

---


## @pk_iv - Browserbase cloud browser plugin for Claude Code
> Cloud browser plugin enabling Claude Code to interact with web applications

- **Tweet:** https://x.com/pk_iv/status/2005694099123478579
- **What:** Browserbase cloud-based browser solution that extends Claude Code's capabilities for web automation and interaction.

---


## @CasJam - Claude Code for video post-production
> Building a custom Claude Code app that handles ~80% of post-production in a single command

- **Tweet:** https://x.com/CasJam/status/2005765644394844261
- **What:** Demonstrates practical applications of Claude Code for automating video post-production: transcription, analysis, clip cutting, and script writing.

---


## @steipete - Shipping at Inference Speed
> Confession: I ship code I never read. Here's my 2025 workflow.

- **Tweet:** https://x.com/steipete/status/2005451576971043097
- **Link:** https://steipete.me/posts/2025/shipping-at-inference-speed
- **What:** Blog post discussing shipping software at inference speed, embracing rapid AI-assisted development cycles.

---


## @michael_chomsky - ResponsiveDialog Component Pattern
> I do this for every project (quote of @jordienr about drawer on mobile, dialog on desktop)

- **Tweet:** https://x.com/michael_chomsky/status/2005454822083076172
- **What:** Endorsement of the responsive dialog component pattern that adapts between drawer and dialog based on viewport.

---


---


---


# Sunday, December 28, 2025

## @rudrank - Awesome Claude Code Plugins List
> I want to make the most out of Claude Code... One thing to explore more are plugins

- **Tweet:** https://x.com/rudrank/status/2005215898593034525
- **Link:** https://github.com/ccplugins/awesome-claude-code-plugins
- **What:** Comprehensive registry of Claude Code plugins: slash commands, subagents, MCP servers, and hooks across multiple specializations.

---


## @mattpocockuk - PRD with Passing Tests Approach
> Tired: PRD + Multi-phase plan. Wired: PRD with 'passing' status on each test case

- **Tweet:** https://x.com/mattpocockuk/status/2005232347374141888
- **What:** Development methodology that combines PRDs with test-driven specification, each feature is one context window large.

---


## @0xSero - Docker MCP Toolkit for Token Savings
> This is how you should use MCPs if you can. Instead of loading all MCPs, load 1 which discovers the rest.

- **Tweet:** https://x.com/0xSero/status/2005355435570958553
- **Link:** https://docs.docker.com/ai/mcp-catalog-and-toolkit/toolkit/
- **What:** Docker MCP toolkit for dynamic MCP discovery, saving 20k tokens by loading one MCP that discovers others.

---


---


---


# Saturday, December 27, 2025

## @systematicls - Shared Tweet/Article
> https://t.co/FQe5bCBqW1

- **Tweet:** https://x.com/systematicls/status/2004900241745883205
- **What:** A shared tweet or article link. The expanded content points to a Twitter article that may contain relevant technical or industry insights.

## @aakashgupta - Karpathy "dramatically behind" commentary
> Andrej Karpathy literally built the neural networks running inside coding assistants... If he feels "dramatically behind" as a programmer, that tells you everything.

- **Tweet:** https://x.com/aakashgupta/status/2004713516930855284
- **What:** Commentary on Karpathy's confession about feeling behind, noting the new stack of agents, subagents, prompts, contexts, memory, modes, etc.

---


## @adocomplete - Claude Code sandboxing docs link
> Learn more about Claude Code Sandboxing

- **Tweet:** https://x.com/adocomplete/status/2004977725136888287
- **Link:** https://code.claude.com/docs/en/sandboxing
- **What:** Link to Claude Code sandboxing documentation covering security and isolation features.

---


## @bcherny - Reply with screenshot/image
> Visual content reply

- **Tweet:** https://x.com/bcherny/status/2004947522889162834
- **What:** Visual reference or example shared in reply format.

---


---


---


# Friday, December 26, 2025

## @tom_doerr - StenoAI local meeting transcription
> Transcribes and summarizes meetings locally using small language models

- **Tweet:** https://x.com/tom_doerr/status/2004452266640634056
- **Link:** https://github.com/ruzin/stenoai
- **What:** Privacy-focused AI meeting transcription and summarization using locally hosted small language models.

---


## @trq212 - Claude Code prompt template for non-technical users
> Full template for asking Claude Code to onboard a non-technical user

- **Tweet:** https://x.com/trq212/status/2004575721235141115
- **What:** Comprehensive prompt template to help non-technical users interact with Claude Code effectively.

---


## @tom_doerr - AppScreen 3D screenshot mockups
> Generates screenshots with 3D device mockups

- **Tweet:** https://x.com/tom_doerr/status/2004616272844087678
- **Link:** https://github.com/YUZU-Hub/appscreen
- **What:** Tool to create beautiful 3D device mockups and screenshot presentations for iOS App Store.

---


## @tom_doerr - Unwatched RSS YouTube player
> RSS YouTube player for Apple devices with chapter skipping and no ads

- **Tweet:** https://x.com/tom_doerr/status/2004627732148232504
- **Link:** https://github.com/fer0n/Unwatched
- **What:** RSS feed based YouTube video player for iOS, macOS, tvOS with chapter support and no ads.

---


## @cameronpetitti - Crosspost app launch
> Years of work is finally ready. Introducing Crosspost.

- **Tweet:** https://x.com/cameronpetitti/status/2004631941782667685
- **Link:** https://www.crosspost.app/
- **What:** Application for managing and crossposting content across multiple social media platforms.

---


## @calebporzio - Chrome game changer addition
> woah...game changer addition to chrome

- **Tweet:** https://x.com/calebporzio/status/2004651797533917261
- **What:** Media post highlighting a significant Chrome feature or addition.

---


## @seconds_0 - Claude Code onboarding prompt for non-technical users
> Here's my "ask claude code to onboard a nontechnical user" prompt

- **Tweet:** https://x.com/seconds_0/status/2004684813773799543
- **Link:** https://code.claude.com/docs/
- **What:** Comprehensive interview-based onboarding prompt for non-technical users with communication rules and quality standards.

---


## @ryanvogel - Video post
> Video demonstration

- **Tweet:** https://x.com/ryanvogel/status/2004729931943870612
- **What:** Video content post.

---


---


---


# Thursday, December 25, 2025

## @hdjirdeh - streamdown vs react-markdown
> Moved away from react-markdown to streamdown and although its not perfect, its so much better.

- **Tweet:** https://x.com/hdjirdeh/status/2004020171808428520
- **What:** Comparison between streamdown and react-markdown for rendering markdown in React with improved formatting and interactive code blocks.

---


## @PovilasKorop - AI Adoption Quote
> How to adopt AI in your company (or personally). Main point: There is no AI course you can "finish."

- **Tweet:** https://x.com/PovilasKorop/status/2004099293389463793
- **What:** Quote highlighting key insight from Steve Ike's AI adoption playbook thread about constant experimentation.

---


## @tom_doerr - BreakFree iOS Sideloading Tool
> Sideloads apps on iOS using DNS and certificates

- **Tweet:** https://x.com/tom_doerr/status/2004208111532335470
- **Link:** https://github.com/FrizzleM/BreakFree
- **What:** Free iOS shortcut for sideloading unlimited apps using DNS and public certificates exploit.

---


---


## @jedisct1 - Logging Sucks

> Logging sucks https://t.co/mbNa6TCKCv

- **Tweet:** https://x.com/jedisct1/status/2004295982696354213
- **What:** Critical examination of traditional logging approaches and their limitations in observability, introducing wide events as an alternative solution.

---


## @bcherny - Claude Code File Read Token Limit Configuration

> @karpathy Added! In the next version of Claude Code, you can use the  CLAUDE_CODE_FILE_READ_MAX_OUTPUT_TOKENS env var.

eg. "CLAUDE_CODE_FILE_READ_MAX_OUTPUT_TOKENS=1234567 claude"

You can also add this to the "env" section in your settings.json

- **Tweet:** https://x.com/bcherny/status/2004337225866375655
- **What:** Announcing a new environment variable in Claude Code to configure maximum output tokens for file reads, addressing token context limits.

**Parent context:** @karpathy reported hitting token file context limits and asked about equivalent configuration options for the Read tool.

---

---



---


# Tuesday, December 23, 2025

## @steve_ike_ - AI Adoption Playbook
> This might be the cleanest AI adoption playbook inside a real product org I've seen.

- **Tweet:** https://x.com/steve_ike_/status/2003497265495785523
- **What:** 15-point comprehensive playbook covering practical approaches to implementing AI across organizations, from "How I AI" podcast.

---


---


---


# Wednesday, December 17, 2025

## @JackPosobiec - Christian Alternative Learning Content for Children
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://t.co/gkfuc6fVjQ

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Recommendation for a Christian children's educational video as an alternative to secular toddler learning content.

---


## @RapidResponse47 - Trump Accounts Government Portal Update
> JUST UPDATED: https://t.co/FKL1oV36R4 https://t.co/YYG4diAEni

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **Link:** https://trumpaccounts.gov/
- **What:** Announcement of an update to the Trump accounts government portal with accompanying screenshot.

---


## @Yampeleg - Claude Code v2.0.71 Release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://t.co/czN80tHvAY

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Strong recommendation to update Claude Code to version 2.0.71, indicating a significant or notable release with positive features.

---


## @JackPosobiec - Christian Toddler Learning Video Alternative
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
> https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Christian-themed toddler educational content featuring Silly Miss Lily, positioned as a faith-based alternative to Ms Rachel videos.

---


## @RapidResponse47 - Trump Accounts Portal Update
> JUST UPDATED: https://trumpaccounts.gov/

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **Link:** https://trumpaccounts.gov/
- **What:** Update notification for Trump Accounts portal website (currently behind Cloudflare challenge, content unavailable).

---


## @JackPosobiec - Silly Miss Lily Christian toddler education content
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://t.co/gkfuc6fVjQ

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Educational content for Christian toddlers featuring Silly Miss Lily as an alternative to secular education channels like Ms. Rachel.

---


## @RapidResponse47 - Trump accounts government update
> JUST UPDATED: https://t.co/FKL1oV36R4 https://t.co/YYG4diAEni

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **What:** Update notice regarding Trump accounts with government website reference.

---


## @Yampeleg - Claude Code v2.0.71 release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://t.co/czN80tHvAY

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic recommendation to update Claude Code to v2.0.71, indicating significant improvements in the release.

---


## @JackPosobiec - Christian Learning Content for Toddlers
> Want a Christian alternative to Ms Rachel that your kids will love? Here you go: The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE
- **What:** Jack recommends a Christian toddler learning video as an alternative to secular educational content for young children.

---


## @RapidResponse47 - Government Accounts Update
> JUST UPDATED: https://trumpaccounts.gov/

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **What:** Brief announcement regarding an update to government accounts information with accompanying image.

---


## @Yampeleg - Claude Code v2.0.71 Release Update
> Stop what u do and update Claude Code to v2.0.71. They cooked. https://x.com/Yampeleg/status/2001360661700596119/photo/1

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **Tags:** [[claude-code]] [[developer-tools]]
- **What:** Enthusiastic recommendation to update to Claude Code version 2.0.71, suggesting significant improvements or new features have been released.

---


## @JackPosobiec - Christian alternative to Ms Rachel toddler content
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://t.co/gkfuc6fVjQ

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Recommendation for a Christian-themed toddler learning video as an alternative to Ms Rachel, featuring Silly Miss Lily teaching about Baby Jesus and Christmas.

---


## @RapidResponse47 - Trump accounts site update
> JUST UPDATED: https://t.co/FKL1oV36R4 https://t.co/YYG4diAEni

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **What:** Announcement of an update to trumpaccounts.gov with accompanying image documentation.

---


## @JackPosobiec - Christian alternative to Ms Rachel for toddler learning
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://t.co/gkfuc6fVjQ

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** YouTube video recommendation for Christian-themed educational content for toddlers as an alternative to Ms Rachel.

---


## @RapidResponse47 - Trump accounts update
> JUST UPDATED: https://t.co/FKL1oV36R4 https://t.co/YYG4diAEni

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **Link:** https://trumpaccounts.gov/
- **What:** Update notification with links to Trump accounts government resource and associated media.

---


## @JackPosobiec - Christian Toddler Learning Alternative
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
> https://www.youtube.com/watch?v=5egr1nOI4SE

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE
- **What:** YouTube video recommendation for Christian-themed toddler educational content as an alternative to secular learning programs.

---


## @JackPosobiec - Christian alternative to Ms Rachel for toddlers
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://t.co/gkfuc6fVjQ

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Promotional recommendation for Christian-focused toddler educational content featuring Baby Jesus story and Christmas themes.

---


## @RapidResponse47 - Trump accounts government website update
> JUST UPDATED: https://t.co/FKL1oV36R4 https://t.co/YYG4diAEni

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **What:** Announcement of updated Trump accounts government website with accompanying visual content.

---


## @Yampeleg - Claude Code v2.0.71 major update
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://t.co/czN80tHvAY

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic endorsement of Claude Code v2.0.71 update, suggesting significant improvements in the latest release.

---


## @JackPosobiec - Christian Alternative to Ms Rachel Educational Content
> Want a Christian alternative to Ms Rachel that your kids will love?
>
> Here you go:
>
> The Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning
>
> https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** Recommendation for Christian-themed toddler learning content featuring Silly Miss Lily as an alternative to mainstream educational resources.

---


## @JackPosobiec - Christian Alternative Educational Content
> Want a Christian alternative to Ms Rachel that your kids will love? \n\nHere you go: \n\nThe Story of Baby Jesus & The First Christmas with Silly Miss Lily | Christian Toddler Learning

- **Tweet:** https://x.com/JackPosobiec/status/2001298327342633418
- **Link:** https://www.youtube.com/watch?v=5egr1nOI4SE&feature=youtu.be
- **What:** YouTube video recommendation for Christian toddler educational content as an alternative to mainstream programs.

---


## @RapidResponse47 - News Update
> JUST UPDATED: https://trumpaccounts.gov/

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **What:** Notification of an update to trumpaccounts.gov with associated media/image content.

---


---


# Tuesday, December 16, 2025

## @nicolaygerold - Tool Search and Discovery in LLM Agents
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
>
> https://t.co/QOiUXSrKXb

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Technical analysis on why deferred tool loading in LLM agents requires discovery mechanisms beyond simple search.

---


## @QwQiao - Coinbase's Evolution Into a Banking Platform
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Investment perspective on Coinbase's shift from a crypto exchange to a bank-like institution with bundled financial products and loyalty programs.

---

---

## @nicolaygerold - Tool Search as Discovery Not Just Search
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
> https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Nicolay Gerold discusses tool search and discovery in LLM agents, exploring why deferred tool loading with context management challenges isn't as simple as it sounds.

---


## @QwQiao - Coinbase's Bank Strategy with Premium Loyalty Program
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's strategic pivot from cryptocurrency exchange to full-service bank with premium loyalty tier (similar to Amazon Prime or Costco Black Card), creating high customer lock-in.

---

---

## @nicolaygerold - Tool search and discovery in LLM agents
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
>
> https://t.co/QOiUXSrKXb

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Analysis of why deferred tool loading in LLM agents requires discovery mechanisms rather than simple search. Addresses context management and tool availability in agent systems.

---


## @QwQiao - Coinbase's transformation to bancorp with loyalty programs
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's strategic pivot from exchange to bancorp using premium tier loyalty program model similar to Amazon Prime and Costco.

---

---

## @nicolaygerold - Tool Search in LLM Agents: From Discovery to Implementation
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search: https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **Tags:** [[ai-agents]] [[tools]] [[context-management]]
- **What:** Nicolay discusses deferred tool loading in LLM agents and why tool discovery should be more sophisticated than simple search, addressing the challenge of managing context windows effectively.

---


## @QwQiao - Coinbase's Strategic Pivot: From Exchange to Banking Platform
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank. ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading. they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program. bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **Tags:** [[crypto]] [[coinbase]] [[fintech]] [[banking]]
- **What:** QwQiao analyzes Coinbase's long-term strategy of transitioning from an exchange to a banking platform through loyalty programs and bundled financial products, similar to Amazon Prime and Costco's models.

---

---

## @nicolaygerold - Tool search should be discovery, not just search
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
> https://t.co/QOiUXSrKXb

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Nicolay explores tool discovery mechanisms in LLM agents, arguing that deferred tool loading should prioritize discovery over simple search to maintain context efficiency.

---


## @QwQiao - Coinbase's long-term strategy of becoming a bank
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's pivot from an exchange to a bank-like platform with a loyalty program, using their premium Amex card and fee structures to build defensibility similar to Amazon Prime.

---

---

## @nicolaygerold - Tool search should not be search but discovery
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
>
> https://t.co/QOiUXSrKXb

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Article about deferred tool loading in LLM agents and why tool search should focus on discovery rather than just search in context management.

---


## @QwQiao - Coinbase's strategy to become a banking platform
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's transition from a crypto exchange to a full-service banking platform with loyalty programs similar to Amazon Prime or Costco.

---

---

## @nicolaygerold - Tool Search: Discovery vs Search in LLM Agents
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
> https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Explores deferred tool loading in LLM agents and why tool discovery should prioritize context management over simple search mechanisms.

---


## @QwQiao - Coinbase's Evolution: From Exchange to Digital Bank
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's strategic pivot from cryptocurrency exchange to full-service digital bank with premium loyalty program, creating stickier business model.

---

---

## @QwQiao - Coinbase transforming from exchange to bank
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's strategic shift from pure exchange to banking services through premium membership tiers and integrated financial products. Predicts significant long-term growth potential.

---

---

## @nicolaygerold - Tool Search Should Be Discovery Not Search
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
>
> https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Nicolay explores how deferred tool loading in LLM agents requires rethinking tool discovery mechanisms rather than traditional search patterns.

---


## @QwQiao - Coinbase's Long-Term Strategy: From Exchange to Bank
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.
>
> ive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.
>
> they r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.
>
> bullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Analysis of Coinbase's shift from an exchange business model to a bank-like model with loyalty programs similar to Amazon Prime, positioning for long-term customer stickiness and growth.

---

---

## @nicolaygerold - Tool Search and Agent Context Management
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search: https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Technical essay on tool search and discovery in LLM agents, exploring why deferred tool loading is more complex than it initially appears.

---


## @QwQiao - Coinbase's Long-term Strategy as a Bank
> i might be a bit late to realize this, but after being a "coinbase one" customer and their amex card i kinda get where coinbase is going long term — they want to become a bank.\n\nive already switched from other credit cards to the coinbase amex card cuz its nice to get 4% cashback in btc. i also get a big discount on my trading fees. but to get these benefits i need to pay an annual fee and lock in $200k. this is akin to amazon prime and costco black card, creating enormous customer loyalty. later they'll probably bundle it with other financial products like stock trading.\n\nthey r moving from a "goddamn exchange business" with little defensibility (munger's voice) to something much stickier — a bank with a loyalty program.\n\nbullish $coin, probably another 10x left over 1-2 decades.

- **Tweet:** https://x.com/QwQiao/status/2001051586932396257
- **What:** Investment thesis on Coinbase's shift from exchange to banking business model through premium membership and customer loyalty programs.

---

## @jaredpalmer - Optimizing MCP Integration with Claude Code

> &gt; ask claude code to read the code mode mcp blog post and then to introspect compile/emit your mcp to a skill + script files
> &gt; reduce token usage by 80-98% and prevent poisoning your context with mcp bloat
> &gt; profit

- **Tweet:** https://x.com/jaredpalmer/status/2000949527571038687
- **What:** Technique for optimizing MCP (Model Context Protocol) usage in Claude Code by compiling MCP definitions into skills and scripts, reducing token usage by 80-98% and avoiding context pollution.

---

---



---


# Monday, December 15, 2025

## @bull_genius - Pacific Rim Megaquake Risk Analysis

> earthquake GCR / megaquake theory explained for dummies
>
> in the past few days theres been quite some attention on @BlerGoom and @mxdondevivo warning of an imminent mag 10 massive earthquake (never seen before) in the nw pacific rim region which would be an extreme tail risk event that would significantly cripple markets and cause huge damage in the region
>
> while new to the topic ive been doing my part to understand where they're coming from (pls correct if i got it totally wrong).
>
> my map here shows 6.5+ earthquakes in the region in the past 15 months.
>
> boiled down to basics: the pacific plate has been moving to NW/NNW while being locked in the southern part causing a strange silence in south pacific/south america which is usually a seismically extremely active spot. on any given year there are usually multiple 6.5 happening there, while its in total silence now.
>
> on the other side, we have seen a rare pattern of activity in places which have been calmer previously, with 7+ quakes happening at all crucial points (tohoku subduction zone, kuril-kamchatka trench, aleutian trench and alaska) and a huge 8.8 in kamchatka, which is one of the 5 strongest quakes in the past 80 years and on record.
>
> last week we had a 7.6 + a consecutive swarm of earthquakes with activity very similar to the buildup to the 2011 great tohoku earthquake which was a 9.1 and damaged fukushima nuclear plant. japan has issued a megaquake warning for the first time since 2011.
>
> this all combined with increased anomalous space weather (solar stroms) which has been linked to trigger seismic events on earth leads to an elevated risk of a very large seismic event in the nw of the pacific with all of the market events on the map being foreshocks to the big one.
>
> earthquakes are very hard to predict in their timing and magnitude but one can agree we have only like 100+ years of data and the current setup looks very much anomalous and the tail risk is definitely much higher than usual.
>
> wdwt chat?

- **Tweet:** https://x.com/bull_genius/status/2000508129163755522
- **What:** Detailed analysis of elevated seismic risk in Northwest Pacific region, documenting unusual earthquake patterns, regional lockups, and increased solar activity. Discusses potential magnitude 10 event as tail risk with significant market and regional damage implications.

---

---



---


# Sunday, December 14, 2025

## @Yampeleg - Claude Code Subagents RAM Consumption Bug

> Claude Code team, please listen!
>
> RAM consumption on Linux explodes (+100GB) when using subagents.
>
> This is a HUGE bug affecting thousands of users for months.
>
> It's all over GitHub and Reddit, with tens of issues and long threads of users trying to debug it.
>
> The current "solutions" people come up with are basically sophisticated prompt engineering tricks, begging Claude not to use subagents in clever ways.
>
> This reproduces even on a clean, fresh Ubuntu install out of the box (no tricks).
>
> I run a 256GB RAM machine and I can't use parallel agents whatsoever, no matter which terminal I use or which OS optimizations I tried.
>
> Subagents are one of the best Claude Code features, and right now they're basically unusable for many of us.
>
> This is 100% a bug.
>
> The actual RAM needed by the agents is much lower in practice, there is a bug in the CLI engine that spawns them.
>
> I personally use the Agents SDK in a custom tool to bypass Claude Code's CLI from spawning agents on its own.
>
> It works flawlessly with tens of agents in parallel and the RAM consumption stays reasonable.
>
> Thank you for your attention to this matter!
>
> —- A happily paying user on max plan

**Quoted context from @claudeai:** "We're releasing more upgrades to Claude Code CLI: - Async subagents - Instant compact - Customer session names - Usage stats"

- **Tweet:** https://x.com/Yampeleg/status/2000301662376808913
- **What:** Detailed bug report about massive RAM consumption (100GB+) when using subagents in Claude Code CLI on Linux. User notes the issue affects thousands and has workaround using Agents SDK directly, suggesting the problem is in how the CLI spawns agents rather than the agents themselves.

---


## @deepfates - Using "Idiomatic" Token for Edit Prompting

> If you're prompting for edits to anything, like code or text or images, You can get a lot of mileage out of the token "idiomatic"

- **Tweet:** https://x.com/deepfates/status/2000306376468533344
- **What:** Quick tip suggesting the word "idiomatic" is a valuable token to use when prompting for edits to code, text, or images to improve output quality.

---


## @avidseries - Terrorism Statistics by Religion

> Percentage of total global deaths from terrorism this century attributed to religiously-motivated Muslim/Islamist groups or individuals: 86-95%
>
> Percentage attributed to religiously-motivated Christian groups or individuals: Less than 0.1%
>
> (Sources: Various, including NYT, GTI, GTD, Fondapol.)

**Reply to @Blahhhhhh34:** Extended list comparing Christian and Muslim-attributed violent incidents throughout history.

- **Tweet:** https://x.com/avidseries/status/2000307562902585699
- **What:** Statistical comparison of terrorism deaths by religious motivation this century. Reply in broader debate about religious violence attribution with cited sources.

---

---



---


# Saturday, December 13, 2025

## @startupideaspod - Anthropic just revealed how to 10x your Claude outputs...
> Anthropic just revealed how to 10x your Claude outputs

 These are the 3 rules most people ignore

- Rule 1: Tone of collaboration — be friendly, clear, and firm 
- Rule 2: Principle of explicitness — action verb + quantity + audience 
- Rule 3: Defined box — constraints beat open fields

The KEY: Boundaries unlock creativity

You have to give it style constraints 

You have to ban specific words 

You have to define length, tone, and audience

A vague prompt like "write a story about a detective" = AI slop

An architected brief like "500 words, Raymond Chandler style, robot detective on Mars, no word 'cyber'" = magic

Stop treating prompts like Google searches 

Start treating them like creative briefs for a teammate

Use this framework to get 10x more out of LLMs

- **Tweet:** https://x.com/startupideaspod/status/1999856845004141041
- **What:** Guidance on effective prompt engineering with Claude - focusing on tone, explicitness, and constraints to unlock AI creativity.

---


## @_simonsmith - GPT-5.2 Pro + NotebookLM slides is a consulting company. I'd...
> GPT-5.2 Pro + NotebookLM slides is a consulting company. I'd watch hiring in big consulting firms closely in 2026. Once people figure this out...

- **Tweet:** https://x.com/_simonsmith/status/1999910106381906199
- **What:** Observation about AI language models creating new opportunities in consulting by automating presentations and slides generation.

---


## @doodlestein - I like to make sure that I'm making some forward progress on...
> I like to make sure that I'm making some forward progress on every one of my active projects each day, even when I'm too busy to spend real mental bandwidth on all of them every single day.

So I've come up with a few prompts that I use a lot with the agents so they're always doing some level of polishing/checking/fixing and general improvement.

The models are basically good enough now, and I have enough unit tests and end-to-end integration tests, that I'm not too worried about them going rogue and making big mistakes. Plus, if one of them did, the other agents would probably catch it and fix it themselves.

Some common ones I use are presented here:

"I want you to sort of randomly explore the code files in this project, choosing code files to deeply investigate and understand and trace their functionality and execution flows through the related code files which they import or which they are imported by. Once you understand the purpose of the code in the larger context of the workflows, I want you to do a super careful, methodical, and critical check with "fresh eyes" to find any obvious bugs, problems, errors, issues, silly mistakes, etc. and then systematically and meticulously and intelligently correct them. Be sure to comply with ALL rules in AGENTS dot md."

and 

"Ok can you now turn your attention to reviewing the code written by your fellow agents and checking for any issues, bugs, errors, problems, inefficiencies, security problems, reliability issues, etc. and carefully diagnose their underlying root causes using first-principle analysis and then fix or revise them if necessary? Don't restrict yourself to the latest commits, cast a wider net and go super deep! Use ultrathink."

When I'm feeling dissatisfied with a project but don't have the energy to actually grapple with things directly, I will do one of these (but only with Opus 4.5 or now GPT 5.2 with extra high thinking effort):

"Great, now I want you to super carefully scrutinize every aspect of the application workflow and implementation and look for things that just seem sub-optimal or even wrong/mistaken to you, things that could very obviously be improved from a user-friendliness and intuitiveness standpoint, places where our UI/UX could be improved and polished to be slicker, more visually appealing, and more premium feeling and just ultra high-quality, like Stripe-level apps."

You can even follow that one up in Codex by queueing up these messages, which will apply to the many suggestions it came up with for improving the project:

"OK so please take ALL of that and elaborate on it more and then create a comprehensive and granular set of beads for all this with tasks, subtasks, and dependency structure overlaid, with detailed comments so that the whole thing is totally self-contained and self-documenting (including relevant background, reasoning/justification, considerations, etc.-- anything we'd want our "future self" to know about the goals and intentions and thought process and how it serves the over-arching goals of the project.)"

followed by:

"Check over each bead super carefully-- are you sure it makes sense? Is it optimal? Could we change anything to make the system work better for users? If so, revise the beads. It's a lot easier and faster to operate in "plan space" before we start implementing these things!"

And then:

"OK, so start systematically and methodically and meticulously and diligently executing those remaining beads tasks that you created in the optimal logical order! Don't forget to mark beads as you work on them."

And then a couple "proceed" messages, then a final:

"Great, now I want you to carefully read over all of the new code you just wrote and other existing code you just modified with "fresh eyes" looking super carefully for any obvious bugs, errors, problems, issues, confusion, etc. Carefully fix anything you uncover."

Note that these are all entered up front and go into a queue of messages which codex processes one at a time when it finished the previous one; unfortunately, this workflow doesn't work with Claude Code because it interrupts the agent with your follow up messages.

Anyway, then you can come back 3+ hours later to see the incredible amount of work done autonomously for you. This works way better now with GPT 5.2 with extra effort.

Finally, have Claude commit it all for you with this:

"Now, based on your knowledge of the project, commit all changed files now in a series of logically connected groupings with super detailed commit messages for each and then push. Take your time to do it right. Don't edit the code at all. Don't commit obviously ephemeral files. Use ultrathink."

I do this every day, multiple times a day, for like 7+ projects now, and keep 3 machines busy constantly (and all my various subscriptions, although I'll have to add even more soon at this rate).

Oh yeah, and each of these blurbs takes under a second to do with a single button press using my little command palette gizmo (plus its new little brother version I got for a second machine and which only costs $60 on Temu!), see pics.

- **Tweet:** https://x.com/doodlestein/status/1999934160442687526
- **What:** Framework for using AI agents to continuously improve code through autonomous review, fixing, and polishing of active projects.

---


## @JamesAFurey - https://t.co/tqfgFk3Z2d
> https://t.co/tqfgFk3Z2d

- **Tweet:** https://x.com/JamesAFurey/status/1999958721611575501
- **Reply to:** Reminder: You can (and should) teach your child to read. It takes one book ($16.99 on Amazon).
- **What:** Reply about resource for teaching children to read using a structured, scripted method that only requires 10 minutes daily.

---

---



---


# Friday, December 12, 2025

## @pvncher - Have this workflow where I get Claude to pull down new logs...
> Have this workflow where I get Claude to pull down new logs from the @getsentry cli, and then pipe them into markdown docs.

Then just kick off context builder GPT-5.2 to analyze the trace and surface relevant context, to then hand off off a bug resolution to 5.2 Pro. https://t.co/HqQfWeoMqd

- **Tweet:** https://x.com/pvncher/status/1999505400832364756
- **What:** Review and analysis of LLM capabilities and performance metrics.

---


## @Baconbrix - @tylerangert @Dimillian Expo / React Native apps can do this...
> @tylerangert @Dimillian Expo / React Native apps can do this too. https://t.co/Kv7uiW9pJv

- **Tweet:** https://x.com/Baconbrix/status/1999567503245070439
- **What:** Discussion about React Native and Expo capabilities for web development features.

**In reply to:** @tylerangert - @Dimillian yes. it likely needs to be a web project.

**Quoted:** @kzzzf - Right-click to inspect with access to components hierarchy and jump-to-source. Y

---

---

## @tommoor - Okay, can confirm https://t.co/uDiRCD5Qev finds legit bugs.
> Okay, can confirm https://t.co/uDiRCD5Qev finds legit bugs.

- **Tweet:** https://x.com/tommoor/status/1999651772487410104
- **What:** Tool for finding bugs in codebases through deep analysis.

---

---



---


# Thursday, December 11, 2025

## @mattshumer_ - I've had access to GPT-5.2 since November 25th....
> I've had access to GPT-5.2 since November 25th.

Since then, I've used it as my daily-driver, pushing it to its limits.

It beats out Opus 4.5 in most things I tried, but there's a (big) catch.

Here's my review of GPT-5.2: https://t.co/GVU1rXRZ5r

- **Tweet:** https://x.com/mattshumer_/status/1999182246616682964
- **What:** Review and analysis of LLM capabilities and performance metrics.

---


## @arcprize - A year ago, we verified a preview of an unreleased version o...
> A year ago, we verified a preview of an unreleased version of @OpenAI o3 (High) that scored 88% on ARC-AGI-1 at est. $4.5k/task

Today, we’ve verified a new GPT-5.2 Pro (X-High) SOTA score of 90.5% at $11.64/task

This represents a ~390X efficiency improvement in one year https://t.co/9T47FdZ5Ry

- **Tweet:** https://x.com/arcprize/status/1999182732845547795
- **What:** Review and analysis of LLM capabilities and performance metrics.

---

---



---


# Wednesday, December 10, 2025

## @PaternalLegacy - 26 weapons grade parenting tips:...
> 26 weapons grade parenting tips:

1/ Give them a "heads up," 5 minutes until bedtime, 10 minutes before leaving the playground

2/ Look at the world more through their eyes

3/ Don’t discipline like an angry madman. Stay calm and firm, model how you want THEM to resolve conflict

4/ Let them argue their case respectfully. Teaches negotiation and critical thinking

5/ Skip the long lectures

6/ Use natural consequences: forgot homework? Let them explain it to the teacher. Forgot their lunch? They'll figure it out

7/ Be consistent and follow through. "We are leaving the playground if you don't stop..."

8/ Make "How can I help?" part of YOUR vocabulary. It builds reliability

9/ Share your unseen efforts: hustling for work, hitting the gym. Actions speak louder than words but when they can’t see it, TELL THEM

10/ Teach accountability by modeling it yourself: “I was wrong. sorry”

11/ Create family traditions like weekly movie nights, Sunday pancakes, whatever works

12/ More game nights

13/ Take an interest in their interests: video games, books, sports... do it with them.

14/ Hike together. Nature slows time and generates gratitude

15/ Build something. LEGO, puzzles, a fort, the Amazon delivery box

16/ Teach them skills: tie knots, start a fire, read a map

17/ Introduce chess or checkers. Start early

18/ Let them plan a family outing or navigate you there (they can get you through the airport)

19/ Always greet your wife with love. That moment sets the tone for the family

20/ Share some challenges (age appropriate)

21/ Respect their privacy. Knock before entering their room

22/ Teach the value of money early: "wants vs. needs," compounding, saving, etc

23/ Let them see you sweat

24/ Teach them to cook. Start small: eggs, pancakes, cookies. Embrace the mess

25/ No screens at meals ever

26/ Prioritize movement as a UNIT: family walks, workouts, hikes, dance-offs- whatever gets the everyone in synch

- **Tweet:** https://x.com/PaternalLegacy/status/1998760273604419586
- **What:** Collection of practical parenting strategies focused on communication, consistency, and modeling positive behavior.

---

---



---


# Thursday, December 4, 2025

## @OnlyXuanwo - AGENTS Framework for GPT-5.1-Codex
> Here is my AGENTS md which works great on gpt-5.1-codex-max, especially on high reasoning level.
>
> This should make you a MAX 200x developer, try it and let me know what you think.
>
> https://gist.github.com/Xuanwo/fa5162ed3548ae4f962dcc8b8e256bed

- **Tweet:** https://x.com/OnlyXuanwo/status/1996572217266811196
- **Link:** https://gist.github.com/Xuanwo/fa5162ed3548ae4f962dcc8b8e256bed
- **What:** An AGENTS markdown framework optimized for GPT-5.1-Codex-Max that claims to increase developer productivity up to 200x, particularly effective for high reasoning-level tasks.

---


## @ericzakariasson - Preventing Agent Hallucinations with Contextual Prompting
> append this prompt to prevent agent hallucinations:
>
> > ask more questions until you have enough context to give an accurate & confident answer
>
> it also helps you discover edge cases you might not have thought about. it's not a silver bullet, but it's a step in the right direction

- **Tweet:** https://x.com/ericzakariasson/status/1996618759105376554
- **What:** A simple prompt injection technique that reduces AI agent hallucinations by requiring the model to ask clarifying questions until it has sufficient context. Helps identify edge cases while being a pragmatic mitigation (not a complete solution) to hallucination problems.

---


## @aidenybai - React Grab: Parallel Coding Agents in Browser
> run parallel coding agents in the browser
>
> Introducing React Grab: https://x.com/aidenybai/status/1996625600073908313/video/1

- **Tweet:** https://x.com/aidenybai/status/1996625600073908313
- **Link:** https://x.com/aidenybai/status/1996625600073908313/video/1
- **What:** Introduction to React Grab, a tool that enables running multiple coding agents in parallel within the browser, expanding the possibilities for collaborative AI development workflows.

---


## @AnthropicAI - Anthropic Interviewer Tool Launch
> We're launching Anthropic Interviewer, a new tool to help us understand people's perspectives on AI.
>
> It's now available at https://claude.ai/interviewer for a week-long pilot.

- **Tweet:** https://x.com/AnthropicAI/status/1996627123021426919
- **Link:** https://claude.ai/interviewer
- **What:** Anthropic launches a new interview tool to gather user perspectives on AI systems, available for a limited pilot period.

---


## @Coach_Yac - Rise of the 49ers Documentary Series
> The players. The coach. The city. The team that changed football forever
>
> #RiseOfThe49ers, a limited series event February 1 and February 2 on AMC and AMC+
>
> Here's the official trailer

- **Tweet:** https://x.com/Coach_Yac/status/1996703037490937864
- **Link:** https://x.com/Coach_Yac/status/1996703037490937864/video/1
- **What:** AMC and AMC+ announce a limited documentary series about the 49ers franchise, premiering February 1-2 with an official trailer.

---


## @fvguima - Premium Paper Towel Recommendation
> My biggest splurge is spending US$600 or so a year on Kimberly-Clark Professional Kleenex Supreme multi-fold towels (S-6868 on ULINE). Have used them for everything from blood (my own) to solvent spills (when I still ran a production wood shop). Cannot remember life before them.
>
> *Quoting @usgraphics:* ULINE Model No. H-1595W and S-6866.
>
> Regardless of the contraption, instead of you spending the energy it takes to tear the roll every single time; we can do it upstream on a massive industrial scale and what you get is a std 9" multifold towel that's precut and folded. Way better than any of this bullshit.

- **Tweet:** https://x.com/fvguima/status/1996743434590142806
- **Quoted:** https://x.com/usgraphics/status/1996742232116977911
- **What:** User enthusiastically recommends industrial-grade pre-folded paper towels, highlighting their durability for various applications from household to workshop use.

---


## @koylanai - Multi-Agent AI Interview System Architecture
> Your best people can't document their expertise because they don't know what they know until they're asked.
>
> We built an interviewer that achieves peer status, so experts reveal the judgment patterns they'd only share with a colleague.
>
> I wrote a blog about how we architected the multi-agent system behind this, how we extract expert thinking, and build digital personas that feel like talking to a peer.

- **Tweet:** https://x.com/koylanai/status/1996757974610559171
- **Link:** https://www.99ravens.agency/resources/blogs/your-experts-wont-train-your-ai-you-have-to-interview-them/
- **What:** Technical deep-dive on designing a multi-agent AI system that interviews experts at a peer level to extract tacit knowledge and build digital personas for knowledge transfer.

---


## @jasonzhou1993 - AI Designer Tool Demo
> No reason to go to Upwork to hire designers anymore
>
> Here I just finished 2 jobs within one min with AI designer

- **Tweet:** https://x.com/jasonzhou1993/status/1996814607512752621
- **Link:** https://x.com/jasonzhou1993/status/1996814607512752621/video/1
- **What:** Demonstration of an AI design tool that completes design work in seconds, suggesting it could replace freelance designer hiring on platforms like Upwork.

---


---



---


# Tuesday, December 2, 2025

## @doodlestein - CASS: Cross-Tool Coding Agent Session Search
> I'm very pleased to introduce my latest tool for both humans and coding agents: the coding agent session search, or "cass" for short.
>
> This tool solves a direct pain point I've been experiencing for months as a heavy user of coding agents, with tons of sessions across many tools (Claude Code, codex, cursor, and now gemini-cli) and projects: I'll know that I talked about something, but be unable to find it or even remember where to try to look for it.
>
> [Full description of tool capabilities, installation, and agent integration guide included]
>
> Making this tool was a real labor of love. Even though I did it all in less than a week, it took a lot of hours and a ridiculous number of tokens and agents. I heavily used all the workflows and tricks I've been posting about recently.

- **Tweet:** https://x.com/doodlestein/status/1995863013987868954
- **Link:** https://github.com/Dicklesworthstone/coding_agent_session_search/blob/main/README.md
- **What:** High-performance Rust tool that enables unified search across coding agent session histories (Claude Code, Cursor, Codex, Gemini, etc.). Includes a robot mode specifically designed for agents to access their own history and peer agent conversations without configuration overhead.

---


## @Altimor - Civilization vs. Violence First Principles
> This was one of my top philosophical realizations this year and biggest break with libertarianism: the realization that the laws of civilization aren't first principles; that the only first principles are that of violence (which are straightforwardly derived from the laws of physics); and that "you can't let your ideals for what ought to happen inside a civilization come before what it takes to have a civilization in the first place" (grateful to @Devon_Eriksen_ for sparking the insight).
>
> *Quoting @Will_Tanner_1:* "Your artificial meritocracy of Excel spreadsheets is propped up by millions of Americans with guns protecting you from the natural meritocracy of extreme violence" might be one of the best tweets ever

- **Tweet:** https://x.com/Altimor/status/1995893516162257284
- **Quoted:** https://x.com/Will_Tanner_1/status/1995657978071142684
- **What:** A philosophical reflection on how civilization's laws are not first principles but rest on the fundamental principle of violence, challenging libertarian ideals about the primacy of abstract rules over the prerequisites for civilization itself.

---


## @hsu_steve - AI-Assisted Quantum Field Theory Research
> I think I've published the first research article in theoretical physics in which the main idea came from an AI - GPT5 in this case. The physics research paper itself (on QFT and state-dependent quantum mechanics) has been published in Physics Letters B.
>
> I've written an accompanying AI paper describing the Generator - Verifier method I used to obtain useful research results from frontier LLMs. It may be of interest to other physicists and to AI researchers.
>
> From the AI paper:
>
> ... models sometimes make very simple mistakes (e.g. in calculation) and also even make incorrect conceptual leaps that are superficially plausible. The second type of error can lead even expert researchers astray, consuming large amounts of effort to detect and correct. Research with an LLM might be compared to collaboration with a brilliant but unreliable human genius who is capable of deep insights but also of errors both simple and profound.
>
> Fortunately, both types of errors can be strongly suppressed by using structured orchestration of multiple model instances, greatly improving reliability. A Generate - Verify protocol, in which one model produces a step forward and another model instance independently checks it, reduces hallucination errors significantly compared to single-pass generation. ...
>
> The physics paper (abstract below) derives new operator integrability conditions required for foliation independence (necessary for integrability of quantum field theory; cf Tomonaga-Schwinger) that are very difficult to satisfy in any modifcation of quantum mechanics that is "state dependent" - i.e., deviates from linear Schrodinger evolution.
>
> Whether quantum evolution is EXACTLY linear is one of the most fundamental questions in all of science. It has implications for quantum computing and quantum foundations - i.e., whether we live in an Everettian multiverse!

- **Tweet:** https://x.com/hsu_steve/status/1996034522308026435
- **What:** First theoretical physics research article where the main contribution originated from GPT-5, published in Physics Letters B. Describes the Generator-Verifier orchestration method for reliably using frontier LLMs in physics research while mitigating hallucination and error risks.

---


---



---


# Monday, December 1, 2025

## @zekramu - On Becoming Competitive in New Corporate Roles
> *Replying to @zekramu:* sold my soul to big tech, first day back in the corporate grind. read Ludwig's article on this. good read. lots of code reading ahead of me.
>
> https://ludwigabap.com/posts/on-becoming-competitive-when-joining-a-new-company/

- **Tweet:** https://x.com/zekramu/status/1995514062546034971
- **Parent:** https://x.com/zekramu/status/1995514060109173210
- **Link:** https://ludwigabap.com/posts/on-becoming-competitive-when-joining-a-new-company/
- **What:** Ludwig's comprehensive guide on how to rapidly become competitive and gain influence when joining a new company. Covers building relationships, maximizing knowledge acquisition, shipping fast, and navigating social dynamics to establish credibility among engineers and leadership.

---


## @jbhuang0604 - DeepSeek v3.2 Attention Mechanisms Deep Dive
> Wondering how DeepSeek v3.2 rivals SOTA models (e.g., GPT5/Gemini 3 pro) while being ~30x cheaper? 🤔
>
> Let's learn how the base model works!
>
> We'll focus on attention, the need for KV caching, and key ideas for improving attention (MQA/GQA/MLA/DSA).

- **Tweet:** https://x.com/jbhuang0604/status/1995559075900522772
- **Link:** https://www.youtube.com/watch?v=Y-o545eYjXM&feature=youtu.be
- **What:** Technical video explaining DeepSeek v3.2's architecture, particularly its attention mechanisms and efficiency improvements. Covers KV caching optimization and various attention variants (MQA, GQA, MLA, DSA) that enable competitive performance at 30x lower cost.

---


## @MaxNordau - Gaza Ministry of Health Death Count Methodology Analysis
> Holy sh1t.
>
> The Gaza Ministry of Health hasn't reported a single natural death since October 2023.
>
> Every single death since October 2023 has been counted as a war death.
>
> In other words: When the news reports "70,000 people have died in Ghazza since October 7, 2023," they mean 70,000 people have died FOR ANY REASON.
>
> The Gaza death count might as well be completely fabricated.

- **Tweet:** https://x.com/MaxNordau/status/1995645070544961681
- **What:** Analysis questioning the methodology of Gaza Ministry of Health death reporting, claiming all deaths since October 2023 are classified as war-related regardless of actual cause. Raises critical questions about data categorization and death count statistics.

---


---



---


# Sunday, November 30, 2025

## @Real_RobN - Biden-Harris Immigration Scheme Allegations
> CONSPIRACY THEORY NO MORE:
>
> Stephen Miller: "The Democrat Party, via the Biden-Harris Terrorist Administration devised a scheme to import illegal aliens into the country by the millions — granting them 'parole,' which gives them work permits, which gives them Social Security numbers, which gives them access to the voting booth — and finally hooking them on welfare like Hunter Biden hooked on drugs, all with the sole purpose of participating in U.S. elections and ultimately overthrowing the Constitutional Republic of the United States."
>
> The whole f**king is seditious,

- **Tweet:** https://x.com/Real_RobN/status/1995220965874434546
- **What:** Political commentary on immigration policy with strong allegations about alleged government intentions, attributed to Stephen Miller.

---


## @ElijahKurien - Best Software Engineering Blogs Collection
> Probably one of the best collection of blogs I've found for software engineering https://t.co/sMtNQbeYEg https://t.co/BCebqUAJSQ

- **Tweet:** https://x.com/ElijahKurien/status/1995269089472991273
- **Link:** https://www.seangoedecke.com/popular/
- **What:** Recommendation of a curated collection of software engineering blogs, suggesting high quality technical content.

---


## @badlogicgames - Writing Good CLAUDE.md and AGENTS.md Guides
> Recommended reading by @dexhorthy
>
> https://t.co/ODo7VGr1MQ
>
> Applies to https://t.co/hvtrEjYOAp just as well. Progressive disclosure in https://t.co/hvtrEjYOAp is great for big mono-repos. Here's my pi-mono https://t.co/hvtrEjYOAp. It's actually a little text adventure :)

- **Tweet:** https://x.com/badlogicgames/status/1995299115438362951
- **Link:** https://www.humanlayer.dev/blog/writing-a-good-claude-md
- **Link:** https://agents.md/
- **What:** Mario Zechner discusses the importance of CLAUDE.md and AGENTS.md files for agent-guided development, with practical insights on progressive disclosure in monorepos.

---


## @buccocapital - 13-Point Company Analysis Framework
> I've found this Deep Research prompt to be a decent way to get up to speed on any company.
>
> Very little focused on valuation, more of a holistic overview
>
> I can't for the life of me remember where I found the original seven-point framework/template but I fleshed it out to 13 to hit the areas I felt were important. If anyone recognizes it, please link/tag the creator
> —————
>
> [Detailed 13-point framework for analyzing companies covering: what they sell, revenue models, revenue quality, cost structure, capital intensity, growth drivers, competitive edge, industry position, unit economics, capital allocation, risks, valuation, and catalysts]

- **Tweet:** https://x.com/buccocapital/status/1995310794339176558
- **What:** Comprehensive 13-point framework for fundamental company analysis, designed to assess business quality, economic moat, and valuation attractiveness without heavy focus on valuation multiples.

---


## @tobi - LLM-Driven Language Cross-Compilation with Agent Specs
> Fun weekend project:
>
> I ported try from Ruby to C as a challenge to agentic workflows.
>
> Steps:
> 1. Extract a directory of spec files for all features of try
> 2. Create automated tests for each spec, executing against the Ruby reference implementation
> 3. Teach the agent to refer to the written specs when a test fails
> 4. Set up an empty directory with basic C libraries (zstr.h, zvec.h- thanks @zuhaitz_dev)
> 5. Instruct Claude to write the C code using those libraries and not stop until all specs pass
>
> Took a bit of fine-tuning, but now I have matching Ruby and C versions. I can add features to both just by updating the spec. It also successfully generated experimental Go and Zig versions.
>
> Published the C version with proper releases: https://github.com/tobi/try-cli
>
> Also packaged it in AUR. Arch users can just run `yay -S try-cli`
>
> This feels like a big part of the future: write once in a high-level language like Ruby, then LLM-compile to any low-level target. Developing high-quality specs like these is totally tractable for agents.
>
> Full specs: https://github.com/tobi/try/tree/main/spec

- **Tweet:** https://x.com/tobi/status/1995316357060063684
- **Link:** https://github.com/tobi/try-cli
- **What:** Demonstrates using Claude agents with comprehensive spec files to automatically port Ruby code to C, Go, and Zig. Shows a practical approach to LLM-based code generation where clear specifications enable reliable multi-language targeting.

---


---



---


# Saturday, November 29, 2025

## @thebeautyofsaas - Designer Suit Shopping Strategy
> What no one tells you is that you can get a 10/10 quality suit (Canali, Loro, Zegna) with a bit of maneuvering and effort for 20-30% of the original price
>
> *Quoting @arlinmoore_:* Owning a $12,000 tailored prada suit will change your life forever. Better investment than any watch.

- **Tweet:** https://x.com/thebeautyofsaas/status/1994794721089393144
- **Quoted:** https://x.com/arlinmoore_/status/1993838585913778283
- **What:** A practical counterpoint to luxury suit investments, showing how to acquire high-quality designer suits at significant discounts through strategic shopping.

---


## @sovereignbrah - Immigration Policy Commentary
> There are millions of people in our country like this. They all need to be deported.

- **Tweet:** https://x.com/sovereignbrah/status/1994852600181846025
- **What:** Political commentary on immigration policy and deportation.

---


## @joelhooks - Claude Code Quality Prompt Engineering
> i tell claude that @mattpocockuk will be reviewing this code so stop with the hack lazy TS bullshit and it literally works lmao

- **Tweet:** https://x.com/joelhooks/status/1994853555807850869
- **What:** A humorous observation about using social pressure and code quality standards as a prompt engineering technique to elicit better TypeScript code from Claude AI.

---


## @kenchangh - X Article Shared
> https://t.co/fgb0IxMWe7

- **Tweet:** https://x.com/kenchangh/status/1994854381267947640
- **Link:** https://x.com/i/article/1968433033637494784
- **What:** A brief share of an X article with minimal context, posted on Saturday evening.

---


---



---


# Friday, November 28, 2025

## @DevilsLA23 - Athletic trainer negligence during player injury
> @mistiiprod Am I tripping or was he literally never attended to by an athletic trainer during this whole incident? This vid pissed me off so much man wtf

- **Tweet:** https://x.com/DevilsLA23/status/1994355149645762959
- **Parent:** https://x.com/mistiiprod/status/1994236185468620898
- **What:** Devs questions why an injured player who took an elbow to the head was left unattended by medical staff during a basketball game, expressing frustration at the apparent lack of care.

---


## @morphllm - WarpGrep: Context Retrieval for Coding Agents
> Introducing WarpGrep, a fast context subagent that improves coding agent performance.
>
> WarpGrep speeds up coding tasks 40% and reduces context rot by 70% on long horizon tasks by treating context retrieval as its own RL trained system.
>
> Inspired by Cognition's SWE-Grep - we're opening access to Claude Code, Codex, OpenCode or any coding agent via MCP (or through our SDK)

- **Tweet:** https://x.com/morphllm/status/1994484969050444103
- **What:** WarpGrep is a specialized context retrieval subagent that significantly improves coding task performance by reducing context drift and accelerating task completion through reinforcement learning.

---


## @buccocapital - Meta's AI-Powered Ad Creation TAM Expansion
> Probably the most important part of the META call
>
> "Advertisers are increasingly going to be able to give us a business objective and a credit card and the Al system [will] basically figure out everything else that's necessary."
>
> Everyone's hunting for the direct beneficiaries of AI, but selling off the one right in front of their face
>
> Massive TAM expansion going on for META. How many people weren't advertising beforehand because of all the work/expertise/money required to build the creative. The less this is a constraint, the greater the TAM

- **Tweet:** https://x.com/buccocapital/status/1994513889619578949
- **What:** Meta's AI ad creation system dramatically expands the total addressable market for advertising by eliminating creative development friction, enabling businesses that previously lacked advertising expertise or resources to participate.

---


---



---


# Thursday, November 27, 2025

## @mattshumer_ - AI Model Stack Comparison After GPT-5 Release
> My Model Stack After the Wildest 8 Days in AI: Opus 4.5 for most daily code tasks (fast and reliable but measures once cuts twice). Codex-Max for larger code tasks where I don't prescribe the solution (measures twice cuts once). GPT-5.1 Pro for deep planning and high-stakes work where accuracy is critical (gets it right first time but slow). Gemini 3 Pro for writing, reasoning, and UI design (best at polished frontends, less reliable on general code).

- **Tweet:** https://x.com/mattshumer_/status/1994113631680950579
- **What:** Comparative analysis of different AI models for various coding tasks following the recent release of GPT-5.1 Pro, establishing clear use case guidelines based on speed, reliability, and specialization.

---


## @YossiBenYakar - Religious justification for child abuse
> This is a Muslim cleric in the United States. Listen carefully to what he says:
>
> "Having sex with a nine-year-old girl, if she can get pregnant, is not considered sexual harassment and is permissible in Islam."
>
> Read that again.
>
> This isn't some fringe outlier. This is a religious justification for pedophilia, preached openly in America.
>
> How is this even allowed on U.S. soil?
> How is this not the national conversation right now?
>
> Share this, people need to hear the truth.

- **Tweet:** https://x.com/YossiBenYakar/status/1994130523736711547
- **Link:** https://x.com/Salwan_Momika1/status/1868342722379272363/video/1
- **What:** Yossi shares a disturbing clip of a Muslim cleric in the US openly claiming that sexual intercourse with prepubescent girls is permissible in Islam, questioning how such teachings are allowed in the country.

---


## @badlogicgames - Passion project in reverse engineering
> The things we do out of love for reverse engineering. https://t.co/kV6RmfdqRm

- **Tweet:** https://x.com/badlogicgames/status/1994138262802477299
- **Link:** https://x.com/badlogicgames/status/1994138262802477299/photo/1
- **What:** Mario Zechner shares a humorous reflection on the lengths developers go to for the sake of reverse engineering projects.

---


## @JackEllis - Balanced perspective on AI capabilities
> This is the most compelling take I've heard on AI. It's from a top software engineer, Adam Wathan, not a grandstanding 17 year old with their big lies. We have huge challenges that AI can't solve, but also a bunch of stuff which it can code faster than me.
> https://t.co/aNWjNMOLZl

- **Tweet:** https://x.com/JackEllis/status/1994141462653751755
- **Link:** https://adams-morning-walk.transistor.fm/episodes/what-should-we-build-with-ai
- **What:** Jack Ellis recommends Adam Wathan's thoughtful podcast episode about realistic AI applications, balancing the hype with practical use cases in software development.

---


## @robbystarbuck - Immigration and national security concerns
> "Today's the day, you f*cking dumb*ss White people" is what he said right before shooting at the police. Importing people who hate your citizens is treason and should be treated as such. Just like the guy who shot the National Guard this week, this man never should've been here.
>
> *Quoting @ProjectConstitu:* 🚨 ALERT: Afghan National Involved in Fairfax Police Shooting Linked to Recent DC Incident Involving National Guard Members
>
> Yesterday, November 26, two National Guard members—Pfc. Andrew Wolfe, 24, and Spc. Sarah Beckstrom, 20—were critically injured in a shooting near the White House in Washington, DC. The suspect, Rahmanullah Lakanwal, an Afghan national who entered the U.S. in 2021, reportedly drove from across the country before the incident. Both service members, who had just been sworn in less than 24 hours prior as part of enhanced security measures under President Trump, are receiving medical treatment.
>
> Looking back to April 23 in Fairfax, VA: A routine traffic stop escalated when Jamal Wali, 36, another Afghan national, expressed frustration and mentioned the Taliban before firing at officers. One bullet injured two officers in their arms, but they were treated and released. Wali was fatally shot in the exchange. Body camera footage captured the event, showing his anger toward the U.S.
>
> These incidents raise questions about vetting processes. Both individuals entered the U.S. under programs from the Obama and Biden administrations—Wali in 2014 as a translator, and Lakanwal through asylum pathways amid the Afghanistan withdrawal. Concerns have been voiced about border security and immigration policies that may have allowed unvetted entries.
>
> President Trump is addressing this by deploying 500 additional Guardsmen, but many are calling for stronger measures to secure the border. Share if you support accountability and safer policies!

- **Tweet:** https://x.com/robbystarbuck/status/1994243668039880756
- **Quoted:** https://x.com/ProjectConstitu/status/1994156290378027102
- **What:** Robby Starbuck criticizes immigration policies following violent incidents involving Afghan nationals, linking recent shootings of National Guard members and police to broader border security concerns.

---


---



---


# Wednesday, November 26, 2025

## @badlogicgames - Agent in Messaging App as Computer God Mode
> Seriously, a an agent with a computer in your messaging app, including group chat, is basically computer god mode. It can just do things and add new capabilities to itself ad-hoc. https://t.co/HR1iiQ1HVi

- **Tweet:** https://x.com/badlogicgames/status/1993614141094076744
- **Link:** https://x.com/badlogicgames/status/1993614141094076744/photo/1
- **What:** Highlights the transformative power of having a coding agent with full system access embedded in messaging apps, enabling ad-hoc capability expansion and autonomous action execution.

---


## @ambricken - Anthropic Applied AI Agent Harness Blog Post
> One of the coolest Applied AI experiments ran internally now shared with the world.
>
> It demonstrates the true power of a harness and filesystem, combined with the intelligence of Claude. This blogpost is so good it almost feels like we're giving away IP 😂

- **Tweet:** https://x.com/ambricken/status/1993756993337627034
- **Quoted:** https://x.com/AnthropicAI/status/1993733817849303409
- **What:** Commentary on Anthropic's engineering blog post about long-running AI agents using human-inspired harness designs, covering challenges in cross-context-window agent operation and filesystem integration.

---


## @sprice - Compound Engineering Plugin Excellence
> *Quoting @kieranklaassen:* Opus 4.5 is insane. Just shipped v2 of my compounding engineering plugin—watch the video for my full thoughts on the model.
>
> I thought I had a good /plan custom Claude Code command.
>
> I'm at a loss for words for how good @kieranklaassen's Compound Engineering plugin is.
>
> Stop what you're doing.
>
> Install this.

- **Tweet:** https://x.com/sprice/status/1993768546191724609
- **Quoted:** https://x.com/kieranklaassen/status/1993054059520217395
- **What:** Enthusiastic endorsement of Kieran Klaassen's Compound Engineering plugin v2, highlighting its exceptional quality and utility for Claude Code workflows.

---


## @QwQiao - Investment Portfolio Update with Amazon
> *Quoting own analysis:* Current stonk holdings: goog, eli lilly, baba, tencent, and previously xiaomi.
>
> Small update: still hold first 4 of the 5, but added amzn and removed xiaomi. Amazon story is simple: their retail margin is going to substantially increase thanks to industrial robots + AWS benefits from a strong AI compute tailwind. Xiaomi: I became enamored with EVs and self-driving but the industry is cutthroat and I don't believe it's a Munger-style "wonderful business" I can hold for 10 years.

- **Tweet:** https://x.com/QwQiao/status/1993779938852249964
- **Quoted:** https://x.com/QwQiao/status/1940725404945277336
- **What:** Portfolio rebalancing decision replacing Xiaomi with Amazon due to industrial robotics margin improvement and AWS AI tailwinds, while maintaining core positions in tech and biotech.

---


## @EricBuess - Claude Opus Setup with Frontend Design Skill
> *Quoting @trq212:* Opus 4.5 is our best model yet for design & vision.
>
> Claude update: /model -> opus, /plugin marketplace add anthropics/claude-code, /plugin install frontend-design@claude-code-plugins, shift+tab until you see plan mode, "Use the frontend-design skill to [describe what you want to build]"

- **Tweet:** https://x.com/EricBuess/status/1993803743733928214
- **Quoted:** https://x.com/trq212/status/1993786550656897491
- **What:** Quick reference guide for setting up Claude Opus with the frontend-design plugin in Claude Code, highlighting the plan mode integration for UI building workflows.

---


## @doodlestein - Beads Viewer: Terminal UI for Agent Task Management
> I'm a huge fan of Steve Yegge's great beads project, which is a task management system for use by coding agents. I use beads hundreds of times daily across projects. I wished I had a better way to browse beads, so I created beads_viewer (bv) this morning. It's a performant Golang tool with graph theoretic calculations to extract insights. Press F1 for commands, try "i" for insights, "g" for graph, "b" for kanban board. Includes AI-friendly robot flags like --robot-insights, --robot-plan, --robot-priority for agents to use without hand-rolling graph logic.

- **Tweet:** https://x.com/doodlestein/status/1993911933272019175
- **Link:** https://github.com/Dicklesworthstone/beads_viewer
- **What:** Announcement of beads_viewer, a performant terminal UI tool for managing and visualizing task dependency graphs created with Steve Yegge's beads system, featuring AI-optimized robot commands.

---


---



---


# Tuesday, November 25, 2025

## @iamsahaj_xyz - Agent-Assisted Development Workflow
> recent workflow I've started to adopt:

step 1
- ask agent to implement something.
- test if it works

loop this until you get a working version

step 2
in a new chat, in plan mode, ask the agent to check the current diff with main branch and refactor the changes
- as if it was being written from scratch,
- goal is to minimize tech debt,
- don't aim for the shortest way possible

step 3
iterate on plan and let it rip when you're happy.

tbf this is nothing new, this is also how most people work regardless of the agent being there, just observed myself doing this more often recently

- **Tweet:** https://x.com/iamsahaj_xyz/status/1993315270648307941
- **What:** A three-step development workflow for agent-assisted coding: implement and test iteratively, then refactor with focus on tech debt minimization, finally execute refined plan.

---


## @alexalbert__ - Claude Opus 4.5 Prompting Guide
> We put together a prompting guide for Claude Opus 4.5 based on extensive internal testing by our research and applied AI teams.

Here's what we've learned so far about getting the best results:

- **Tweet:** https://x.com/alexalbert__/status/1993365963706913257
- **What:** Announcement of an official prompting guide for Claude Opus 4.5 with best practices learned from extensive internal testing by Anthropic teams.

---


## @nityeshaga - Claude Opus 4.5 Prompting Guide
> *Quoting @alexalbert__:* We put together a prompting guide for Claude Opus 4.5 based on extensive internal testing by our research and applied AI teams.

Here's what we've learned so far about getting the best results:

- **Tweet:** https://x.com/nityeshaga/status/1993382486567756042
- **Link:** https://github.com/anthropics/claude-code/blob/main/plugins/claude-opus-4-5-migration/skills/claude-opus-4-5-migration/references/prompt-snippets.md
- **Quoted:** https://x.com/alexalbert__/status/1993365963706913257
- **What:** Anthropic's internal testing team compiled a comprehensive prompting guide for Claude Opus 4.5. Key optimization snippets available in their official repository.

---


## @ryancarson - Beads Task Management Tool
> Beads by @Steve_Yegge is SO good.

Perfect when you're in the flow and you notice another bug or a task you need to tackle another time. I just type

`bd: add task to cleanup design of /efile-submission. not top priority`

No need to break out Linear or do something complex.

Now I can keep going and come back easily to the task with just this ...

`bd list -s open`

- **Tweet:** https://x.com/ryancarson/status/1993382714599162206
- **Link:** https://github.com/steveyegge/beads
- **What:** Beads is a lightweight task management tool by Steve Yegge that lets developers quickly capture tasks without context switching. Perfect for noting bugs and follow-up work while in flow state.

---


## @rseroter - Spotify's Background Coding Agents Context Engineering
> The @SpotifyEng team built background coding agents that can edit code, run tests, and such. But how do they give them instructions?

Here's a look at what they do for context engineering ...

- **Tweet:** https://x.com/rseroter/status/1993428229009588321
- **Link:** https://engineering.atspotify.com/2025/11/context-engineering-background-coding-agents-part-2
- **What:** Spotify engineering shares how they use context engineering to instruct background coding agents. The agents can edit code, run builds and tests, and open PRs. Understanding how to give agents proper instructions is essential for reliable results.

---


## @thebirdabides - Sohu AI Chip Performance vs Nvidia
> *Replying to @bubbleboi:* If you actually understand how computers work, you will make a ton of money in this market .

Nobody in Silicon Valley or Wall Street knows how chips work anymore. Google is taking half of Nvidia's market share and market cap. But the real winner won't be Google it's going to be a startup that makes a better TPU and sells it to everyone..

- **Tweet:** https://x.com/thebirdabides/status/1993431760743670208
- **Parent:** https://x.com/bubbleboi/status/1993431039272767685
- **Link:** https://www.tomshardware.com/tech-industry/artificial-intelligence/sohu-ai-chip-claimed-to-run-models-20x-faster-and-cheaper-than-nvidia-h100-gpus
- **What:** Tom's Hardware covers Etched's Sohu AI chip, claiming 20x faster performance and lower cost than Nvidia H100 GPUs. Relevant to discussion of specialized AI hardware startups disrupting the market.

---


## @notnotstorm - Running 24x Claude Code Instances Workflow
> when running 24x claude code instances makes sense:

1. an initial agent scanned my repo looking for general improvements. it flagged 20 things. I liked 12 of them and told it to create a github issue for each

2. I opened up 12 tmux panes and ran `/fix <issue_number>` in each one. this is a slash command that fixes a gh issue in a new worktree and submits a pr

3. I split each of those panes in half and ran `/review <pr_number>` on each of the 12 prs

4. I ran `/respond` in each of the 12 original panes, to respond to the reviews and update the pr's with any necessary fixes

5. I ran `/summarize_prs` to figure out the best merge order and flag PR's that might have bad concerns or tradeoffs

next step is decide which PR's I want to merge and merge them

it's still a very manual process but every week I feel like I'm getting a lot faster

- **Tweet:** https://x.com/notnotstorm/status/1993443281846649209
- **What:** Developer demonstrates parallelized workflow using 24 Claude Code instances with tmux panes for issue scanning, fixing, reviewing, and PR management. Shows emerging patterns for scaling AI-assisted development across multiple concurrent tasks.

---


## @pdrmnvd - Using AskUserQuestion in Claude Commands
> Do you love Claude's plan-mode question asker and wish you could bring it with you everywhere?
>
> Add `AskUserQuestion` to allowed-tools in a .claude/command then explicitly tell Claude to use it.
>
> > Use the AskUserQuestion tool to ask the user...
>
> Here's me using it for a PR review slash command.

- **Tweet:** https://x.com/pdrmnvd/status/1993451295152484409
- **What:** Demonstrates how to use the AskUserQuestion tool in Claude Code commands by configuring it in .claude/command files, enabling interactive question-asking in custom slash commands like PR reviews.

---


## @0xblacklight - Writing a Good CLAUDE.md
> Full post here, summary below:
> https://t.co/Mo1aSrKXx9

- **Tweet:** https://x.com/0xblacklight/status/1993463350395912233
- **Link:** https://www.humanlayer.dev/blog/writing-a-good-claude-md
- **Parent:** https://x.com/0xblacklight/status/1993463348155859360
- **What:** Article explaining best practices for writing CLAUDE.md configuration files, which are critical for onboarding LLM agents to codebases since LLMs are stateless and must be told codebase context on each session.

---


## @badlogicgames - Slack Bot Coding Agent with Docker Isolation
> Ok, I think this is going somewhere! Built a Slack bot that's basically a coding agent which has:
>
> 1. Access to the channel history (jsonl file it can grep)
> 2. File read/write/edit tools
> 3. Bash
>
> Bash tool operates inside a Docker container, into which channel history JSONL and channel attachments are mounted.
>
> Bot can do whatever it wants inside the Docker container. Install tools like GH CLI, Node, Python, etc, clone repositories, compile stuff, fetch stuff from the web.
>
> Bot is invoked by mentioning it in the channel, which will trigger an agentic run. Bot posts a message to the slack channel, which gets updated with new outputs from the agent run. For debugging, a thread is attached to the message, which shows all tool invocations chronologically.
>
> And it has a tool that lets it attach one or more files from the Docker container to its Slack message. So it can create stuff for me in the container, and ship the result as a plain old Slack attachment. Very nice!
>
> This is super nice to work with. And through the Docker isolation, I might actually not shoot myself in the foot.

- **Tweet:** https://x.com/badlogicgames/status/1993479329586499890
- **What:** Building a Slack-integrated coding agent that runs inside Docker containers with file/edit tools and bash access, allowing the bot to install tools, clone repos, and attach results directly to Slack messages with full isolation.

---


---



---


# Monday, November 24, 2025

## @MatthewBerman - Opus 4.5 Outperforms All Humans on Anthropic Interview Exam
> Absolutely insane stat.
>
> Opus 4.5 outperformed EVERY SINGLE HUMAN CANDIDATE EVER in Anthropic's notoriously difficult take-home exam for prospective performance engineering candidates. https://t.co/RJxlgwUlCy

- **Tweet:** https://x.com/MatthewBerman/status/1993038043876671863
- **What:** Remarkable benchmark showing that Claude Opus 4.5 has outperformed every single human candidate in Anthropic's challenging take-home exam for performance engineering positions.

---


## @simonw - Opus 4.5 Token Efficiency Economics
> *Quoting @alexalbert__:* It's also dramatically more efficient. On SWE-bench Verified at medium effort, Opus 4.5 beats Sonnet 4.5 while using 76% fewer output tokens. The new effort parameter lets you trade off intelligence for cost/latency with a single dial.

This is notable: Opus 4.5 is ~60% more expensive than Sonnet ($25/million output compared to $15/million) but if it can use 76% fewer output reasoning tokens for the same complex task it may end up cheaper!

- **Tweet:** https://x.com/simonw/status/1993070568435073135
- **Quoted:** https://x.com/alexalbert__/status/1993030687881080944
- **What:** Analysis of Opus 4.5's cost-effectiveness compared to Sonnet despite higher per-token pricing, thanks to dramatically reduced output token usage.

---


## @pvncher - OpenAI Reasoning Context Pollution
> *Replying to @sacino:* why do you think gpt-5.1-low is second?

@bitofseo I wrote about this elsewhere but I firmly believe it's because OpenAI reasoning traces pollute the context window and, gpt models are more sensitive to noise in the context window than Claude models.

- **Tweet:** https://x.com/pvncher/status/1993113207892758580
- **Parent:** https://x.com/sacino/status/1993112377261539843
- **What:** Explanation for why GPT-5.1-low underperforms: OpenAI's reasoning traces pollute the context window, and GPT models are more sensitive to context noise than Claude.

---


## @pvncher - Reasoning Trade-offs for Coding Tasks
> *Replying to @joelwashington:* @pvncher @bitofseo Cool finding, surprising and very interesting. Why do you think other evals are generally showing xhigh better, is there something about yours that are testing long context in a way others aren't? I've generally been defaulting to xhigh b/c it's fast, but I'm now going to try low

Actually surprisingly, codex max xhigh decently on repo bench, but not as good as vanilla 5.1 low. It's not on the leaderboard, but it's in the explorer. I would say, for coding intelligence, more reasoning is better, but that's also why I split planning / discovery, from execution. Execution needs less reasoning

- **Tweet:** https://x.com/pvncher/status/1993124628059799604
- **Parent:** https://x.com/joelwashington/status/1993123487687622774
- **What:** Discussion of reasoning levels for coding tasks - proposing a strategy to split planning/discovery (needs more reasoning) from execution (needs less reasoning).

---


---


# Sunday, November 23, 2025

## @DeanTTraining - Oreo Blizzard High Protein Ice Cream Recipe
> Probably just gonna keep posting this every week until everyone on the internet knows about it…
>
> (If you don't already have one, put the Ninja Creami Deluxe on your Christmas list)
>
> Oreo Blizzard High Protein Ice Cream Recipe
>
> - 240ml Fairlife Skim Milk
> - 240ml Almond Milk Unsweetened Vanilla
> - 51g True Nutrition Cookies N Cream Egg White Protein
> - 30g Oreos Cookies N Creme Instant Pudding Mix
> - 4 Oreo Thins
> - 2g Xanthan Gum
>
> 540 calories / 50g protein

**Quote Context:**
> @DeanTTraining Where's the recipe?
> — Luke (@Lukebraus) https://x.com/Lukebraus/status/1992535378730025230

- **Tweet:** https://x.com/DeanTTraining/status/1992683209834848650
- **What:** High-protein ice cream recipe for an Oreo Blizzard made with the Ninja Creami Deluxe, containing 540 calories and 50g of protein.

---


---


# Saturday, November 22, 2025

## @kieranklaassen - New Sub-Agent for Compounding Engineering
> This is my new favorite sub-agent. I love it. Sharing soon in the Compounding Engineering plugin.
>
> https://t.co/6LI5u1ZHTh https://t.co/gnSqSbAXdP

- **Tweet:** https://x.com/kieranklaassen/status/1992349643607617924
- **Link:** https://github.com/EveryInc/compound-engineering-plugin
- **What:** Announcement of a new sub-agent tool that will be shared in the Compounding Engineering plugin, which the author describes as their new favorite.


---

## @XJosh - Understanding Izzat: India's Cultural Honor System
> Kiwi Farms user breaks down 'Izzat', the Indian subcontinent's cultural honor system. It effectively explains every single trope about Indian behavior: they all participate in an invisible clout-chasing game that involves screwing over everyone as much as possible. Worth the read https://t.co/Ob4mkqt7H6

- **Tweet:** https://x.com/XJosh/status/1992348701793349827
- **Link:** https://x.com/XJosh/status/1992348701793349827/photo/1
- **What:** Analysis of 'Izzat', the Indian cultural honor system, explaining it as a clout-chasing game that drives interpersonal behavior in the Indian subcontinent.


---

## @alexhillman - Always Do (11 Imperatives)
> Always Keep Humans at the Center - use AI to remove drudgery and free up time for real, authentic relationships

- **Tweet:** https://x.com/alexhillman/status/1992252350812270856
- **What:** Personal reflection on core imperatives with emphasis on keeping humans central to all technology decisions.


---


---


# Friday, November 21, 2025

## @AlphaNews - Derek Chauvin Petition Alleges Prosecutorial Misconduct
> BREAKING: Derek Chauvin's attorney files new petition, says prosecution 'can only run from the truth for so long'
>
> In a bombshell petition—alleging prosecutorial misconduct—more than 50 former and current officers have provided sworn declarations stating that the technique used by Derek Chauvin and the other Minneapolis police officers involved in the arrest of George Floyd was part of MPD training.

- **Tweet:** https://x.com/AlphaNews/status/1992031829843431689
- **What:** Breaking news on Derek Chauvin's attorney filing a petition alleging prosecutorial misconduct in the George Floyd case, with 50+ officers providing sworn declarations that the technique used was part of standard MPD training.


---

## @mitsuhiko - Agent Design Challenges and Insights
> Well, @badlogicgames reminded of the value of sharing, so here's the update: agent building is hard. Agent SDKs are tricky, caching is a per-model art, reinforcement can help, isolation saves your sanity, filesystems! New models are "it depends." https://t.co/6RiHJysI20

- **Tweet:** https://x.com/mitsuhiko/status/1992000898147766638
- **Link:** https://lucumr.pocoo.org/2025/11/21/agents-are-hard/
- **What:** Armin Ronacher shares key learnings about agent design complexity, covering SDK abstractions, caching strategies, reinforcement learning, isolation patterns, and the model-dependent nature of agentic AI.


---

## @amyforsandiego - Judge Questions Student Privacy vs Parental Rights
> The judge said to @GavinNewsom lawyers:

"So the state, with a straight face, is saying that a KINDERGARTNER who says that he or she wants to transition has a right to privacy that supersedes ... the parents' 14th Amendment, long-standing - long, long, long, long-standing - right to the care, custody and control of their children" Thank you Judge!

**Quoted Tweet:** @sdut - Court mulls San Diego County district's debate over whether schools should tell parents if kids may be transgender https://t.co/fesAccHc7M

- **Tweet:** https://x.com/amyforsandiego/status/1991913114317844499
- **What:** Amy Reichert shares a judge's statement questioning the state's position that a kindergartner's privacy right regarding transition overrides parental rights, in the context of a San Diego school district case.

---


---


# Thursday, November 20, 2025

## @tnm - MIT-Licensed Code Search and CLI Tool
> I don't know wtf this is but if you want MIT-licensed code search + CLI that you can use for yourself and for your devtools, check out https://t.co/9mMKJ43KAt

**Quoted Tweet:** @aaxsh18 - we just made Claude Code
- use 53% fewer tokens
- respond 48% faster
- give 3.2x better responses

just by giving it a better grep https://t.co/GUf1dS9e8B

- **Tweet:** https://x.com/tnm/status/1991751474372833728
- **Link:** https://github.com/cased/kit
- **What:** Ted Nyman shares the Kit tool, an MIT-licensed code search and CLI tool that can be used as a standalone utility or integrated into developer tools. He's quoting Aamir Shakir's post about Claude Code improvements.


---

## @aeitroc - Quibbler Hook Recommendation
> @bcardarella Add this hook https://t.co/Q0OIrbbkym

**Parent Tweet:** @bcardarella - I told Claude to one-shot an integration test against a detailed spec I provided. It went silet for about 30 minutes. I asked how it was going twice and it reassured me it was doing work. Then I asked why it was taking so long: https://t.co/1Oc1zbhFcQ

- **Tweet:** https://x.com/aeitroc/status/1991564773323075714
- **Link:** https://github.com/fulcrumresearch/quibbler
- **What:** Bessi recommends using the Quibbler hook to address Brian Cardarella's issue with Claude spending excessive time on integration test generation.

---


---


# Wednesday, November 19, 2025

## @transitive_bs - Feynman Discusses Why Simple Things Are Complex
> @Rainmaker1973 amazing convo from feynman discussing why \"simple\" things like this are so complex under the hood https://t.co/fEv7bgXqeX

**Parent Tweet:** @Rainmaker1973 - New researsh shows ice is slippery because of electrical charges — not pressure and friction.

For almost 200 years, the prevailing explanation for ice's slipperiness was that friction or pressure from a skate, boot, or tire melted a microscopic film of water on the surface, creating a lubricating layer. A new study from Saarland University has overturned that long-standing idea.

Instead, the true cause lies in the electric fields generated by molecular dipoles. When any object contacts ice, the partial charges in its own molecules interact with the highly ordered dipole arrangement of water molecules in the ice crystal. This electrostatic tug-of-war loosens the topmost layer of the ice lattice, transforming it into a thin, disordered, quasi-liquid film—without any need for heat or significant pressure.

Remarkably, this self-lubrication mechanism works even at temperatures approaching absolute zero, where thermal energy is virtually absent and conventional pressure-melting or frictional heating theories completely break down. In those extreme conditions, ice remains slippery simply because its surface molecules are electrically vulnerable.

- **Tweet:** https://x.com/transitive_bs/status/1991360786804122079
- **Link:** https://www.youtube.com/watch?v=Q1lL-hXO27Q
- **What:** Travis Fischer shares a Feynman discussion about the surprising complexity of why ice is slippery, relating to new research about electrical charges and molecular dipoles rather than traditional pressure-melting theories.

---


---


# Tuesday, November 18, 2025

## @blader - Market rotation from NVDA to GOOG on Gemini 3 emergence
> re: gemini 3
>
> for the past 4 years i've had the plurality of our liquid net worth in NVDA
>
> about a month ago i sold it all and rotated into GOOG
>
> take from that what you will

- **Tweet:** https://x.com/blader/status/1990958680456471005
- **What:** Siqi Chen signals confidence in Google by rotating a significant portfolio position from NVIDIA to Google, timed around Gemini 3's emergence as a frontier AI model.


---

## @VictorTaelin - Comprehensive analysis: Gemini 3 capabilities and limitations
> My notes on Gemini 3
>
> # Short Version:
>
> First of all: you've all seen the benchmarks, so I don't think you need me to judge this one. Still, based on my tests, this is as real as it gets, and I want to talk about it. This model outperforms GPT-5 Pro, Gemini 2.5 Deep Think, and everything else, on my hardest problems, by far.
>
> It is the new SOTA at:
> → debugging complex compiler bugs
> → refactoring files without logical mistakes
> → solving difficult λ-calculus problems
> → ASCII art (it is almost decent now!)
> → Competitive Gen 3 OU (won't elaborate 😭)
>
> It is still an LLM, though. It has similar failure modes, and is worse than Sonnet / GPT-5 in some scenarios.
>
> It seems very bad at:
> → inferring intent
> → not going overboard
> → one-shot vibe coding
> → creative writing
> → health questions
>
> Also, I suspect this checkpoint isn't the best Google has.
>
> Now, on to a complete, manually typed Gemini 3 overview.
>
> ---
>
> # Long Version
>
> 1. Vibe Test: λ-Calculus Programming
>
> I like this vibe test because it is cheat proof: as soon as a model solves my hardest problem, I just create a harder one, moving the goalpost a little bit.
>
> Current track record:
> → n-tuple-map: solved by Grok 3 (Feb 2025)
> → n-tuple-fold: solved by GPT-5 (Aug 2025)
> → n-tuple-rotl: solved by Gemini 3 (today!)
>
> Implementing rotl is impressive, because:
> → no other model gets even close to solving it
> → Gemini's solution is 2x simpler than my own's
> → Gemini 3 solved it 5x faster than myself
>
> In fact, its solution is so short, it fits a single line:
>
> λn.λt.λk.(tλx.(nλg.λh.(h(gλq.λr.λs.(q(r s))))λu.λf.(f x)λu.u k))
>
> Pretty, isn't it? This minuscule function is a generic rotator for λ-encoded tuples. For a comparison, every other model creates a 5x larger term... that doesn't work. Nothing else creates anything like that, at all. That answer was a jaw-dropping moment for me.
>
> I'll post a Gist with the prompt, and a runnable solution.
>
> 2. Real-World Debugging
>
> A few weeks ago, I was stuck in a tough HVM4 bug. I posted about it here, lamenting that no AI could solve it. Well, turns out, an AI did solve it. Someone managed to run my prompt on an old checkpoint via LMSys, and it nailed the issue: a stack underflow on a specific optimization. The solution was simple: replace `WNF_SPOS < 0` by `WNF_SPOS < spos`.
>
> This was the first time an AI solved a real problem before I could solve it myself, and that let me move on to the next thing, leading to great progress.
>
> I now tested Gemini 3 on many old debugging prompts, and it solved half of them. Bugs that took me hours are now solved by a computer in a minute!
>
> Now, and sadly: I've sent the stack underflow issue to the Gemini 3 model that launched today, and it failed to spot the culprit. So, either this model is not the smartest variant Google has, or I was really lucky that day. ):
>
> 3. Real-World Coding / Refactoring
>
> This model is great at writing large files with no mistakes.
>
> For example, I've asked some AIs to rewrite HVM4.hs with a few core changes. I then inspected the trickiest functions. As you'd expect, all models failed on important details that lead to serious bugs - except for Gemini 3, which nailed it.
>
> This is particularly encouraging to me, since models struggled with niche restrictions like linearity, making them unusable for core HVM functions. Gemini 3 seems extremely competent at it.
>
> (Code in the image below.)
>
> 4. Problems and Quirks
>
> I've asked Gemini 3 to one shot a web app, and it did poorly. GPT-5.1 (high) gave me complete file, with everything I asked for, zero bugs. Gemini 3 gave me a 3x smaller file, with tons of missing features and many bugs. I couldn't get Gemini 3 to one shot a file nearly as good as the one by GPT-5.1.
>
> I've also sent it my pre-meningitis prompt, and it completely discarded meningitis (💀). Not sure I'd trust it for health issues.
>
> I've asked it to write a story, and it was bad. No excuses.
>
> It will often go overboard and write full files instead of just patching holes.
>
> It seems slower than even GPT-5 (high) on Gemini CLI, although it is much faster when called directly?
>
> Lastly, and funnily, it struggles to produce incorrect code when context calls for it. For example, if your type has a generic "Show" instance, and you ask it to build a custom one, it will often struggle, because that'd technically be an error. It can't grasp that you'd just remove the old one afterwards!
>
> 5. Conclusion
>
> Enough typing, bye

- **Tweet:** https://x.com/VictorTaelin/status/1990844923994886282
- **What:** VictorTaelin provides an in-depth technical analysis of Gemini 3, documenting its strengths in compiler debugging, refactoring, and lambda-calculus programming, while identifying weaknesses in creative tasks and web development.


---

## @beyang - Gemini 3 becomes Amp's default smart agent on launch
> We've been testing Gemini 3 for a few days and this is the first model where we felt compelled to switch Amp's default smart agent on model release day. Congrats to Google on a great new frontier LLM!

**Quote Context:** @thorstenball - Amp's new default model: Gemini 3 Pro

- **Tweet:** https://x.com/beyang/status/1990824222734905502
- **What:** Beyang from Amp reports that Google's Gemini 3 impressed them so much they made it the default smart agent on day one of release, marking a significant frontier achievement.

---


---


# Monday, November 17, 2025

## @mitsuhiko - AI discourse: Why JSON beats TOON for token efficiency
> AI discourse on Twitter is frustrating. Take this tweet with thousands of views. It claims you should  use TOON instead of JSON. But if you actually count tokens, the savings are … barely existing, it's not in the training data, and tabular JSON beats it. https://t.co/tD00NOS0mN https://t.co/vJe4zB407l

**Quote Context:** @DataChaz - Token-Oriented Object Notation (TOON)
> If you're still sending raw JSON into your LLMs, you're burning tokens, latency, and budget!
>
> Try TOON (Token-Oriented Object Notation).
>
> Clear like YAML, compact like CSV:
>
> • 30–60% fewer tokens
> • Up to 50% lower costs
> • Shines for tabular data.
>
> Free and Open source

- **Tweet:** https://x.com/mitsuhiko/status/1990549149629222938
- **What:** Armin Ronacher critiques claims that TOON saves significant tokens compared to JSON, arguing actual token savings are negligible and that tabular JSON is more effective.

---
DATE: Monday, November 17, 2025

---

## @kevinkern - Oracle: AI-powered coding assistant for complex tasks
> Nice addon for codex. Oracle sends your hard tasks to gpt 5 pro.
>
> Tip: You can pair it with codefetch to set up the context first. https://t.co/DhyMZFpL5Y

**Quote Context:** @steipete - Is your agent stuck?
> "consult the oracle🧿 npx -y @ steipete/oracle"
>
> This packs prompt, files & sends it to GPT-5 Pro. Supports both API and browser.

- **Tweet:** https://x.com/kevinkern/status/1990546264996618279
- **What:** Kevin Kern highlights Oracle, a Node.js package that integrates with Codex to delegate hard coding problems to GPT-5 Pro, with optional context setup via codefetch.

---


---


# Sunday, November 16, 2025

## @coderabbitai - Open Source Git Worktree Manager for AI Coding Agents
> We are open-sourcing one of our internal tools!
>
> Introducing our AI-native open-source Git worktree manager CLI that works with all your AI Coding Agents ✌️ (that was a mouth full)
>
> Have fun!

- **Tweet:** https://x.com/coderabbitai/status/1990107743269663026

- **What:** CodeRabbit releases a CLI tool for managing Git worktrees, specifically designed for AI coding agents. Enables efficient isolation of work across multiple worktrees for concurrent agent operations.

---


---


# Saturday, November 15, 2025

## @steipete - Ask the Oracle: Automated Browser Agent with GPT Integration
> "ask the oracle🧿" ... spins up browser fully automated, submits to GPT 5 Pro, sends back text to your agent (works with any agent)

- **Tweet:** https://x.com/steipete/status/1989884121716347292
- **Link:** https://github.com/steipete/oracle

- **What:** Open-source tool that orchestrates browser automation with GPT 5 Pro integration, enabling agents to submit web content to AI models and receive processed results. Works as a generic bridge for any agent framework.


---

## @badlogicgames - Context Limitations: GPT vs Claude on Large Files
> The best part is that it doesn't even truncate to 10kb but 5kb.
>
> That file has 2200 lines, which fit snuggly inside the context. Alas, poor GPT won't see even a 10th of the content.

- **Tweet:** https://x.com/badlogicgames/status/1989863756814336032

- **What:** Discussion about how Claude can fit 2200-line files in context while GPT has severe truncation limits (5kb), highlighting the context window advantage for agents working with large source files.


---

## @badlogicgames - Alternative to MCP: Browser Tools via Bash and Code
> Blog post:
> https://mariozechner.at/posts/2025-11-02-what-if-you-dont-need-mcp/

**Quote context:** "Create a tiny script that can do most of what chrome-devtools mcp can, based on @badlogicgames 's blog post, added to my collection" - @steipete

- **Tweet:** https://x.com/badlogicgames/status/1989785200268923166
- **Link:** https://mariozechner.at/posts/2025-11-02-what-if-you-dont-need-mcp/

- **What:** Blog post arguing that for many browser automation use cases, agents don't need MCP servers—just Bash scripts and code. Demonstrates minimal browser tools (start, navigate, evaluate JavaScript, screenshot) using Puppeteer Core instead of heavyweight MCP implementations.

---


---


# Friday, November 14, 2025

## @QwQiao - Investment Portfolio Strategy: Tech Giants and Long-Term Holdings
> made this list a while ago so just waiting for the right price:
>
> - mag7: greatest businesses in the history of businesses
> - tsmc, asml: ai monopolies
> - axp, v, ma, mco, spgi, race, rms: classic buffett-munger "wonderful businesses"
> - baba, tcehy: chinese bigtech + ai play
> - defi blue chips: revenue meta
> - coin, hood: "banks" for young gen
> - ubtech, xpeng, unitree: robotics
>
> all these i can hold for a 5-10yrs

**Quote context:** "so what's on everyone's bear market shopping list - stocks & crypto allowed" - @blknoiz06

- **Tweet:** https://x.com/QwQiao/status/1989374634005782817

- **What:** Investment thesis covering major tech stocks (Mag 7), semiconductor leaders, Warren Buffett-style quality companies, Chinese tech plays, DeFi protocols, fintech platforms, and robotics companies suitable for 5-10 year holds.

---


---


# Wednesday, November 12, 2025

## @mattpocockuk - Claude Rules Configuration
> My Claude rules file:
>
> https://t.co/04E0xxX88s

- **Tweet:** https://x.com/mattpocockuk/status/1988712350703317200
- **Link:** https://gist.github.com/mattpocock/3fa37286736669878523596f1206ff4a
- **What:** Matt Pocock shares his personal Claude rules configuration file from a GitHub gist for reference and inspiration.


---

## @mikeyk - Claude Frontend Design Skills Plugin
> Our Applied AI team with a great write up on improving Claude's frontend design via Skills. Also with a Claude Code plugin that packages up the skill!
> https://t.co/5gPFn5UwhW

- **Tweet:** https://x.com/mikeyk/status/1988691831836782610
- **Link:** https://www.claude.com/blog/improving-frontend-design-through-skills
- **What:** Mike Krieger highlights a blog post about enhancing frontend design capabilities through Claude Skills, with an accompanying Claude Code plugin.


---

## @trq212 - Deep Research with Claude Agent SDK
> We built a Deep Research demo for the Claude Agent SDK!
>
> It's one our most requested use cases: spawn multiple AI agents to research a topic in parallel, then synthesize their findings into a report.
>
> on how it works: https://t.co/jU2kRc9hIq

- **Tweet:** https://x.com/trq212/status/1988690675542675536
- **What:** Thariq announces a Deep Research demo showcasing parallel agent research capability within the Claude Agent SDK for comprehensive report synthesis.


---

## @joulee - AI Autocomplete Interface Design
> Really slick. I expect to see this autocomplete paradigm everywhere in AI interface design over the coming months.

**Quote Tweet:**
> I'm very excited to announce AI Autocomplete
>
> AI Autocomplete is a breakthrough patented technology that supercharges natural language input = Unlocking 10x faster search and commerce, advertising, and powerful augmented reality. Available for use as an SDK.
>
> This solves a fundamental problem of today's chat interfaces – They are good at single step request, but any multi-step action (like booking a flight or purchasing goods) quickly becomes a back and forth 'game of 10 questions'.
>
> While working on our own assistant, we realized the core driver of this problem is a human one: People don't know everything they need to say upfront, for every action you could do on the internet. And to solve it, we would need to think about how to marry design and technology in a new way.
>
> AI Autocomplete solves this, and can now plug into chat interfaces to guide you in real-time, with everything you would need to say, upfront. So you can do anything you can do on the internet in one shot. No more back and forth.
>
> As a result, this unlocks multiple AI breakthroughs:
> 1. 10x faster search and commerce
> 2. Smarter (and far lower cost) media generation
> 3. Natural language advertising
> 4. Powerful, lightweight Augmented Reality
>
> From here, we'll be using this for Hero, but we also want others to use it too since this is an industry-wide problem. So if you have a product that could benefit from AI Autocomplete and want to work with us, reach out below!
>
> Shoutout to @seunglee1b who helped think of and patent this nearly 3 years ago! And shoutout to the entire @hero_assistant team that keeps innovating on the next generation of AI products

- **Tweet:** https://x.com/joulee/status/1988670115014168730
- **What:** Julie Zhuo's endorsement of AI Autocomplete as a paradigm-shifting UI pattern for multi-step actions in chat interfaces.

---


---


# Tuesday, November 11, 2025

## @jiratickets - Hipster Cinema Love
> At the hipster indie cinema. Paid more for the beer than the ticket. I love this place. Always an incredible selection of classic films on the calendar and you can tell the staff truly cares. They even greet me by name. If they knew my political views they'd happily see me killed https://t.co/qGeiBHNBzL

- **Tweet:** https://x.com/jiratickets/status/1988411236904824893
- **What:** A heartfelt appreciation for a local indie cinema with a dark humor twist about differing political views and genuine customer service.

---


---


# Sunday, November 9, 2025

## @thekitze - Claude Code Infrastructure Showcase
> jesus christ some ppl make me feel like i know NOTHING about vibe engineering. WOW.

- **Tweet:** https://x.com/thekitze/status/1987445317076406582
- **Link:** https://github.com/diet103/claude-code-infrastructure-showcase
- **What:** An impressive showcase of Claude Code infrastructure and "vibe engineering" practices that demonstrates advanced implementation patterns.

---


---


# Saturday, November 8, 2025

## @alxfazio - CC-Trace GitHub Repository
> https://github.com/alexfazio/cc-trace

Parent context:
> i built a claude skill that lets claude code reverse-engineer itself
>
> it uses mitmproxy to inspect system prompts and tool definitions, debug slash commands and sub-agents, and more

- **Tweet:** https://x.com/alxfazio/status/1987163101054046361
- **Link:** https://github.com/alexfazio/cc-trace
- **What:** Repository for the cc-trace Claude skill that provides reverse-engineering capabilities for Claude Code inspection and debugging.


---

## @alxfazio - Claude Code Self-Reverse Engineering Skill
> i built a claude skill that lets claude code reverse-engineer itself
>
> it uses mitmproxy to inspect system prompts and tool definitions, debug slash commands and sub-agents, and more
>
> batteries included: guided setup, scripts, and AskUserQuestion tool for simplified usage

- **Tweet:** https://x.com/alxfazio/status/1987163032128999764
- **What:** A Claude skill enabling Claude Code to reverse-engineer itself using mitmproxy to inspect system prompts, tool definitions, and debug commands with included guided setup and utilities.

---


---


# Friday, November 7, 2025

## @kovyrin - Try Tool Workflow Enhancement
> The `try` tool from @tobi has been the biggest positive change to my local workflow in the past year. Nothing comes close. The day I installed and started using it was the last day I lost any of my experiments/plans/repos/docs.
> Highly recommended!

- **Tweet:** https://x.com/kovyrin/status/1986949397079331235
- **Link:** https://github.com/tobi/try
- **What:** Strong endorsement of the "try" tool for local development workflow, highlighting its ability to prevent loss of experimental work, plans, repos, and documentation.

---
DATE: Friday, November 7, 2025

---

## @zeeg - Claude Skills Development Discussion
> Who's made some sick Claude skills that are useful in day to day development (in TS, Next.js, or general)?
>
> Would love to see some canned setups for documentation, spec generation, testing, etc

- **Tweet:** https://x.com/zeeg/status/1986878103722098930
- **What:** David Cramer asking for recommendations on useful Claude skills for development workflows, seeking examples for documentation, spec generation, and testing setups.


---

## @kieranklaassen - Planning Over Vibe Coding with AI Subagents
> The fastest way to ship with AI isn't vibe coding. It's planning.
>
> I built an AI image feature by spending 40 minutes NOT coding—just planning with specialized subagents that research, review, and question the spec. By the time I typed "/work," the implementation was already solved.
>
> Full breakdown + compounding engineering philosophy:

- **Tweet:** https://x.com/kieranklaassen/status/1986873619784634497
- **Link:** https://every.to/source-code/teach-your-ai-to-think-like-a-senior-engineer
- **What:** Kieran Klaassen shares strategies for teaching AI to think like a senior engineer, emphasizing planning with specialized subagents over direct coding to accelerate feature development.


---

## @meowkoteeq - Apple DMCA'd App Store Frontend Repos
> Apple has since DMCA'd repos containing the frontend of their new web App Store.
>
> Some copies might still be up on GitHub, but they'll probably be taken down soon.
>
> If that upsets you, cheer yourself up with this suspiciously large image file of suspicious-looking Tim Cook.

> **Quote:** @ionleu - "oops…"

- **Tweet:** https://x.com/meowkoteeq/status/1986866136399368372
- **What:** Anna reports on Apple's DMCA takedowns of repositories containing the web App Store frontend, noting that copies may still exist on GitHub but will likely be removed.


---

## @doodlestein - Using ast-grep for Pattern Detection in Code
> A useful addendum to your AGENTS dot md or CLAUDE dot md file. First ask codex or claude code to install ast-grep for you if you don't have it already.
>
> It's pretty handy for systematically finding general patterns in code that could be tricky to do using regular string matching that's not syntax-aware.

- **Tweet:** https://x.com/doodlestein/status/1986845121057268083
- **What:** Jeffrey Emanuel recommends ast-grep as a tool for systematically finding syntax-aware code patterns, useful to include in AGENTS or CLAUDE documentation files.

---


---


# Thursday, November 6, 2025

## @ericzakariasson - Code Review Bottlenecks and Diff Viewer Improvements
> reviewing code is already becoming a bottleneck, and there's so much to do with diff viewing. cool to see how small tweaks can have big impact

> **Quote:** @fredrikalindh - "github diffs suck. this open source diff viewer removes 80% of content without removing any context"

- **Tweet:** https://x.com/ericzakariasson/status/1986475583233270237
- **What:** Eric discusses how code review is becoming a bottleneck and highlights an open source GitHub diff viewer that dramatically improves usability by removing unnecessary content while preserving context.

---
DATE: Thursday, November 6, 2025

---

## @jxnlco - Structured Outputs as Foundation for AI Agents
> Structured outputs aren't optional anymore. They're the foundation.
>
> Sharing my final Office Hour notes from this cohort on how we're implementing and evaluating AI agents in production systems.

- **Tweet:** https://x.com/jxnlco/status/1986452775127888211
- **What:** Jason Liu shares insights on structured outputs as the foundation for implementing and evaluating AI agents in production systems, with office hour notes on best practices.


---

## @mattpocockuk - Evalite: TypeScript Testing for AI-Powered Apps
> Ugh you should all use Evalite, it's going to be so good and I love making it and I love seeing people use it and fixing their bugs and seeing them be happy
>
> https://t.co/lHlHtWWdPU

- **Tweet:** https://x.com/mattpocockuk/status/1986425441985642751
- **Link:** https://www.evalite.dev/
- **What:** Evalite is a testing framework for AI-powered applications built in TypeScript. It provides a local dev server for running evaluations and testing AI behaviors, simplifying the evals process for developers.

---


---


# Wednesday, November 5, 2025

## @terrysahaidak - Offscreen and Picture API in React Native Skia Worklets
> @pugson @farcaster_xyz @tanishqxyz not really
>
> i'm talking about Offscreen API or Picture API running purely in worklets.
>
> here i made example in the skia repo about that
>
> https://t.co/RNJEqJ2R5L
>
> **In reply to @pugson:** i think we are talking about the same thing? using Skia.Paint()

- **Tweet:** https://x.com/terrysahaidak/status/1986192583786209672
- **Link:** https://github.com/Shopify/react-native-skia/blob/main/apps/example/src/Examples/Chat/ChatScreen/ChatScreen.tsx#L101-L126
- **What:** Discussion and example implementation of using Offscreen API or Picture API running purely in React Native Skia worklets, demonstrating advanced rendering patterns.


---

## @ScriptedAlchemy - Codex and NAPI for Agent Handoffs
> Codex + NAPI = agent handoffs. https://t.co/GwaJG6No4I

- **Tweet:** https://x.com/ScriptedAlchemy/status/1986175809481228487
- **What:** Notes on using Codex and NAPI for implementing agent handoff patterns, likely related to inter-agent communication and task delegation strategies.


---

## @leerob - Grep Plus Semantic Search Improves Coding Agents
> I've heard people say "grep is all you need" for coding agents, so this research was for me.
>
> Every single model was better with grep + semantic search!
>
> **Quote from @cursor_ai:** Semantic search improves our agent's accuracy across all frontier models, especially in large codebases where grep alone falls short. Learn more about our results and how we trained an embedding model for retrieving code. https://t.co/qL8np1sf8n

- **Tweet:** https://x.com/leerob/status/1986126377188565003
- **What:** Research finding that combines grep with semantic search to improve coding agent performance across all frontier models, particularly valuable in large codebases where traditional grep approaches have limitations.

---
DATE: Wednesday, November 5, 2025

---

## @steipete - MCPort: Generate Self-Contained Bun CLI from MCP
> npx mcporter generate-cli \
  --command https://t.co/tQUFU2qvn2 \
  --compile
>
> Generates a self-contained bun cli out of any mcp.
> https://t.co/fz1tUJA61Q

- **Tweet:** https://x.com/steipete/status/1986036444666675302
- **Link:** https://github.com/steipete/mcporter
- **What:** Tool that generates self-contained Bun CLIs from Model Context Protocol (MCP) servers. Enables packaging MCP implementations as standalone command-line tools with compilation support.

---


---


# Tuesday, November 4, 2025

## @kieranklaassen - Token Efficiency in Agent Design with MCP
> Your agent connects to 50 MCP servers with 1,000 tools. It loads every tool definition into context before reading your request. Then it passes a 10,000-row spreadsheet through the model twice to copy data between tools.
>
> You just burned 150,000 tokens on overhead.
>
> Code execution with MCP solves this: agents write code to call tools, loading definitions on-demand and filtering data in the execution environment. Same task, 2,000 tokens—98.7% reduction.

Quoted context:
> New on the Anthropic Engineering blog: tips on how to build more efficient agents that handle more tools while using fewer tokens.
>
> Code execution with the Model Context Protocol (MCP): https://t.co/PeStmufIkp

- **Tweet:** https://x.com/kieranklaassen/status/1985940599560945753
- **What:** Explanation of token efficiency in AI agent design by using code execution with MCP instead of loading all tool definitions upfront, resulting in 98.7% token reduction.


---

## @boristane - Just-in-Time Tool Discovery with Anthropic's Approach
> anthropic just published a blog highlighting a pattern I've been using for weeks: a search tools tool
>
> instead of loading all tools into the context window of the model, I load a "search tools" tool the model can use to browse a catalog of tools
>
> just-in-time tool discovery https://t.co/EFSm1k2KfB

- **Tweet:** https://x.com/boristane/status/1985930942850924801
- **Link:** https://x.com/boristane/status/1985930942850924801/photo/1
- **What:** Discussion of just-in-time tool discovery pattern for AI agents, where a search tool allows models to browse tool catalogs on-demand.


---

## @mtlushan - Unexpected Dorm Room High Speed Ethernet Experience
> when I filled out the form to activate "high speed ethernet" in my dorm room, I could not have imagined this https://t.co/FaIoLh8dMB

- **Tweet:** https://x.com/mtlushan/status/1985901533116989839
- **Link:** https://x.com/mtlushan/status/1985901533116989839/photo/1
- **What:** Humorous tweet about an unexpected outcome after requesting high-speed ethernet in a dorm room, with an attached image.


---

## @MattWalshBlog - Violence and Political Extremism Summary
> Just to recap the last two months:
>
> -Charlie Kirk shot in the throat on stage
> -Thousands of leftists spend weeks celebrating openly
> -Leftist militants take to the streets committing and calling for more violence
> -Attorney General candidate for Virginia expresses his desire to murder conservatives and watch their children die
> -Democrats voters turn out en masse to vote for him
>
> Do you understand who your enemies are yet?

- **Tweet:** https://x.com/MattWalshBlog/status/1985889998969692307
- **What:** Political commentary summarizing recent violent incidents and their responses, framing a narrative about political divisions.

---
DATE: Tuesday, November 4, 2025

---

## @megbasham - Virginia AG Race and Political Precedent Concerns
> Maybe a tiny sobering moment we could stop and think about on the right – – right now, a candidate who wished for the death of not just his Republican opponents but also their children is leading in the Virginia AG race.
>
> And if he wins, we now have a precedent that you can call for the death of Republicans and still get elected. To me, that's pretty much the most important political story right now.

- **Tweet:** https://x.com/megbasham/status/1985882396525232185
- **What:** Commentary on a Virginia AG candidate's violent rhetoric and its political implications.


---

## @glcst - SQLite Database for AI Agent State Management
> Time and time again we hear from agent builders that they want a database that looks like a filesystem. Where they can store files locally, agent state, tool call state, and basic local observability.
>
> Obviously SQLite is the perfect shape for this. But a higher level of abstraction helps.
>
> I told Pekka not to worry about this now. Which of course means he just started hacking on it anyway, and as usual, it is looking very awesome!

**Quoted context:**
> @penberg: "SQLite is the perfect database for AI agents—but nobody knows how to use it. Many agent developers I've talked to make the same point: SQLite is ideal for capturing agent state, handling auditing, ensuring compliance, and managing snapshots. It's lightweight, all data represented in one single file. But when I ask them what the interface should look like, nobody can really answer. What should the schema look like? How do we make it work across different agent frameworks? How do we handle the filesystem transparently?
>
> After some iteration and conversations with folks building agents, I've identified the three missing pieces:
>
> 1. A standardized schema specification. We need a common way to represent agent state, actions, and outcomes. This isn't just about storing data—it's about enabling an ecosystem of tooling. When everyone uses the same schema, we can build debugging tools, replay systems, and compliance analyzers.
>
> 2. A programmatic SDK. Raw SQL obviously isn't enough. Developers need type-safe APIs, automatic migrations, and framework integrations. The SDK should feel native whether you're using a framework or rolling your own agent system.
>
> 3. A transparent filesystem layer. People building agent compute infrastructure actually want a transparent agent filesystem that works with bash, curl, and friends. Agents shouldn't have to think about where their data lives. They just read and write files, and our system handles the rest.
>
> That why me and @glcst at @tursodatabase have been hacking on AgentFS (https://t.co/qESfjwjC36)—a specification and implementation for agent state management. If you're building agents and fighting with state management, I'd love to hear from you. And if you want to help shape this standard, check out the repo and join the discussion."

- **Tweet:** https://x.com/glcst/status/1985788399488549254
- **What:** Discussion on SQLite's suitability for AI agent state management and the development of AgentFS as a standardized solution with schema specifications and SDK.


---

## @dystopiangf - Immigration and Societal Decline
> One of many problems with mass 3rd world immigration: your country in decline & decay is still a massive improvement over their home countries. They don't even perceive the decline. They'll think "this is as good as it gets" the whole way down, which is terrifying to witness

- **Tweet:** https://x.com/dystopiangf/status/1985766641108722034
- **What:** Commentary on immigration and its perceived effects on societal decline and perception.

---


---


# Monday, November 3, 2025

## @JadeAtrophis - Quote Tweet Comment
> https://t.co/8GzHnHH04F

**Quoted context:**
> @raesanni: "@Ben_Sapo123 I'm a good person. So unlike Erika, I didn't marry a racist homophobe misogynist for clout and I'm not fucking a new racist homophobe misogynist for clout. See how that works?"

- **Tweet:** https://x.com/JadeAtrophis/status/1985403215911788605
- **What:** Quote tweet responding to a social media discussion.

---


---


# Thursday, October 30, 2025

## @kevintwohy - Board Gaming Console Launch
> Here's how we made Board.
>
> A massive team effort of creativity and grit to create a brand new game console, interaction tech, OS, brand, packaging, ecomm, 12 new game titles – and ship it to customers in under 24 months.
>
> The Board team did it and they are just getting started. https://t.co/haquGzRk3y
>
> Check out Board at: https://t.co/X9aAXXMi5D

- **Tweet:** https://x.com/kevintwohy/status/1983930173192806510
- **Link:** https://board.fun/
- **What:** Overview of the Board gaming console project, featuring a 24" face-to-face gaming console combining board game and video game elements with 12 original titles.

---


---


# Wednesday, October 15, 2025

## @dexhorthy - Advanced Claude Code Usage and Research Planning
> superthread of every resource I have published about advanced claude code usage, research-plan-implement, and advanced context engineering for coding agents 👇
>
> (mostly chronological) https://t.co/6Wspo0YIlm

- **Tweet:** https://x.com/dexhorthy/status/1978676162495688719
- **What:** Comprehensive superthread collecting all resources on advanced Claude Code usage, research-plan-implement methodology, and context engineering techniques for coding agents.

---

---

# Tuesday, September 25, 2012

## @KentBeck - Make the Change Easy, Then Make the Easy Change
> for each desired change, make the change easy (warning: this may be hard), then make the easy change

- **Tweet:** https://x.com/KentBeck/status/250733358307500032
- **What:** A core principle of effective programming: the difficulty isn't in making the change itself, but in structuring your code so that the change becomes trivial to implement.

---

