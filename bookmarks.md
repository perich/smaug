
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


# Sunday, January 4, 2026

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


---


# Saturday, January 3, 2026

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
## @GrantSlatton - Looking for quality 100% cotton t-shirt brands
> i'm in the market to replace all my plain white t-shirts

both v-neck and crew neck

does anyone have a 100% cotton t-shirt brand they LOVE both the feel and fit of?

- **Tweet:** https://x.com/GrantSlatton/status/2007654971425337456
- **What:** Personal shopping request for high-quality cotton t-shirts in multiple neckline styles.

---

DATE: Saturday, January 3, 2026
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
## @carolccs1111 - Reply with image
> @rebatheonryo @6asscat https://t.co/fvK5snKIEZ

> *Replying to @rebatheonryo:* @6asscat that nigga was hearing yiddish in his walls

- **Tweet:** https://x.com/carolccs1111/status/2007705529033146674
- **Parent:** https://x.com/rebatheonryo/status/2007684616455631217
- **What:** Image reply in a conversation thread.

---

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


---


# Friday, January 2, 2026

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

## @donvito - GLM 4.7 First Impressions
> wow GLM 4.7 is great

tried it in claude code

- **Tweet:** https://x.com/donvito/status/2006738817773171175
- **Link:** https://z.ai/subscribe?cc=fission_glmcode_sub_v1&ic=V8VOHXNASO&n=Melvin%20Vivas
- **What:** Positive first impression of GLM 4.7 model when used in Claude Code environment, part of the GLM Coding Plan offering AI-powered code generation for agents and IDEs at affordable pricing.

## @emmagine79 - Quick Smaug Implementation Success
> @alexhillman ayyyy thanks for this fam! i was able to use Claude opus + anti gravity to put this together in like 2 hours

- **Tweet:** https://x.com/emmagine79/status/2007051496496714038
- **Media:** Video demonstration
- **What:** Community response to Smaug (Alex's Twitter bookmarks organizer), showing rapid implementation success using Claude Opus - built a similar system in just 2 hours, demonstrating the accessibility and power of AI-assisted development.

## @OsaurusAI - Osaurus Mac AI Agent Demo
> Powered by Osaurus MCP tools.
Claude sees your screen, clicks, types, navigates — you supervise.
This is what AI agents look like on Mac.

- **Tweet:** https://x.com/OsaurusAI/status/2007091913393070168
- **Link:** https://github.com/dinoki-ai/osaurus
- **What:** Native macOS LLM server with MCP support enabling Claude to interact directly with the Mac interface - screen reading, clicking, typing, navigation. Runs local or cloud models with OpenAI/Anthropic compatible APIs. Built in Swift for Apple Silicon.

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

## @parcadei - Continuous Claude v2 Context Management

> *Replying to @yuzu_4ever's critique of Claude Code:* you need this
>
> Context management for Claude Code. Hooks maintain state via ledgers and handoffs. MCP execution without context pollution. Agent orchestration with isolated context windows.

- **Tweet:** https://x.com/parcadei/status/2005755875701776624
- **Parent:** https://x.com/yuzu_4ever/status/2005520908656500964
- **Link:** https://github.com/parcadei/Continuous-Claude-v2
- **Filed:** [Continuous Claude v2](./knowledge/tools/continuous-claude-v2.md)
- **What:** A Python framework for maintaining session continuity and efficient context management in Claude Code workflows, including ledger-based state persistence, MCP execution isolation, and agent orchestration patterns for multi-agent systems.

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


# Tuesday, December 30, 2025

## ## @nosilverv - Glass Airfryer for Frozen Meat Cooking
> This is an incredible product. Take frozen meat -> Put there 10 min -> Delicious meal. No pans, no smoke, no black stuff that gives you cancer, no oils, no cleaning

- **Tweet:** https://x.com/nosilverv/status/2005972663475527751
- **What:** A quote-tweet praising a Ninja glass airfryer, highlighting its convenience for cooking frozen meat without oils, smoke, or cleanup.

---

## ## @Yampeleg - Essential Claude Code Tools and Plugins
> Tools I actually use myself got Claude Code:

1. WhatsApp bridge for Claude Code:

• warelay by @steipete
• https://t.co/S5rxuEvtgs

2. The best browser control plugin:
(i tried them all, this is the most reliable)

• dev-browser by @sawyerhood
• https://t.co/2G0oLKSqzD

3. An incredible collection of tools built to work with one another for everything code related:
(with emphasis on session continuity)

• Continuous-Claude-v2 by @parcadei
• https://t.co/G1U8iytn9s

I use them all by myself, highly recommend trying them out.

Thx for shipping!!

- **Tweet:** https://x.com/Yampeleg/status/2006032038772584885
- **Link:** https://github.com/clawdbot/clawdbot
- **What:** A comprehensive recommendation of three essential Claude Code tools including clawdbot (WhatsApp bridge), dev-browser (browser automation), and Continuous-Claude-v2 for enhanced development workflows.

---

## ## @adocomplete - LSP Integration in Claude Code
> Learn how to integrate LSP into Claude Code: https://t.co/VXvWkCnyqg

- **Tweet:** https://x.com/adocomplete/status/2006050516758073647
- **Link:** https://code.claude.com/docs/en/plugins-reference#lsp-servers
- **What:** A guide on integrating Language Server Protocol (LSP) into Claude Code to enable IDE-level code intelligence features like diagnostics and navigation.

---

## ## @giffmana - AI Video Generation Quality Surprise
> This was surprisingly good O.O

From the replies: Claude + Kling, and my guess is Nano Banana for each shot's first image?

I haven't really kept up with the 2025 video model progress, I've mostly been busy with coding, vlm's, and imagens. So this was a mini-shock to me.

- **Tweet:** https://x.com/giffmana/status/2006106603557187693
- **What:** A reaction to impressive AI-generated video content created with Claude and Kling, noting the significant progress in video generation models during 2025.

---

## ## @jarrodwatts - Custom Claude Code Interview Command for Specs
> I built a custom Claude Code command, /interview, to create bulletproof specs.

• Create a plan using plan mode
• Run the /interview command
• Claude asks 20-50 clarifying questions
• Claude updates the plan file based on your answers

Great for removing any ambiguity! https://t.co/xHrT2fpo8y

- **Tweet:** https://x.com/jarrodwatts/status/2006138974834716993
- **What:** A custom Claude Code command that automates specification creation by asking clarifying questions and updating plan files, helping to eliminate ambiguity in project requirements.

---

## ## @bull_genius - Prepping for the Megaquake DIY Edition

> prepping for the megaquake, DIY gmi edition
>
> >set up phone alerts on all earthquakes
> >on m5+ in text, any m7+ wake me up at night
> >autoshort everything on max leverage on m9+ across multiple perp dex and tradfi venues
> >otm put options on everything japan expiring mar 26
> >garage stocked with ram sticks, vintage nintendo, rare pokemon cards + hentai books
> >you gonna make it anon, now all we have to do is wait
> >chill cozy in my blanket watching the 2024 monroe robertson classic 'planetquake' in director's cut
> >fill out felt reports on significant quakes to advance science at usgs
>
> life is good

- **Tweet:** https://x.com/bull_genius/status/2006154714220519854
- **What:** A humorous take on earthquake hedging strategies that combines financial hedging (shorting on leverage, put options) with earthquake preparedness activities, quoting discussion of elevated megaquake risk in the Pacific region.

---

## ## @kieranklaassen - Claude Code Plugin for 2026 Planning

> Want to use your 2x Claude credits? Use my plugin to plan 2026: https://t.co/BCDTiLlR3t

- **Tweet:** https://x.com/kieranklaassen/status/2006226703467864325
- **Link:** https://github.com/EveryInc/compound-engineering-plugin
- **What:** A promotional tweet for Kieran Klaassen's Compound Engineering Plugin that helps with planning and workflow optimization, enabling developers to make each unit of engineering work easier through improved planning, review, and documentation cycles.

---

## @koylanai - Digital Brain skill for Claude Code
> Agent Skills for Context Engineering - digital brain implementation

- **Tweet:** https://x.com/koylanai/status/2005857134311854480
- **Link:** https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering
- **What:** GitHub repository containing a digital brain skill implementation for Claude Code, enabling advanced context engineering and knowledge management capabilities.

---


---


---


# Monday, December 29, 2025

## ## @ClaudeCodeLog - Comparing Claude Code Versions with Flag and Prompt Changes
> Reminder: You can compare any two versions like this https://t.co/DJreLUDDsl
This will now show both changes in flags and prompts.

- **Tweet:** https://x.com/ClaudeCodeLog/status/2005750479205327284
- **Link:** https://github.com/marckrenn/claude-code-changelog/compare/v2.0.70...v2.0.76

- **What:** A tool for comparing Claude Code versions that now tracks both feature flag changes and system prompt modifications, enabling deep analysis of what's changed between releases.

---

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

## ## @LouisKnightWebb - Shipping 1M+ Lines of Code with AI Agents
> After shipping 1M+ lines of code with AI coding agents, I've started writing up what I've learned: https://t.co/WcB60XEkMn https://t.co/wEhsd3MWgo

- **Tweet:** https://x.com/LouisKnightWebb/status/2005221059491229846
- **Link:** https://www.vibekanban.com/vibe-guide

---

## ## @dejavucoder - Claude Code 2.0 Guide and Best Practices
> claude code is having it's cursor moment after karpathy sensei's post. never been a better time to try it.

my latest blog on how to get the most out of claude code 2.0  and other agents in general is up now. grab a chai and have fun reading!

https://t.co/cQpvo0xocY https://t.co/gzKCEMfEG6

- **Tweet:** https://x.com/dejavucoder/status/2005285904420843892
- **Link:** https://sankalp.bearblog.dev/my-experience-with-claude-code-20-and-how-to-get-better-at-using-coding-agents/

---

## ## @trq212 - Spec-Based Feature Building with Claude Code
> my favorite way to use Claude Code to build large features is spec based

start with a minimal spec or prompt and ask Claude to interview you using the AskUserQuestionTool

then make a new session to execute the spec https://t.co/Lwejskje4a

- **Tweet:** https://x.com/trq212/status/2005315275026260309

---

## ## @trq212 - Interview-Driven Specification Writing
> the prompt I've been using is:

read this @SPEC.md and interview me in detail using the AskUserQuestionTool about literally anything: technical implementation, UI & UX, concerns, tradeoffs, etc. but make sure the questions are not obvious

be very in-depth and continue interviewing me continually until it's complete, then write the spec to the file

- **Tweet:** https://x.com/trq212/status/2005315279455142243

---

## ## @trq212 - Minimal Spec Strategy
> @shafu_xyz Honestly could just be a prompt instead, its just the minimal amount of info you have about the feature imo

- **Tweet:** https://x.com/trq212/status/2005350313574953030

---

## ## @ryancarson - Everyone Needs to See This AI Resource
> Send this to anyone you know who is

1) AI doubter
2) AI casual user
3) nvm … just send it to all your friends

- **Tweet:** https://x.com/ryancarson/status/2005440708677980520

- **What:** A shareable resource about AI that appeals to skeptics, casual users, and everyone in between.

---

## ## @steipete - Shipping at Inference Speed
> 📢 Confession: I ship code I never read. Here's my 2025 workflow. https://t.co/tmxxPowzcR

- **Tweet:** https://x.com/steipete/status/2005451576971043097
- **Link:** https://steipete.me/posts/2025/shipping-at-inference-speed

- **What:** Peter Steinberger shares his workflow for shipping code quickly in 2025 using AI, exploring why watching code stream by is faster than reading it.

---

## ## @hubermanlab - New Stimulants Enhancing REM Sleep and Focus
> Important paper, also for adults who "enjoy" stimulants. A new class of actual focus enhancing stimulants is emerging too— and they seem to enhance REM duration that night. Most are for narcolepsy and no, not Modafinil. 2026 is going to be a banner year for Rx stimulants.

- **Tweet:** https://x.com/hubermanlab/status/2005461253968556096

- **What:** Discussion of emerging stimulant medications that enhance focus and REM sleep, mostly targeting narcolepsy, marking 2026 as significant for prescription stimulant developments.

---

## ## @jonnydels - 49ers Offensive Excellence Reaching Historic Levels
> They just showed a graphic on SNF that this 3-game stretch for the 49ers is their highest 3-game point total since 1994......

People really need to take a step back and realize how crazy what we've seen the past 3 weeks is.

Can we stop talking about what they aren't, what Brock isn't, and talk about how this is the best offensive football we've seen in 30 years? That some have seen from the 49ers in their entire life?

- **Tweet:** https://x.com/jonnydels/status/2005504814738772312

- **What:** A passionate take on the 49ers' historic 3-game scoring stretch, arguing their current offensive performance is the best in 30 years and deserves recognition beyond criticism.

---

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

## ## @zhangjintao9020 - Claude Code Ralph Wiggum Plugin Guide
> 如果你想实现的需求相对确定/可验证，并且你不在意 token 消耗或是订阅制，那么可以在 Claude Code 中使用这个官方插件 Ralph Wiggum。

- **Tweet:** https://x.com/zhangjintao9020/status/2005061204121972748
- **Link:** https://github.com/anthropics/claude-plugins-official/blob/main/plugins%2Fralph-wiggum%2FREADME.md
- **What:** Jintao Zhang shares information about the Ralph Wiggum official plugin for Claude Code, which uses a Stop hook to repeatedly drive Claude to work and verify until requirements are met.

---

## ## @arctotherium42 - Immigration Policy Critique
> Somalis really are the reductio ad absurdum of the lib position on immigration. Highest welfare use and lowest incomes and horrifying cultural practices (FGM) and openly hate America and funnel money to overseas terrorists on top of the billions of dollars in fraud.

- **Tweet:** https://x.com/arctotherium42/status/2005091171148943654
- **What:** A critical commentary on immigration policy and alleged issues related to Somali communities in the United States, quoting Nick Shirley's fraud investigation.

---

## ## @koylanai - Permission Framework for Creative Work
> try this: You don't have to be agreeable right now. You don't have to be comprehensive. You don't have to cover your bases or hedge your bets. The goal isn't to be unkillable—it's to be alive.

- **Tweet:** https://x.com/koylanai/status/2005195637432750523
- **What:** Muratcan Koylan shares a philosophical framework about taste, permission-giving, and the importance of being authentic and alive in creative work over being polished or consensus-approved.

---

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

## ## @nickshirleyy - Minnesota Fraud Investigation Exposé
> 🚨 Here is the full 42 minutes of my crew and I exposing Minnesota fraud, this might be my most important work yet. We uncovered over $110,000,000 in ONE day. Like it and share it around like wildfire! Its time to hold these corrupt politicians and fraudsters accountable

- **Tweet:** https://x.com/nickshirleyy/status/2004642794862961123
- **What:** Nick Shirley released a 42-minute investigation documenting alleged fraud cases totaling over $110 million discovered in a single day, focusing on corruption and government accountability.

---

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

## ## @doodlestein - Agent Flywheel Learning Hub Launch
> I added a whole "Learning Hub" to https://t.co/TKaKxRJ3V5 for after you've finished setting up your cloud machine with all the tools and aren't sure what to do next or how to best leverage the tools

- **Tweet:** https://x.com/doodlestein/status/2004333644484374707
- **Link:** https://agent-flywheel.com/learn
- **What:** Jeffrey Emanuel released a Learning Hub for Agent Flywheel, providing guided lessons and tutorials for developers who have set up their agentic coding environment and need guidance on next steps.

---

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


---


# Wednesday, December 24, 2025

## ## @ServoWealth - Asset Class Diversification Impact on Retirement Success
> The most shocking retirement investing stat you'll ever read!?!
>
> If you retired in 2000 (similar stock valuations to today) with $1M, needing $50k/yr plus inflation:
>
> 1. If you put it in S&P 500, you RAN OUT OF $ in 2016
>
> 2. If you put it into 60/40 S&P 500/Total Bond, you are down to $199K (about to go broke)
>
> 3. If you put it into an all-stock asset class portfolio diversified across U.S. & Int'l large & small value, you have over $2.9M left (tripled your wealth)
>
> If you're retiring on anything other than a diversified asset class portfolio you're taking a huge risk of running out of $

- **Tweet:** https://x.com/ServoWealth/status/2003853807881437506
- **What:** A comparison of retirement outcomes using $1M with $50k annual withdrawals, showing that diversified asset class portfolios significantly outperform traditional S&P 500 or 60/40 allocations over a 25-year period.

---

## ## @koylanai - Agent Skills for Context Engineering Gaining Traction on Replicate
> This is incredible. Three days. ~1500 GitHub stars.

Agent Skills for Context Engineering #1 on @replicate Hype today 🧙

AI community is hungry for operational knowledge about agents. Not another framework release. Not another benchmark. Practical skills for building systems that work.

Context engineering is becoming the discipline that separates agents that demo well from agents that run in production.

This repo is essentially my notebook from the past year. Next: I'm adding more skills soon.

Thank you to everyone who starred, forked, and shared. This is just the beginning.

- **Tweet:** https://x.com/koylanai/status/2003948029661893093
- **Link:** https://hype.replicate.dev/
- **What:** A discussion of the rapid growth and community reception of an Agent Skills for Context Engineering repository that's trending on Replicate's Hype platform. The author reflects on how AI developers are seeking practical, operational knowledge for building production-ready agents rather than new frameworks.

---

## ## @ChangJonathanC - Running Claude Code as a Separate User for Safety
> @trq212 I do it but let Claude run as a separate user
https://t.co/tX6QKsPLDr

- **Tweet:** https://x.com/ChangJonathanC/status/2004006928335409362
- **Link:** https://jonathanc.net/blog/claude-daemon
- **What:** A practical security approach for running Claude Code safely using macOS user isolation and ACLs to limit permissions, avoiding the risks of running with dangerous flag overrides in the home directory.

---

## ## @thenarrator - Why Prediction Markets Force Accountability Into Beliefs
> this is one of the clearest explanations of why prediction markets matter that I've seen.

Vitalik is basically saying:

> prediction markets aren't about gambling, they're about forcing accountability into beliefs.

> on social media, people get rewarded for being loud, extreme, and wrong.

whereas on prediction markets, you get punished for being wrong  and that flips incentives completely.

> what's powerful here is the idea that markets discipline narratives.

you can scream "this will definitely happen" on X and get likes, but the moment you have to put money behind it, uncertainty suddenly matters.

that's why prediction markets feel healthier than most info ecosystems:

> lies are costly
> confidence has a price
> reality settles arguments

they don't eliminate misinformation, but they price and that alone makes them one of the most honest coordination tools we've ever built.

- **Tweet:** https://x.com/thenarrator/status/2004038759843496300
- **What:** An analysis of how prediction markets create better information ecosystems by punishing incorrect predictions and forcing believers to put economic skin in the game, contrasting with social media's incentives for extreme claims without accountability.

---

## ## @steipete - Dash - Amazing Terminal UI for GitHub
> God damn. Dash is amazing!  https://t.co/YfsZmfNOar

- **Tweet:** https://x.com/steipete/status/2004217462049702230
- **Link:** https://www.gh-dash.dev/
- **What:** A brief endorsement of DASH, a rich terminal UI tool that allows developers to navigate and manage their GitHub repositories without leaving the command line.

---


---


# Tuesday, December 23, 2025

## ## @EnoReyes - Agent-Ready Codebases
> AI Agents require verification loops to succeed, and software is incredibly verifiable. Most codebases don't actually provide these signals to agents.

Companies that invest in agents + agent readiness will see 5-10x the return of those who don't.

- **Tweet:** https://x.com/EnoReyes/status/2003483475157127650
- **What:** Argues that AI agents succeed when codebases provide clear verification signals through good specs and validation, and companies investing in "agent readiness" will gain significant competitive advantage.

---

## ## @vvhuang_ - AI Paper on Proactive User Assistance
> 7mo late but i think i found my favorite AI paper of 2025!

tldr: secure, local (V)LMs observe computer activity, learn a natural-language model of the user, & use the model to proactively assist the user in completing tasks

very simple idea, very thoughtfully implemented https://t.co/LLjr163Kb7

- **Tweet:** https://x.com/vvhuang_/status/2003506217415770473
- **Link:** https://x.com/vvhuang_/status/2003506217415770473/photo/1
- **What:** Highlights an AI paper that uses local vision language models to observe user behavior, learn their patterns, and proactively assist with tasks—balancing simplicity with thoughtful implementation.

---

## ## @JayaGup10 - Article or Thread Share
> https://t.co/uPXcTUEsnc

- **Tweet:** https://x.com/JayaGup10/status/2003525933534179480
- **Link:** https://x.com/i/article/2003525085420744704
- **What:** A shared article or thread from Jaya Gupta (content details not available in bookmark metadata).

---

## ## @benhylak - Structured Prompts as Functions at Raindrop
> at @raindrop_ai, we like to treat every prompt as a function: structured inputs, structured outputs
>
> every function used to prepare the input for the model lives in the same prompt file, and we have an extension for iterating on the prompt right inside our codebase. https://t.co/EHELJQBJDo

- **Tweet:** https://x.com/benhylak/status/2003536316080828455
- **Link:** https://x.com/benhylak/status/2003536316080828455/video/1
- **What:** A technique at Raindrop AI for treating prompts as functions with structured inputs/outputs and maintaining them alongside code with extensions for iteration.

---

## ## @YuxiangWei9 - Self-Play SWE-RL for Agent Self-Improvement
> Software agents can self-improve via self-play RL
>
> Introducing Self-play SWE-RL (SSR): training a single LLM agent to self-play between bug-injection and bug-repair, grounded in real-world repositories, no human-labeled issues or tests. 🧵

- **Tweet:** https://x.com/YuxiangWei9/status/2003541373853524347
- **What:** A method for training LLM agents to self-improve through self-play reinforcement learning, alternating between bug injection and repair tasks using real-world code repositories.

---

## ## @aiDotEngineer - Amp Code: Next Generation AI Coding Agent
> 🆕 Amp Code: Next Generation AI Coding
>
> https://t.co/xjKvgUnhId
>
> @AmpCode recently spun out as an independent agent lab from @Sourcegraph. 4x (!) returning champion @beyang returns to discuss the journey of building Amp, and explore 8 of the strong opinions they have developed in building their nextgen coding agent... including rejecting MCP slop!

- **Tweet:** https://x.com/aiDotEngineer/status/2003558055875944822
- **Link:** https://www.youtube.com/watch?v=gvIAkmZUEZY
- **What:** A video discussion about Amp Code, a new AI coding agent spun out from Sourcegraph, featuring insights from the team about their development philosophy and opinions on AI coding tools.

---

## ## @badlogicgames - Claude for Chrome Privacy Analysis
> Just quicky, I'm tired. It appears the the sidepanel frontend is actually making all the requests. The background service doesn't make any requestr (so far).
>
> Every time the url changes in a tab, the sidepanel sends that info to the mothership. They also send telemetry to https://t.co/PlcdIGZCWd, basically a browser/machine fingerprint.

- **Tweet:** https://x.com/badlogicgames/status/2003586083729162484
- **Link:** https://www.honeycomb.io/
- **What:** A reverse engineering analysis showing that Claude for Chrome sends browser/machine fingerprint telemetry to Honeycomb every time the URL changes.

---

## @steve_ike_ - AI Adoption Playbook
> This might be the cleanest AI adoption playbook inside a real product org I've seen.

- **Tweet:** https://x.com/steve_ike_/status/2003497265495785523
- **What:** 15-point comprehensive playbook covering practical approaches to implementing AI across organizations, from "How I AI" podcast.

---


---


---


# Monday, December 22, 2025

## ## @rrhoover - Personal Peptide Experimentation and Health Optimization
> Reading this overview on the peptide boom (with some cautions).
>
> BPC-157 was my gateway after some knee issues.
>
> I've used peptides on and off for a few years, including CJC+Ipa, Sermorelin, Melanotan II (wildly affective but I don't recommend for most), GHK-Cu (caused aches), and others.

- **Tweet:** https://x.com/rrhoover/status/2003136459021181435
- **What:** Ryan Hoover sharing personal experience with peptide-based health optimization treatments and their varying effectiveness.

---

## ## @irl_danB - Context Windows and Agent Architecture
> context window won't be "solved" as long as attention is quadratic

and presumably Suhail is thinking about the compaction problem as it occurs in long running agents like claude code

but this is downstream from an architectural problem with standard agent implementations (claude code among them) that use a linear "chat-like" history

we all work through coding tasks linearly, but any seasoned software engineer's mental model of their progress looks more like a call stack: pushing tasks on and popping them off when complete

when the claude code harness organizes the context more like a call stack (think flame graph) than a linear chat log, compaction will not even be necessary in many cases and less lossy in the cases where it is

for the familiar, think: loom

- **Tweet:** https://x.com/irl_danB/status/2003223600195625356
- **What:** Technical analysis of how context window limitations in AI systems are fundamentally tied to quadratic attention complexity, and proposing a call-stack-based architecture instead of linear chat histories could better model how developers actually think through problems.

---

## ## @kodisha - Rust Tooling Performance Wins
> I am currently migrating some old repos:

typecheck: tsc -> tsgo  => at least 5-10x speedup
lint: eslint -> oxlint => insane, 15-20 sec to 25ms
format: prettier -> oxformat => 4s to 500ms
build: vite to rolldown-vite => 110s to ~4s 💀

Insane work @OxcProject  @youyuxi  🔥

- **Tweet:** https://x.com/kodisha/status/2003272433386795293
- **What:** Demonstrates massive performance improvements (5-20x speedups) by migrating TypeScript tooling from JavaScript-based tools to Rust-based alternatives like oxlint and rolldown.

---


---


# Sunday, December 21, 2025

## ## @sweatystartup - Hidden Heart Disease Risk in Young Healthy Adults
> It starts in your 20s. In nearly everyone.
>
> Go get an angiogram if you make real money.
>
> A CAC score doesn't show widow maker plaque. Or soft plaque.

- **Tweet:** https://x.com/sweatystartup/status/2002939161633047002
- **What:** Nick Huber advocating for angiograms as essential heart health screening, noting limitations of CAC scores for detecting dangerous plaque.

---


---


# Saturday, December 20, 2025

## ## @badlogicgames - Mario Zechner Discovers Zagi Project
> @mattzcarey So, I was just googling zagi and came up short. Hunted it down on your GH account. You need to work on that self-promotion :)
>
> This looks super cool!

- **Tweet:** https://x.com/badlogicgames/status/2002462374088053232
- **Link:** https://github.com/mattzcarey/zagi
- **What:** Mario Zechner discovering and endorsing Matt Carey's zagi project while encouraging better self-promotion.

---


---


# Friday, December 19, 2025

## ## @GrageDustin - Voter Fraud Investigation in Minnesota Somali Community
> 🚨 BREAKING EXCLUSIVE: We have uncovered records outlining an organized voter fraud scheme in the Somali Community here in Minnesota.
>
> The county prosecutor declined to charge the case, but the Trump Administration needs step in to clean up Minnesota's elections. 🧵

- **Tweet:** https://x.com/GrageDustin/status/2002071157382787372
- **What:** Allegations of organized voter fraud involving the Somali community in Minnesota with details presented on alleged lack of prosecution.

---

## ## @theo - Open Source OCR Solution olmOCR Cost Breakdown
> If you want a competent, actually open solution, highly recommend olmOCR. Costs under $200 to process a million pages. Fully open source as well :)

- **Tweet:** https://x.com/theo/status/2002178958196895782
- **What:** Recommendation for olmOCR as a cost-effective and fully open source alternative for OCR processing at significant scale.

---


---


# Thursday, December 18, 2025

## ## @simonw - Engineering Accountability: Submitting Proven Code
> I see a lot of complaints about untested AI slop in pull requests. Submitting those is a dereliction of duty as a software engineer:  Your job is to deliver code you have proven to work https://t.co/Eso7BWaTtF

- **Tweet:** https://x.com/simonw/status/2001668038664593493
- **Link:** https://simonwillison.net/2025/Dec/18/code-proven-to-work/
- **What:** Simon Willison argues that software engineers must demonstrate tested, working code in PRs rather than submitting untested AI-generated code for others to review and validate.

---

## ## @doodlestein - ElevenLabs Audio Narration for Information Consumption
> One side effect of my alarming addition to coding agents is that I work every single day until my eyes are too tired to read anything.
>
> And so even though I've always been dismissive of audiobooks and listening as an inferior, slower way to absorb information, with dramatically worse comprehension and retention (all of which is unfortunately still true in my case), it's now the only way I can realistically consume certain kinds of content, since I can do it with my eyes closed in bed.
>
> And so, surprisingly to me, one of my most-used apps now is the Eleven Labs reader app. You can paste in a link to an article or book or just some random text and have it read to you in a pretty natural, inoffensive way.
>
> I'm partial to the "George" voice, but they have so many to choose from that you can surely find one that you don't find annoying.
>
> At $5/month, my Eleven subscription is probably the single best value proposition across all my many AI service subscriptions.

- **Tweet:** https://x.com/doodlestein/status/2001755881441226922
- **What:** Personal reflection on using ElevenLabs text-to-speech narration as a practical solution for consuming content when visual reading becomes impractical, highlighting it as an excellent value among AI service subscriptions.

---

## ## @trq212 - Claude Code Chrome Extension for Browser Testing
> Claude Code can now control your browser for testing, getting data, etc. using our chrome extension!

- **Tweet:** https://x.com/trq212/status/2001764339506909270
- **What:** Announcement that Claude Code now supports browser control via a Chrome extension, enabling direct testing and data extraction capabilities within the browser environment.

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


# Monday, November 24, 2025

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

## @MatthewBerman - Opus 4.5 Outperforms All Humans on Anthropic Interview Exam
> Absolutely insane stat.
>
> Opus 4.5 outperformed EVERY SINGLE HUMAN CANDIDATE EVER in Anthropic's notoriously difficult take-home exam for prospective performance engineering candidates. https://t.co/RJxlgwUlCy

- **Tweet:** https://x.com/MatthewBerman/status/1993038043876671863
- **What:** Remarkable benchmark showing that Claude Opus 4.5 has outperformed every single human candidate in Anthropic's challenging take-home exam for performance engineering positions.

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

## @XJosh - Understanding Izzat: India's Cultural Honor System
> Kiwi Farms user breaks down 'Izzat', the Indian subcontinent's cultural honor system. It effectively explains every single trope about Indian behavior: they all participate in an invisible clout-chasing game that involves screwing over everyone as much as possible. Worth the read https://t.co/Ob4mkqt7H6

- **Tweet:** https://x.com/XJosh/status/1992348701793349827
- **Link:** https://x.com/XJosh/status/1992348701793349827/photo/1
- **What:** Analysis of 'Izzat', the Indian cultural honor system, explaining it as a clout-chasing game that drives interpersonal behavior in the Indian subcontinent.

## @alexhillman - Always Do (11 Imperatives)
> Always Keep Humans at the Center - use AI to remove drudgery and free up time for real, authentic relationships

- **Tweet:** https://x.com/alexhillman/status/1992252350812270856
- **What:** Personal reflection on core imperatives with emphasis on keeping humans central to all technology decisions.


---


---


# Friday, November 21, 2025

---
DATE: Friday, November 21, 2025
## @AlphaNews - Derek Chauvin Petition Alleges Prosecutorial Misconduct
> BREAKING: Derek Chauvin's attorney files new petition, says prosecution 'can only run from the truth for so long'
>
> In a bombshell petition—alleging prosecutorial misconduct—more than 50 former and current officers have provided sworn declarations stating that the technique used by Derek Chauvin and the other Minneapolis police officers involved in the arrest of George Floyd was part of MPD training.

- **Tweet:** https://x.com/AlphaNews/status/1992031829843431689
- **What:** Breaking news on Derek Chauvin's attorney filing a petition alleging prosecutorial misconduct in the George Floyd case, with 50+ officers providing sworn declarations that the technique used was part of standard MPD training.

## @mitsuhiko - Agent Design Challenges and Insights
> Well, @badlogicgames reminded of the value of sharing, so here's the update: agent building is hard. Agent SDKs are tricky, caching is a per-model art, reinforcement can help, isolation saves your sanity, filesystems! New models are "it depends." https://t.co/6RiHJysI20

- **Tweet:** https://x.com/mitsuhiko/status/1992000898147766638
- **Link:** https://lucumr.pocoo.org/2025/11/21/agents-are-hard/
- **What:** Armin Ronacher shares key learnings about agent design complexity, covering SDK abstractions, caching strategies, reinforcement learning, isolation patterns, and the model-dependent nature of agentic AI.

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

## @aeitroc - Quibbler Hook Recommendation
> @bcardarella Add this hook https://t.co/Q0OIrbbkym

**Parent Tweet:** @bcardarella - I told Claude to one-shot an integration test against a detailed spec I provided. It went silet for about 30 minutes. I asked how it was going twice and it reassured me it was doing work. Then I asked why it was taking so long: https://t.co/1Oc1zbhFcQ

- **Tweet:** https://x.com/aeitroc/status/1991564773323075714
- **Link:** https://github.com/fulcrumresearch/quibbler
- **What:** Bessi recommends using the Quibbler hook to address Brian Cardarella's issue with Claude spending excessive time on integration test generation.

---


---


# Wednesday, November 19, 2025

---
DATE: Wednesday, November 19, 2025
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

## @badlogicgames - Context Limitations: GPT vs Claude on Large Files
> The best part is that it doesn't even truncate to 10kb but 5kb.
>
> That file has 2200 lines, which fit snuggly inside the context. Alas, poor GPT won't see even a 10th of the content.

- **Tweet:** https://x.com/badlogicgames/status/1989863756814336032

- **What:** Discussion about how Claude can fit 2200-line files in context while GPT has severe truncation limits (5kb), highlighting the context window advantage for agents working with large source files.

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

---
DATE: Friday, November 14, 2025
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

## @mikeyk - Claude Frontend Design Skills Plugin
> Our Applied AI team with a great write up on improving Claude's frontend design via Skills. Also with a Claude Code plugin that packages up the skill!
> https://t.co/5gPFn5UwhW

- **Tweet:** https://x.com/mikeyk/status/1988691831836782610
- **Link:** https://www.claude.com/blog/improving-frontend-design-through-skills
- **What:** Mike Krieger highlights a blog post about enhancing frontend design capabilities through Claude Skills, with an accompanying Claude Code plugin.

## @trq212 - Deep Research with Claude Agent SDK
> We built a Deep Research demo for the Claude Agent SDK!
>
> It's one our most requested use cases: spawn multiple AI agents to research a topic in parallel, then synthesize their findings into a report.
>
> on how it works: https://t.co/jU2kRc9hIq

- **Tweet:** https://x.com/trq212/status/1988690675542675536
- **What:** Thariq announces a Deep Research demo showcasing parallel agent research capability within the Claude Agent SDK for comprehensive report synthesis.

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

---
DATE: Tuesday, November 11, 2025
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
## @zeeg - Claude Skills Development Discussion
> Who's made some sick Claude skills that are useful in day to day development (in TS, Next.js, or general)?
>
> Would love to see some canned setups for documentation, spec generation, testing, etc

- **Tweet:** https://x.com/zeeg/status/1986878103722098930
- **What:** David Cramer asking for recommendations on useful Claude skills for development workflows, seeking examples for documentation, spec generation, and testing setups.

## @kieranklaassen - Planning Over Vibe Coding with AI Subagents
> The fastest way to ship with AI isn't vibe coding. It's planning.
>
> I built an AI image feature by spending 40 minutes NOT coding—just planning with specialized subagents that research, review, and question the spec. By the time I typed "/work," the implementation was already solved.
>
> Full breakdown + compounding engineering philosophy:

- **Tweet:** https://x.com/kieranklaassen/status/1986873619784634497
- **Link:** https://every.to/source-code/teach-your-ai-to-think-like-a-senior-engineer
- **What:** Kieran Klaassen shares strategies for teaching AI to think like a senior engineer, emphasizing planning with specialized subagents over direct coding to accelerate feature development.

## @meowkoteeq - Apple DMCA'd App Store Frontend Repos
> Apple has since DMCA'd repos containing the frontend of their new web App Store.
>
> Some copies might still be up on GitHub, but they'll probably be taken down soon.
>
> If that upsets you, cheer yourself up with this suspiciously large image file of suspicious-looking Tim Cook.

> **Quote:** @ionleu - "oops…"

- **Tweet:** https://x.com/meowkoteeq/status/1986866136399368372
- **What:** Anna reports on Apple's DMCA takedowns of repositories containing the web App Store frontend, noting that copies may still exist on GitHub but will likely be removed.

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
## @jxnlco - Structured Outputs as Foundation for AI Agents
> Structured outputs aren't optional anymore. They're the foundation.
>
> Sharing my final Office Hour notes from this cohort on how we're implementing and evaluating AI agents in production systems.

- **Tweet:** https://x.com/jxnlco/status/1986452775127888211
- **What:** Jason Liu shares insights on structured outputs as the foundation for implementing and evaluating AI agents in production systems, with office hour notes on best practices.

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

## @ScriptedAlchemy - Codex and NAPI for Agent Handoffs
> Codex + NAPI = agent handoffs. https://t.co/GwaJG6No4I

- **Tweet:** https://x.com/ScriptedAlchemy/status/1986175809481228487
- **What:** Notes on using Codex and NAPI for implementing agent handoff patterns, likely related to inter-agent communication and task delegation strategies.

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

## @boristane - Just-in-Time Tool Discovery with Anthropic's Approach
> anthropic just published a blog highlighting a pattern I've been using for weeks: a search tools tool
>
> instead of loading all tools into the context window of the model, I load a "search tools" tool the model can use to browse a catalog of tools
>
> just-in-time tool discovery https://t.co/EFSm1k2KfB

- **Tweet:** https://x.com/boristane/status/1985930942850924801
- **Link:** https://x.com/boristane/status/1985930942850924801/photo/1
- **What:** Discussion of just-in-time tool discovery pattern for AI agents, where a search tool allows models to browse tool catalogs on-demand.

## @mtlushan - Unexpected Dorm Room High Speed Ethernet Experience
> when I filled out the form to activate "high speed ethernet" in my dorm room, I could not have imagined this https://t.co/FaIoLh8dMB

- **Tweet:** https://x.com/mtlushan/status/1985901533116989839
- **Link:** https://x.com/mtlushan/status/1985901533116989839/photo/1
- **What:** Humorous tweet about an unexpected outcome after requesting high-speed ethernet in a dorm room, with an attached image.

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
## @megbasham - Virginia AG Race and Political Precedent Concerns
> Maybe a tiny sobering moment we could stop and think about on the right – – right now, a candidate who wished for the death of not just his Republican opponents but also their children is leading in the Virginia AG race.
>
> And if he wins, we now have a precedent that you can call for the death of Republicans and still get elected. To me, that's pretty much the most important political story right now.

- **Tweet:** https://x.com/megbasham/status/1985882396525232185
- **What:** Commentary on a Virginia AG candidate's violent rhetoric and its political implications.

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

---
DATE: Wednesday, October 15, 2025
## @dexhorthy - Advanced Claude Code Usage and Research Planning
> superthread of every resource I have published about advanced claude code usage, research-plan-implement, and advanced context engineering for coding agents 👇
>
> (mostly chronological) https://t.co/6Wspo0YIlm

- **Tweet:** https://x.com/dexhorthy/status/1978676162495688719
- **What:** Comprehensive superthread collecting all resources on advanced Claude Code usage, research-plan-implement methodology, and context engineering techniques for coding agents.

---


---


# Wednesday, December 17, 2025

## ## @ExaAILabs - Semantic People Search with 1 Billion Profiles
> Introducing state-of-the-art People Search:
>
> You can now semantically search over 1 billion people using a hybrid retrieval system backed by finetuned Exa embeddings.
>
> Try it: https://t.co/cQ6UlWHnKY
> We also created an eval: https://t.co/2OIAryN7MT https://t.co/12BdYDWJU1

- **Tweet:** https://x.com/ExaAILabs/status/2001373897154007390
- **Link:** https://exa.ai/
- **What:** Exa released a semantic people search feature enabling searches across 1 billion profiles using finetuned embeddings and hybrid retrieval, along with a benchmark evaluation.

---

## ## @JDVance - DEI as Systemic Discrimination Against White Men
> A lot of people think "DEI" is lame diversity seminars or racial slogans at NFL games. In reality, it was a deliberate program of discrimination primarily against white men. This is an incredible piece that describes the evil of DEI and its consequences:
>
> https://t.co/fMiIfvz0qz

- **Tweet:** https://x.com/JDVance/status/2001404279517478927
- **Link:** https://www.compactmag.com/article/the-lost-generation/
- **What:** Opinion piece arguing that DEI initiatives represent systemic discrimination, with analysis of the generational impacts and consequences of these programs.

---

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

## @Yampeleg - Claude Code v2.0.71 Release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://x.com/Yampeleg/status/2001360661700596119/photo/1

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Recommendation to update Claude Code to v2.0.71, suggesting significant improvements or features in the latest release.

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

## @Yampeleg - Claude Code v2.0.71 release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://t.co/czN80tHvAY

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic announcement of Claude Code v2.0.71 release with a photo showing the update is available.

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

## @Yampeleg - Claude Code v2.0.71 release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://t.co/czN80tHvAY

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic recommendation to update Claude Code to version 2.0.71 with accompanying media preview.

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

## @RapidResponse47 - Trump Accounts Government Portal Update
> JUST UPDATED: https://trumpaccounts.gov/

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **Link:** https://trumpaccounts.gov/
- **What:** Brief announcement of updates to the Trump accounts government portal.

---

## @Yampeleg - Claude Code v2.0.71 Release
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://x.com/Yampeleg/status/2001360661700596119/photo/1

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic announcement about Claude Code v2.0.71 release with strong approval.

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

## @RapidResponse47 - Trump Accounts Portal Update
> JUST UPDATED: https://trumpaccounts.gov/

- **Tweet:** https://x.com/RapidResponse47/status/2001314232210465267
- **Link:** https://trumpaccounts.gov/
- **What:** Brief update notification about a portal related to Trump accounts and official government information.

---

## @Yampeleg - Claude Code v2.0.71 Release Update
> Stop what u do and update Claude Code to v2.0.71.
>
> They cooked. https://x.com/Yampeleg/status/2001360661700596119/photo/1

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic announcement about a new Claude Code release (v2.0.71) with positive sentiment about the update quality.

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

## @Yampeleg - Claude Code v2.0.71 Release
> Stop what u do and update Claude Code to v2.0.71.\n\nThey cooked.

- **Tweet:** https://x.com/Yampeleg/status/2001360661700596119
- **What:** Enthusiastic announcement about Claude Code v2.0.71 release with an attached image/media.

---


# Tuesday, December 16, 2025

---
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
## @nicolaygerold - Tool search should not be search but discovery
> If you are one of the ones who cares about context management and wants to have tools and a clean context window, here is me blabbing about tool search:
>
> https://t.co/QOiUXSrKXb

- **Tweet:** https://x.com/nicolaygerold/status/2000963680570368089
- **Link:** https://nicolaygerold.com/posts/tool-search-should-not-be-just-search-but-discovery
- **What:** Deep dive into context management and tool discovery mechanisms in LLM agents. Explores why deferred tool loading is more complex than it appears.

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
