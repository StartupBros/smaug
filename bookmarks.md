# Wednesday, March 25, 2026

## @aakashgupta - Karpathy's Autoresearch Vision: From Single Agent to Autonomous Research Community
> Karpathy buried the most important part of autoresearch in the README, and almost nobody read it.

Above the installation instructions, he wrote a short fiction piece set in the future. Autonomous swarms of AI agents running across compute cluster megastructures. Generation 10,205 of a self-modifying codebase that has grown beyond human comprehension. No researchers in the loop. Then the last line: "This repo is the story of how it all began."

He's telling you what he thinks he built.

Today the repo is 630 lines of Python. One GPU. One file the agent can edit. 5-minute training runs. 12 experiments per hour. You wake up to a results.tsv and a cleaner git history. Cute.

But Karpathy already posted the roadmap. Step one was the single-agent loop, which is what shipped. Step two is asynchronous collaboration. Thousands of agents running parallel branches on different GPUs, contributing findings back to a shared repo. He compared it to SETI@home. His exact words: "The goal is not to emulate a single PhD student, it's to emulate a research community of them."

Step three is what he described on X as agents promoting the most promising ideas to increasingly larger scales. Small model finds an architectural improvement. Mid-size model validates it. Frontier model absorbs it. A research pipeline where each stage filters signal from noise automatically.

42,000 GitHub stars in a week. 5,800 forks. Community ports running on Mac Minis, RTX cards, 4GB laptops. One user on a GeForce 1050 Ti got it working. The surface area for this swarm already exists. Distributed GPUs sitting idle overnight in every developer's apartment, every university lab, every startup office.

Shopify's CEO ran it on company data overnight and got a 19% gain from 37 experiments. Imagine 10,000 agents running 37 experiments each. 370,000 experiments. The ones that improve get promoted. The ones that fail get reverted. The system remembers everything.

Karpathy spent a decade at the center of AI research. He co-founded OpenAI. He ran AI at Tesla. He coined "vibe coding." When someone with that track record writes a fictional origin story for autonomous AI research and then publishes the first chapter as open source, the fiction is the spec.
>
> *Quoting @aakashgupta:* For $25 and a single GPU, you can now run 100 experiments overnight without designing any of them.

Karpathy open-sourced autoresearch. 42,000 GitHub stars in a week. Fortune called it "The Karpathy Loop."

Every article about it focused on the ML angle. They all missed the bigger story. The pattern underneath works on anything you can score with a number. Ad copy, cold emails, video scripts, job posts, skill files.

Three files. One the agent edits. One it can never touch. One instruction file from you. Each cycle takes 5 minutes. Score went up? Git commit. Score went down? Git reset. Twelve cycles per hour. A hundred overnight.

Karpathy ran it on code he'd already optimized by hand for months. The agent found 20 improvements he'd missed. 11% faster. Tobi Lutke pointed it at Shopify's Liquid templating engine. 53% faster rendering from 93 automated commits.

I spent two weeks pulling the system apart. Today's guide shows you how to use it on the things you actually make every day. Six use cases, the three-step setup, and the eval mistakes that kill runs before they start.

- **Tweet:** https://x.com/aakashgupta/status/2036666385099870394
- **Link:** https://www.aibyaakash.com/p/autoresearch-guide
- **What:** Aakash Gupta reads between the lines of Karpathy's autoresearch README fiction — a spec for autonomous swarms of AI agents doing distributed research across idle GPUs worldwide — and argues the 630-line repo shipped today is just chapter one of that roadmap.


## @aakashgupta - Karpathy's Autoresearch: The Spec Hidden in the Fiction
> Karpathy buried the most important part of autoresearch in the README, and almost nobody read it. Above the installation instructions, he wrote a short fiction piece set in the future. Autonomous swarms of AI agents running across compute cluster megastructures. Generation 10,205 of a self-modifying codebase that has grown beyond human comprehension. Then the last line: "This repo is the story of how it all began." He's telling you what he thinks he built.
>
> *Quoting @aakashgupta:* For $25 and a single GPU, you can now run 100 experiments overnight without designing any of them. Karpathy open-sourced autoresearch. 42,000 GitHub stars in a week. Fortune called it "The Karpathy Loop." Three files. One the agent edits. One it can never touch. One instruction file from you. The roadmap: single-agent loop (shipped) → async multi-GPU collaboration → staged self-improvement pipelines.

- **Tweet:** https://x.com/aakashgupta/status/2036666385099870394
- **Quoted:** https://x.com/aakashgupta/status/2034851259442749909
- **Filed:** [karpathy-autoresearch-guide](./knowledge/articles/karpathy-autoresearch-guide.md)
- **What:** Aakash Gupta argues Karpathy's fictional README intro is actually the product spec — tracing the 3-step roadmap from single-agent loops to async multi-GPU swarms to staged self-improvement, with Shopify's 53% Liquid rendering gain and 42k GitHub stars as proof the distributed GPU surface already exists.

---

# Tuesday, March 24, 2026

## @garrytan - GStack Adversarial Autoplan Workflow: One-Shot Code with 100% Test Coverage
> Building your own tools like GStack is an amazing experience. You come up with something you think might work and then two days later it replaces what you were doing before.
>
> Instead of /plan-ceo-review and /plan-eng-review sequentially, I find myself using "/autoplan with adversarial review" every time (it is kind of like Claude's -auto-mode but for making choices that my prompts used to ask)
>
> And after I finalize the plan and exit plan mode, CC codes it all, and then I do "/review with full claude and codex, full adversarial with claude and codex"
>
> And then it just one-shots everything from there, no bugs, 100% test coverage

- **Tweet:** https://x.com/garrytan/status/2036638037908836635
- **What:** Garry Tan describes his GStack workflow evolution — replacing sequential `/plan-ceo-review` + `/plan-eng-review` passes with a single `/autoplan with adversarial review`, then finishing with a dual-model adversarial code review (Claude + Codex together), which consistently produces one-shot correct implementations with full test coverage.


## @JasonrShuman - "Do It For Me" Economy: AI Installers Will Beat SaaS Vendors for SMBs
> Silicon Valley thinks AI agents are a $20/mo self-serve subscription.
>
> Main Street is paying local agencies $10,000 just to turn them on.
>
> Everyone assumes AI will be bought primarily online like Slack or Zoom. I think they are wrong.
>
> Some of the biggest winners in the AI boom won't be the software vendors. It will be the humans installing it.
>
> Here is the reality of SMBs right now:
> • 54% lack internal AI expertise.
> • 41% have data quality too poor for AI to even work.
> • 41% already prefer buying AI through a local IT provider.
>
> You cannot "1-click install" a genius AI into a messy CRM or a 15-year-old server. It will just execute the wrong tasks at the speed of light.
>
> The AI software will be cheap and a lot will absolutely be bought online. Making it actually work for a messy, real-world business will be expensive.
>
> Very bullish on the "Do It For Me" economy being back.

- **Tweet:** https://x.com/JasonrShuman/status/2036603049729466700
- **What:** Argument that the biggest AI winners for SMBs won't be software vendors but human integrators — because 54% of small businesses lack AI expertise and 41% already prefer buying through local IT providers, making professional installation services worth $10k+ even when the software itself is cheap.


## @amirmxt - Google Ads Campaign Management via Claude Cowork + MCP
> austin run's anthropics growth
>
> great breakdown on how he runs his campaigns with dispatch:
>
> - custom claude cowork plugin that connects directly to the google ads API via MCP
> - basically encodes his entire paid search workflow into reusable skills [...]
> - full campaign management loops from a single interface - desktop and phone
>
> *Quoting @helloitsaustin:* if you're a performance marketer, here's how I use a custom Claude Cowork plugin to manage Google Ads at @AnthropicAI. it connects to the Google Ads API via MCP, encodes my common paid search workflows into skills, and works on desktop and Dispatch.

- **Tweet:** https://x.com/amirmxt/status/2036591977177776466
- **Quoted:** https://x.com/helloitsaustin/status/2036553581625745511
- **What:** Breakdown of how Anthropic's growth team runs Google Ads management through Claude Cowork — a custom MCP plugin queries campaigns via GAQL, evaluates search terms, outputs audit CSVs with reasoning columns, and can apply changes (like negatives) directly from chat on desktop or Dispatch mobile.


## @iamsupersocks - Anthropic Engineering: Multi-Agent Harness for Long-Running Autonomous Apps
> Anthropic explique comment faire bosser Claude en autonomie pendant des heures et le concept clé à retenir s'appelle le "harness". Un harness, c'est l'architecture qui entoure le modèle : les agents, les règles, les boucles de feedback. C'est pas le modèle lui-même, c'est le système qu'on construit autour pour le faire performer. [...] L'espace des possibles ne rétrécit pas, il bouge.
>
> *Quoting @AnthropicAI:* New on the Anthropic Engineering Blog: How we use a multi-agent harness to push Claude further in frontend design and long-running autonomous software engineering. Read more: https://t.co/HWvmXk1ykn

- **Tweet:** https://x.com/iamsupersocks/status/2036504448621511070
- **Link:** https://www.anthropic.com/engineering/harness-design-long-running-apps
- **Quoted:** https://x.com/AnthropicAI/status/2036481033621623056
- **What:** French-language thread summarizing Anthropic's engineering blog post on multi-agent harnesses — covering the two core failure modes of solo agents (context drift and inability to self-evaluate) and how a producer/evaluator architecture with separate critic agents dramatically improves output quality in frontend and full-app development tasks.


## @imakeBADads - AI Infrastructure Consulting Opportunity for Mid-Market Companies
> Every day I turn down companies offering me $100k+ to build them AI infrastructure.
>
> They know they lack the expertise, but they don't want to blow their cash hiring engineers that will drain them.
>
> They'd rather pay someone a bag to:
>
> - Build it in 1-3 months
> - Save them 5-6 figures/mo
>
> You could literally spin up a new business and build everything under this service.
>
> That's how big this opportunity is.
>
> *Quoting @damianplayer:* the biggest AI opportunity right now is mid-market companies ($5M-$50M+ revenue): • too big for cookie-cutter solutions • too small for enterprise consulting • drowning in manual workflows • have budget but zero AI expertise (most companies) they're stuck with serious cash but frozen by AI paralysis. markets open to those with balls & a cold email sequence.

- **Tweet:** https://x.com/imakeBADads/status/2036481725950263628
- **Quoted:** https://x.com/damianplayer/status/2033909532921933877
- **What:** Quote-amplifying the thesis that mid-market companies ($5M–$50M revenue) are the biggest underserved AI opportunity — they have budget but lack expertise, and are willing to pay consultants $100k+ to build and maintain their AI infrastructure.


## @shannholmberg - Auto-Improving Claude Skills with Karpathy's Autoresearch Loop

> Karpathy's AutoResearch is changing how campaigns get optimized and most marketers haven´t heard of it yet.
>
> Ole Lehmann tested it on landing page copy, 56% → 92% pass rate overnight.
>
> here´s how it works for marketing / skills 🧵 https://t.co/99RvkfrcO1
>
> *Quoting @itsolelehmann:* https://t.co/kgo8wNoiDv

- **Tweet:** https://x.com/shannholmberg/status/2036461256006357409
- **Link:** https://x.com/i/article/2033576301383061504
- **What:** An X article by Ole Lehmann explaining how to apply Andrej Karpathy's "autoresearch" method to auto-improve Claude skill prompts via an agent loop — define a yes/no checklist of quality criteria, run the skill, score the output, mutate the prompt, repeat until it hits 95%+ pass rate. A landing page copy skill went from 56% to 92% pass rate with zero manual intervention.


## @BonesawMD - Bullish Take on AI Job Displacement as Path to Intellectual Renaissance

> I'm probably one of the few people who is happy to see people steadily have their jobs replaced by AI like this.
>
> Some days I salivate shamelessly if I think of it too much.
>
> Most jobs are filler & LARP.
> Made up and unnecessary.
>
> If you watch people work, you realise hardly anybody does anything and often they do it poorly anyway.
>
> I don't blame them. Why pour your blood, sweat, and tears into companies that don't value you, harvest your creative energy, and drain your life force?
>
> Many people reading this secretly know they're getting paid to do nothing for more than 85% of their 'working' day.
>
> Great civilisations of the past such as Ancient Greece could advance fields like geometry, philosophy, art, music, and engineering so immensely because people had idle time to think –– they didn't waste their entire day and peak consciousness pretending to be busy, doing mundane non-life affirming tasks.
>
> It'll look much worse until it gets better, but we may see an intellectual boom in our lifetime. An entire new economic landscape that rewards creativity and up-skilling.
>
> I am so bullish it's unreal.
>
> *Quoting @claudeai:* You can now enable Claude to use your computer to complete tasks.
>
> It opens your apps, navigates your browser, fills in spreadsheets—anything you'd do sitting at your desk.
>
> Research preview in Claude Cowork and Claude Code, macOS only.

- **Tweet:** https://x.com/BonesawMD/status/2036430427234209846
- **What:** An optimistic philosophical take on AI-driven job displacement — arguing that most jobs are low-value busywork, and that freeing people from them (as Claude's new computer-use feature accelerates) could trigger an intellectual boom analogous to ancient Greece, where idle time enabled great advances. Prompted by Anthropic's computer-use research preview announcement.


## @yacineMTB - Entry Path into AI: Karpathy's Backprop Videos + PufferLib

> if you are interested in getting into AI, the best way today is to start with karpathy's videos on backprop/gradient descent and then get pufferlib (puffer dot ai) and start training models

- **Tweet:** https://x.com/yacineMTB/status/2036302350265020509
- **What:** A concise on-ramp recommendation for AI beginners: start with Andrej Karpathy's backprop/gradient descent video series to build intuition, then move to PufferLib (puffer.ai) to begin hands-on reinforcement learning model training.


## @oprydai - SBA Waiving Loan Fees for US Manufacturers in FY2026

> i'm telling you. if you are in software, pivot to hardware.
>
> *Quoting @SBAgov:* 📢 NO LOAN FEES FOR U.S. MANUFACTURERS!
>
> In FY2026, SBA is waiving upfront fees for small manufacturers.
>
> These include:
> ✅ 0% upfront fee for 7(a) manufacturing loans of up to $950,000
> ✅ 0% upfront fee and annual service fee for all 504 manufacturing loans
>
> Connect with a lender today! https://t.co/2WEDrqNTfv

- **Tweet:** https://x.com/oprydai/status/2036301830318334372
- **Link:** https://www.sba.gov/funding-programs/loans/lender-match-connects-you-lenders
- **What:** The SBA is waiving upfront loan fees for small US manufacturers in FY2026 — 0% fees on 7(a) manufacturing loans up to $950K and 0% fees on all 504 manufacturing loans. The author uses this as a prompt to encourage software folks to pivot to hardware.


## @heynavtoor - OpenAI Parameter Golf: Train a <16MB Language Model for $1M in Compute

> 🚨 PhD students are panicking. OpenAI just told the world: we don't care about your degree. Build the best AI model under 16MB and we'll find you.
>
> That's smaller than one photo on your phone.
>
> It's called Parameter Golf.
>
> Train the smartest language model you can. It must fit in 16 megabytes. You get 10 minutes on 8xH100 GPUs. Lowest score wins.
>
> OpenAI is backing it with $1,000,000 in free compute credits.
>
> No resume. No interview. No PhD required. Just build.
>
> Here's what's inside this thing:
>
> → A public leaderboard where anyone can submit
> → Competitors beating each other's scores within hours
> → Architectures nobody has ever tried before
> → The baseline scored 1.2244. In 3 days it dropped to 1.1428. Still falling.
> → 236 pull requests. 1,500 forks. The leaderboard changes every few hours.
>
> Here's the wildest part:
>
> Top performers get noticed by OpenAI researchers and recruiters directly. No application. No hiring pipeline. Your model IS your resume.
>
> AIs labs spend millions recruiting through conferences and university pipelines. OpenAI just replaced all of that with a single GitHub repo.
>
> Challenge runs until April 30th. Everything is public.
>
> 3.1K GitHub stars. MIT License.
>
> 100% Open Source.

- **Tweet:** https://x.com/heynavtoor/status/2036295451234984150
- **What:** OpenAI's "Parameter Golf" challenge — a public competition to train the best language model that fits within 16MB, with $1M in free compute credits as backing and a public leaderboard running until April 30, 2026. Top performers get recruited directly by OpenAI researchers without a traditional application process.


## @Shpigford - Shpigford/skills: Agent Skills Collection for AI Coding Assistants
> *Replying to @richiemcilroy:* just over a month ago we ripped out Intercom from @Cap and replaced it with our own in-house version. took half a day to implement, saving over $3k/yr.
>
> @richiemcilroy @cap Yasss. I did this so many times I turned it in to a /skill that you can run in your app repo and it'll build the whole thing for you!

- **Tweet:** https://x.com/Shpigford/status/2036632676950474838
- **Parent:** https://x.com/richiemcilroy/status/2036494709372100958
- **Filed:** [shpigford-skills](./knowledge/tools/shpigford-skills.md)
- **What:** Josh Pigford's collection of 10 agent skills (150 stars) compatible with Claude Code, Cursor, Gemini Code Assist, and GitHub Copilot — covers chat widget builds, Rails project setup, favicon generation, marketing screenshots, READMEs, and a skeptical self-review pass.

## @amirmxt - Google Ads Campaign Management via Claude Cowork + Google Ads MCP
> austin run's anthropic's growth
>
> great breakdown on how he runs his campaigns with dispatch: custom claude cowork plugin connecting directly to the Google Ads API via MCP — skills for search term mining, budget optimization, and weekly reviews; GAQL queries that output CSV with reasoning column per flag; adding negatives right from chat; extends to Dispatch on mobile.
>
> *Quoting @helloitsaustin:* if you're a performance marketer, here's how I use a custom Claude Cowork plugin to manage Google Ads at @AnthropicAI. it connects to the Google Ads API via MCP, encodes my common paid search workflows into skills, and works on desktop and Dispatch.

- **Tweet:** https://x.com/amirmxt/status/2036591977177776466
- **Quoted:** https://x.com/helloitsaustin/status/2036553581625745511
- **What:** Breakdown of how Anthropic's growth team uses Claude Cowork with a custom Google Ads MCP plugin — connects directly to the API via GAQL, encodes paid search workflows as reusable skills, outputs auditable CSVs with per-flag reasoning columns, and manages campaigns from mobile via Dispatch.

## @itsolelehmann - Detox Your Claude Setup: Self-Audit Prompt to Cut Dead Weight Rules
> *[X article: "Your Claude setup rots over time. Detox it in 60 seconds (with this self-audit prompt)"]*

- **Tweet:** https://x.com/itsolelehmann/status/2036533756572639611
- **Link:** https://x.com/i/article/2036433375150354432
- **What:** Ole Lehmann argues accumulated CLAUDE.md rules degrade output quality — shares a copy-paste self-audit prompt where Claude reads its own entire setup and flags redundant, conflicting, or overly specific rules; also shows how to automate weekly audits via Cowork's built-in scheduling.

## @iruletheworldmo - The Claude Dispatch Guide: 48 Hours Running AI From Your Phone
> if you haven't tried dispatch yet you need to wake up
>
> this guide will see you free
>
> it's a must read. must bookmark.
>
> *Quoting @PawelHuryn:* [The Claude Dispatch Guide: 48 Hours Running AI From My Phone — testing all 4 Claude mobile surfaces, real PM async workflows, gotchas with folder access and file transfer, and why a GitHub-backed knowledge layer compounds across all surfaces]

- **Tweet:** https://x.com/iruletheworldmo/status/2036368407369506840
- **Quoted:** https://x.com/PawelHuryn/status/2036058594433519790
- **Link:** https://x.com/i/article/2036056172810096640
- **What:** Endorsement of Paweł Huryn's 48-hour Dispatch test — covers setup, real PM async workflows (directing work from a bounce house sideline), gotchas, and why building a GitHub-backed knowledge layer (CLAUDE.md + skills) compounds across all Claude surfaces.

## @shannholmberg - Karpathy's AutoResearch for Marketing Campaign Optimization
> Karpathy's AutoResearch is changing how campaigns get optimized and most marketers haven't heard of it yet.
>
> Ole Lehmann tested it on landing page copy, 56% → 92% pass rate overnight.
>
> here's how it works for marketing / skills

- **Tweet:** https://x.com/shannholmberg/status/2036461256006357409
- **Quoted:** https://x.com/itsolelehmann/status/2033919415771713715
- **What:** Overview of Karpathy's autoresearch method applied to Claude skill improvement and marketing optimization, demonstrating dramatic pass rate increases on landing page copy testing.

## @imakeBADads - The AI Infrastructure Consulting Opportunity
> Every day I turn down companies offering me $100k+ to build them AI infrastructure.
>
> They know they lack the expertise, but they don't want to blow their cash hiring engineers that will drain them.
>
> They'd rather pay someone a bag to:
>
> - Build it in 1-3 months
> - Save them 5-6 figures/mo
>
> You could literally spin up a new business and build everything under this service.
>
> That's how big this opportunity is.
>
> *Quoting @damianplayer:* the biggest AI opportunity right now is mid-market companies ($5M-$50M+ revenue): too big for cookie-cutter solutions, too small for enterprise consulting, drowning in manual workflows, have budget but zero AI expertise. They're stuck with serious cash but frozen by AI paralysis.

- **Tweet:** https://x.com/imakeBADads/status/2036481725950263628
- **Quoted:** https://x.com/damianplayer/status/2033909532921933877
- **What:** Commentary on the massive opportunity for AI infrastructure consulting services targeting mid-market companies seeking quick implementation without long-term engineering hires.

## @iamsupersocks - Anthropic's Multi-Agent Harness for Long-Running Apps
> Anthropic explique comment faire bosser Claude en autonomie pendant des heures et le concept clé à retenir s'appelle le "harness".
>
> Un harness, c'est l'architecture qui entoure le modèle : les agents, les règles, les boucles de feedback. C'est pas le modèle lui-même, c'est le système qu'on construit autour pour le faire performer.
>
> La solution : ne jamais laisser un agent se noter lui-même.
>
> L'équipe sépare le boulot en deux rôles distincts. Un agent qui produit, un autre qui évalue. Pour le frontend, l'évaluateur navigue la page en live via Playwright et itère 5-15 fois. Pour les apps complètes: trois agents (planificateur, développeur, testeur). Résultat après 6 heures: app complète avec sprites, niveaux jouables, et génération IA.
>
> *Quoting @AnthropicAI:* New on the Anthropic Engineering Blog: How we use a multi-agent harness to push Claude further in frontend design and long-running autonomous software engineering. Read more: https://t.co/HWvmXk1ykn

- **Tweet:** https://x.com/iamsupersocks/status/2036504448621511070
- **Quoted:** https://x.com/AnthropicAI/status/2036481033621623056
- **Filed:** [anthropic-harness-design-long-running-apps](./knowledge/articles/anthropic-harness-design-long-running-apps.md)
- **What:** French-language thread summarizing Anthropic's engineering approach to multi-agent harnesses that enable Claude to work autonomously for hours, using separate producer/evaluator agents inspired by GANs.

## @JasonrShuman - The "Do It For Me" Economy: Local AI Installation
> Silicon Valley thinks AI agents are a $20/mo self-serve subscription.
>
> Main Street is paying local agencies $10,000 just to turn them on.
>
> Everyone assumes AI will be bought primarily online like Slack or Zoom. I think they are wrong.
>
> Some of the biggest winners in the AI boom won't be the software vendors. It will be the humans installing it.
>
> Here is the reality of SMBs right now:
> • 54% lack internal AI expertise.
> • 41% have data quality too poor for AI to even work.
> • 41% already prefer buying AI through a local IT provider.
>
> You cannot '1-click install' a genius AI into a messy CRM or a 15-year-old server. It will just execute the wrong tasks at the speed of light.
>
> The AI software will be cheap and a lot will absolutely be bought online. Making it actually work for a messy, real-world business will be expensive.
>
> Very bullish on the 'Do It For Me' economy being back.

- **Tweet:** https://x.com/JasonrShuman/status/2036603049729466700
- **What:** Analysis of the AI distribution gap between Silicon Valley SaaS expectations and Main Street reality, arguing that local implementation services and "Do It For Me" consulting will be major value captures in the AI boom.

## @BonesawMD - AI Job Replacement as Path to Intellectual Boom
> I'm probably one of the few people who is happy to see people steadily have their jobs replaced by AI like this.
>
> Some days I salivate shamelessly if I think of it too much.
>
> Most jobs are filler & LARP.
> Made up and unnecessary.
>
> If you watch people work, you realise hardly anybody does anything and often they do it poorly anyway.
>
> I don't blame them. Why pour your blood, sweat, and tears into companies that don't value you, harvest your creative energy, and drain your life force?
>
> Many people reading this secretly know they're getting paid to do nothing for more than 85% of their 'working' day.
>
> Great civilisations of the past such as Ancient Greece could advance fields like geometry, philosophy, art, music, and engineering so immensely because people had idle time to think.
>
> It'll look much worse until it gets better, but we may see an intellectual boom in our lifetime. An entire new economic landscape that rewards creativity and up-skilling.
>
> I am so bullish it's unreal.
>
> *Quoting @claudeai:* You can now enable Claude to use your computer to complete tasks. It opens your apps, navigates your browser, fills in spreadsheets—anything you'd do sitting at your desk. Research preview in Claude Cowork and Claude Code, macOS only.

- **Tweet:** https://x.com/BonesawMD/status/2036430427234209846
- **Quoted:** https://x.com/claudeai/status/2036195789601374705
- **What:** Bonesaw argues that AI job displacement could enable an intellectual boom by freeing people from meaningless work, allowing society to focus on creativity and meaningful pursuits like ancient civilizations did.

## @oprydai - Pivot to Hardware for Software Engineers
> i'm telling you. if you are in software, pivot to hardware.
>
> *Quoting @SBAgov:* 📢 NO LOAN FEES FOR U.S. MANUFACTURERS! In FY2026, SBA is waiving upfront fees for small manufacturers. These include: 0% upfront fee for 7(a) manufacturing loans of up to $950,000. 0% upfront fee and annual service fee for all 504 manufacturing loans.

- **Tweet:** https://x.com/oprydai/status/2036301830318334372
- **Quoted:** https://x.com/SBAgov/status/2036087345506574830
- **What:** Mustafa suggests software engineers should consider pivoting to hardware, highlighting new government financing opportunities for small manufacturers with waived upfront fees.

## @heynavtoor - OpenAI Parameter Golf Competition with $1M in Compute
> 🚨 PhD students are panicking. OpenAI just told the world: we don't care about your degree. Build the best AI model under 16MB and we'll find you.
>
> That's smaller than one photo on your phone.
>
> It's called Parameter Golf.
>
> Train the smartest language model you can. It must fit in 16 megabytes. You get 10 minutes on 8xH100 GPUs. Lowest score wins.
>
> OpenAI is backing it with $1,000,000 in free compute credits.
>
> No resume. No interview. No PhD required. Just build.
>
> → A public leaderboard where anyone can submit
> → Competitors beating each other's scores within hours
> → Architectures nobody has ever tried before
> → The baseline scored 1.2244. In 3 days it dropped to 1.1428. Still falling.
> → 236 pull requests. 1,500 forks. The leaderboard changes every few hours.
>
> Top performers get noticed by OpenAI researchers and recruiters directly. No application. No hiring pipeline. Your model IS your resume.
>
> 3.1K GitHub stars. MIT License. 100% Open Source.

- **Tweet:** https://x.com/heynavtoor/status/2036295451234984150
- **What:** OpenAI launched Parameter Golf, a competition to build the smartest language model under 16MB with $1M in free GPU compute credits, disrupting traditional hiring by using model performance as the sole qualification.

---

---

# Monday, March 23, 2026

## @aaronjmars - Maximizing Claude Pro/Max with Rate-Limit Window Optimization via Aeon

> holy shit, found the best way to maximize 100% your Claude Pro/Max subscription
>
> rate-limits works on a 5h window & reset after that
> anthropic have an API endpoint using your Claude Code API key : GET /api/oauth/usage
> built a SKILL for aeon (github dot com/aaronjmars/aeon) that monitors when my 5h window is about to ends
> if there is less than 30mn left on my windows, it trigger all my scheduled skills (fix PRs, do research etc) until I reach my 100% limit
>
> the optimizoooor

- **Tweet:** https://x.com/aaronjmars/status/2036230574822580675
- **What:** A technique using the Anthropic OAuth usage API endpoint to track the 5-hour rate-limit window on Claude Pro/Max subscriptions, triggering scheduled background tasks (via the aeon tool) whenever less than 30 minutes remain in the window to maximize utilization.


## @MattEpstein16 - Reaction to Free AI Tool Capability Demonstration
> Absouloutly fucked that this is free
> *Quoting @MitcheIl:* https://t.co/1AX8svq17s

- **Tweet:** https://x.com/MattEpstein16/status/2036160818056683678
- **Link:** https://x.com/i/article/2035101919669362688
- **What:** A viral reaction tweet (with video) to Mitchell's article demonstrating a free AI tool or capability that Matt Epstein found remarkably impressive — the caption expresses disbelief that something this powerful is available at no cost.


## @om_patel5 - Software Engineers Reacting to AI Coding Agent Article
> software engineers right now:
> *Quoting @akshay_pachaar:* https://t.co/SSSIK3BX4z

- **Tweet:** https://x.com/om_patel5/status/2036114160518406157
- **Link:** https://x.com/i/article/2034961967149195264
- **What:** A humorous reaction tweet (with an attached image/meme) pointing to Akshay Pachaar's article on AI-assisted engineering workflows, commenting on how software engineers are feeling about the current state of AI coding agents.


## @806texasgrl - SBA Waiving Upfront Loan Fees for U.S. Small Manufacturers in FY2026
> FAMILY, go get your bread. Better yet, set up a business making healthy bread. The Small Business Admin is looking to give out money & not for opening a "Learing center"
> *Quoting @SBAgov:* 📢 NO LOAN FEES FOR U.S. MANUFACTURERS!

In FY2026, SBA is waiving upfront fees for small manufacturers.

These include:
✅ 0% upfront fee for 7(a) manufacturing loans of up to $950,000
✅ 0% upfront fee and annual service fee for all 504 manufacturing loans

Connect with a lender today!

- **Tweet:** https://x.com/806texasgrl/status/2036112233382682816
- **Link:** https://www.sba.gov/funding-programs/loans/lender-match-connects-you-lenders
- **What:** The SBA announced it is waiving all upfront fees for small U.S. manufacturers in FY2026, covering both 7(a) loans up to $950K and all 504 manufacturing loans, with a lender-matching tool available at sba.gov.


## @Argona0x - Splitting Monorepo CLAUDE.md into Scoped Subdirectory Files Boosts Rule Adherence
> i mass-configured 4 repos using this exact folder structure last week

cut my debugging time by ~60% and saved roughly $2,400 in dev hours

the rules/ folder alone is worth the entire guide

but the post doesn't mention what actually breaks without this

i had a 1,200-line CLAUDE.md in a monorepo. claude was ignoring 40% of my instructions. instruction adherence drops off a cliff past **300 lines** – general consensus confirms <300 lines is best to avoid context bloat in every session

splitting it fixed everything:

→ root CLAUDE.md down to 60 lines (project overview + essential commands only)
→ /backend/CLAUDE.md scoped with biome auto-fix rules hitting 85% lint coverage on access
→ /frontend/CLAUDE.md loads zustand store patterns only when editing that dir
→ context bloat reduced 70-80% because claude auto-pulls nested CLAUDE.md per directory instead of swallowing everything at once

rule adherence went from ~60% to **95%** – matching production benchmarks where **progressive disclosure + CLAUDE.md <150 instructions** boosts reliability via evaluation-driven dev

i went from 3 junior contractors reviewing claude outputs at $80/hr to just me.

110 fewer hours a month of someone squinting at code claude already got right

the real unlock is understanding that claude runs **`head -100` previews on nested refs** (avoiding deeply nested chains that cause incomplete reads) and fully reads flat subdir CLAUDE.md files on access – keep refs **one level deep from root** per official docs

most people will read this thread and still keep their 500-line CLAUDE.md

that's fine. less competition
> *Quoting @akshay_pachaar:* https://t.co/SSSIK3BX4z

- **Tweet:** https://x.com/Argona0x/status/2036106517678624820
- **Link:** https://x.com/i/article/2034961967149195264
- **What:** A practitioner's report on splitting a 1,200-line monorepo CLAUDE.md into scoped per-directory files (root + /backend + /frontend), achieving a jump from ~60% to 95% instruction adherence — with the key insight that Claude reads nested CLAUDE.md files lazily and only when entering that directory, so keeping each file under 300 lines prevents context bloat.


## @itsolelehmann - Audit Your Claude Setup with a Single Prompt to Remove Conflicting Rules
> i deleted half my Claude setup last week and every output got BETTER

sounds backwards, but anthropic's own team just explained exactly why it works.

here's the one prompt that tells you what to cut (and you don't even have to paste anything):

this is what happens to everyone...

you get a bad output, so you add a rule to your skills. "be more concise."

next week, another bad output. another rule. "use a casual tone."

but a month later, something else breaks. "always explain technical terms."

you keep stacking, and it feels productive because you're fixing problems as they come up.

but 3 months in, you've got 30 rules piled on top of each other.

some of them contradict each other ("be concise" and "always explain your reasoning" are fighting).

some of them fix problems that the model doesn't even have anymore.

and the model is trying to follow all of them at once, which means it's doing none of them well.

it's like handing a chef a 47-step recipe when they only need 12.

the extra 35 steps slow the chef down, make them second-guess the parts they already know, and the dish comes out worse than if you'd just let them cook.

that's what over-prompting does.

anthropic just published a piece on how they build claude code (the ai coding agent).

their own engineering team found that their scaffolding was making the ai worse

which means your custom instructions are almost certainly doing the same thing.

so here's the actionable move...

instead of manually reading through your setup line by line, just tell claude to audit itself.

if you're in claude's desktop app, claude already has access to your:

claude[.]md (the file where your preferences and rules live), your skills folder (where your reusable instruction files are stored), your context files, everything.

just open claude code/cowork and say this:

—

"read my entire setup before responding. check my claude .md, every skill in my skills folder, every file in my context folder, and any other instruction files you can find.

then go through every rule, instruction, and preference you found. for each one, tell me:

1. is this something you already do by default without being told?
2. does this contradict or conflict with another rule somewhere else in my setup?
3. does this repeat something that's already covered by a different rule or file?
4. does this read like it was added to fix one specific bad output rather than improve outputs overall?
5. is this so vague that you'd interpret it differently every time? (ex: 'be more natural' or 'use a good tone')

then give me a list of everything you'd cut with a one-line reason for each, a list of any conflicts you found between files, and a cleaned up version of my claude.md with the dead weight removed."

—

one message. claude goes and reads your entire setup, audits it, and comes back with exactly what to cut and why.

you don't dig through files, you don't read every rule yourself. it does the whole thing.

once you get the results, don't just blindly delete everything it flags.

here's the process:

1. read what it flagged and why
2. delete the flagged rules
3. run your 3 most common tasks with the trimmed setup
4. did the output stay the same or get better? the deleted rules were dead weight
5. did something specific break? add back just that one rule

the goal is to find the minimum viable setup that gets you the output you want.

your ai setup should be getting simpler over time.

addition by subtraction baby

- **Tweet:** https://x.com/itsolelehmann/status/2036065138147471665
- **What:** A detailed thread arguing that accumulated Claude custom instructions become self-defeating over time through contradictions and redundancy, with a specific self-audit prompt you can run inside Claude Code to identify and prune dead-weight rules — inspired by Anthropic's own finding that their scaffolding was degrading Claude Code's output quality.


## @PrajwalTomar_ - 3-Layer Agent Harness for Non-Designers to Ship Complete UI
> This engineer couldn't do design.

So he built a 3-layer agent harness and now he ships complete designs. Pixels, spacing, typography, everything.

If design is blocking your MVP, read this.
> *Quoting @neethanwu:* https://t.co/z7p1rL84KV

- **Tweet:** https://x.com/PrajwalTomar_/status/2036013596719960561
- **Link:** https://x.com/i/article/2034424000588152833
- **What:** Neethan Wu's article describes building a multi-layer AI agent pipeline that handles the full design workflow — layout, spacing, typography — allowing engineers without design skills to ship polished UIs without a designer.


## @mattpocockuk - Claude Code for Real Engineers Cohort Course
> Folks who looked at my Claude Code cohort and didn't buy it:

What stopped you?

All feedback is a gift. The more brutal, the better.

- **Tweet:** https://x.com/mattpocockuk/status/2036010331370111340
- **Link:** https://www.aihero.dev/cohorts/claude-code-for-real-engineers-2026-04
- **What:** Matt Pocock is running a paid cohort called "Claude Code for Real Engineers" on aihero.dev, soliciting candid feedback from people who considered buying but didn't — essentially market research to improve or reprice the offering.


## @aakashgupta - Karpathy's Locked Eval Architecture as the Template for AI-Augmented Organizations
> Karpathy accidentally shipped the org chart for every AI-augmented company in 2030.
>
> Three files. program.md is the human writing strategy in plain English. https://t.co/rrgrQfMOGG is the agent executing, iterating, and shipping code. https://t.co/zkuCCCk43j is the locked evaluation layer that neither the human nor the agent can touch mid-run.
>
> That third file is the one worth studying.
>
> In most companies deploying AI agents today, the person who sets the goal also controls how success is measured. The marketing team picks the KPI, runs the campaign, and reports the results. The PM defines the metric, ships the feature, and presents the dashboard. The incentive to subtly shift the goalposts is built into the structure.
>
> Karpathy separated goal-setting from evaluation by making https://t.co/zkuCCCk43j immutable. The agent optimizes val_bpb. The agent cannot redefine val_bpb. The agent cannot swap in a friendlier dataset. The agent cannot adjust the tokenizer to make its numbers look better. It either improved on the locked metric or it gets reverted. No narrative. No context. No "well, if you look at it this way."
>
> That's why the results held. 700 experiments, 20 kept, and when Karpathy applied those 20 improvements to a model twice the size, every single one transferred. The gains were real because the agent had zero ability to make fake gains look real.
>
> Shopify's CEO ran the same architecture overnight. 37 experiments, 19% quality improvement, smaller model beating a larger one. The pattern transferred because the evaluation was trustworthy.
>
> Now scale the principle. A sales team where the AI agent writes outbound sequences, an independent system scores reply quality, and a human sets the targeting criteria. A product team where the agent ships variants, a locked analytics pipeline measures retention, and a PM writes the experiment brief. A recruiting team where the agent screens candidates, a calibrated rubric scores them, and a hiring manager defines the role.
>
> The separation Karpathy built into 630 lines of Python is the same separation every company will need when agents do the execution. Whoever controls the eval controls the outcome. Lock it down or the agent will find the shortest path to a number that means nothing.
>
> *Quoting @aakashgupta:* For $25 and a single GPU, you can now run 100 experiments overnight without designing any of them.
>
> Karpathy open-sourced autoresearch. 42,000 GitHub stars in a week. Fortune called it "The Karpathy Loop."
>
> Every article about it focused on the ML angle. They all missed the bigger story. The pattern underneath works on anything you can score with a number. Ad copy, cold emails, video scripts, job posts, skill files.
>
> Three files. One the agent edits. One it can never touch. One instruction file from you. Each cycle takes 5 minutes. Score went up? Git commit. Score went down? Git reset. Twelve cycles per hour. A hundred overnight.
>
> Karpathy ran it on code he'd already optimized by hand for months. The agent found 20 improvements he'd missed. 11% faster. Tobi Lutke pointed it at Shopify's Liquid templating engine. 53% faster rendering from 93 automated commits.
>
> I spent two weeks pulling the system apart. Today's guide shows you how to use it on the things you actually make every day. Six use cases, the three-step setup, and the eval mistakes that kill runs before they start.
>
> Full guide: https://t.co/CbJSXRXRKh

- **Tweet:** https://x.com/aakashgupta/status/2036006034729304175
- **Link:** https://www.aibyaakash.com/p/autoresearch-guide
- **Filed:** [Autoresearch Guide: Karpathy's Locked Eval as Org Design](./knowledge/articles/autoresearch-guide-karpathy-eval-org-design.md)
- **What:** Deep analysis arguing that Karpathy's autoresearch three-file architecture (editable code, locked eval, human strategy) is the template for every AI-augmented organization — the separation of execution from evaluation is what makes results trustworthy at scale.


## @saakohl - Latent-Y: First Autonomous Agent for Lab-Validated Drug Design
> Today we're launching Latent-Y: the world's first autonomous agent for drug design, lab-validated end to end.
>
> Give it a research goal. Latent-Y reasons, designs, iterates, and delivers lab-ready antibodies, autonomously or collaboratively, with the biological reasoning of a PhD protein design expert.
>
> Technical report: https://t.co/E7IHfkvvD3
> Blog post: https://t.co/GfJAfzj0Qx
> Apply for access: https://t.co/E0SR9znZiP

- **Tweet:** https://x.com/saakohl/status/2035988968764788938
- **Link:** https://www.latentlabs.com/latent-y/
- **Filed:** [Latent-Y: Autonomous Drug Design Agent](./knowledge/articles/latent-y-drug-design-agent.md)
- **What:** Latent Labs launches Latent-Y, an autonomous AI agent for antibody and drug design that takes a research goal and delivers lab-ready results, claiming to be the first fully lab-validated end-to-end autonomous drug design system.


## @saakohl - Latent-Y: Autonomous Drug Design Agent
> Today we're launching Latent-Y: the world's first autonomous agent for drug design, lab-validated end to end.
>
> Give it a research goal. Latent-Y reasons, designs, iterates, and delivers lab-ready antibodies, autonomously or collaboratively, with the biological reasoning of a PhD protein design expert.
>
> Technical report: https://t.co/E7IHfkvvD3
> Blog post: https://t.co/GfJAfzj0Qx
> Apply for access: https://t.co/E0SR9znZiP

- **Tweet:** https://x.com/saakohl/status/2035988968764788938
- **What:** Latent Labs announced Latent-Y, an AI agent that autonomously designs and lab-validates antibodies and other biologics. It operates like a PhD-level protein design expert and can work autonomously or in collaboration with human researchers.

## @aakashgupta - Karpathy's Autoresearch and the Immutable Evaluation Layer
> Karpathy accidentally shipped the org chart for every AI-augmented company in 2030.
>
> Three files. program.md is the human writing strategy in plain English. train.py is the agent executing, iterating, and shipping code. val_bpb is the locked evaluation layer that neither the human nor the agent can touch mid-run.
>
> That third file is the one worth studying.
>
> In most companies deploying AI agents today, the person who sets the goal also controls how success is measured. The marketing team picks the KPI, runs the campaign, and reports the results. The PM defines the metric, ships the feature, and presents the dashboard. The incentive to subtly shift the goalposts is built into the structure.
>
> Karpathy separated goal-setting from evaluation by making val_bpb immutable. The agent optimizes val_bpb. The agent cannot redefine val_bpb. The agent cannot swap in a friendlier dataset. The agent cannot adjust the tokenizer to make its numbers look better. It either improved on the locked metric or it gets reverted. No narrative. No context. No 'well, if you look at it this way.'
>
> That's why the results held. 700 experiments, 20 kept, and when Karpathy applied those 20 improvements to a model twice the size, every single one transferred. The gains were real because the agent had zero ability to make fake gains look real.
>
> Shopify's CEO ran the same architecture overnight. 37 experiments, 19% quality improvement, smaller model beating a larger one. The pattern transferred because the evaluation was trustworthy.
>
> The separation Karpathy built into 630 lines of Python is the same separation every company will need when agents do the execution. Whoever controls the eval controls the outcome. Lock it down or the agent will find the shortest path to a number that means nothing.
>
> *Quoting @aakashgupta:* For $25 and a single GPU, you can now run 100 experiments overnight without designing any of them. Karpathy open-sourced autoresearch. 42,000 GitHub stars in a week. Fortune called it 'The Karpathy Loop.' Three files. One the agent edits. One it can never touch. One instruction file from you. Each cycle takes 5 minutes. Score went up? Git commit. Score went down? Git reset. Twelve cycles per hour. A hundred overnight.

- **Tweet:** https://x.com/aakashgupta/status/2036006034729304175
- **Quoted:** https://x.com/aakashgupta/status/2034851259442749909
- **What:** Aakash Gupta explains how Karpathy's autoresearch framework—with its immutable evaluation layer—provides a blueprint for AI-augmented organizations. The locked evaluation prevents agents and humans from gaming metrics, ensuring genuine improvements. The pattern applies across sales, product, recruiting, and engineering.

## @mattpocockuk - Claude Code Cohort Feedback Request
> Folks who looked at my Claude Code cohort and didn't buy it:
>
> What stopped you?
>
> All feedback is a gift. The more brutal, the better.
>
> https://t.co/Ur0ebWlIRl

- **Tweet:** https://x.com/mattpocockuk/status/2036010331370111340
- **What:** Matt Pocock asking for feedback from people who viewed his Claude Code cohort landing page but didn't purchase. The cohort is a paid educational program about using Claude Code for development.

## @aaronjmars - Maximizing Claude Pro/Max with Rate-Limit Monitoring Skill
> holy shit, found the best way to maximize 100% your Claude Pro/Max subscription
>
> > rate-limits works on a 5h window & reset after that
> > anthropic have an API endpoint using your Claude Code API key : GET /api/oauth/usage
> > built a SKILL for aeon (github dot com/aaronjmars/aeon) that monitors when my 5h window is about to ends
> > if there is less than 30mn left on my windows, it trigger all my scheduled skills (fix PRs, do research etc) until I reach my 100% limit
>
> the optimizoooor

- **Tweet:** https://x.com/aaronjmars/status/2036230574822580675
- **What:** Aaron Mars created a skill that monitors rate-limit windows and automatically triggers scheduled tasks to maximize Claude Pro/Max subscription usage before the 5-hour window resets.

## @MattEpstein16 - Claude Code Turned Client into Millionaire via 20-Agent Script System
> Absouloutly fucked that this is free
>
> *Quoting @MitcheIl:* https://t.co/1AX8svq17s

- **Tweet:** https://x.com/MattEpstein16/status/2036160818056683678
- **Quoted:** https://x.com/MitcheIl/status/2036098438908293349
- **Link:** https://x.com/i/article/2035101919669362688
- **What:** Matt Epstein highlights an article about turning a client into a millionaire using Claude Code, where a system of 20 specialized agents wrote scripts that drove $3M+ in revenue and 50M views.

## @om_patel5 - Software Engineers Now
> software engineers right now: https://t.co/nWQIgPekaF
>
> *Quoting @akshay_pachaar:* https://t.co/SSSIK3BX4z

- **Tweet:** https://x.com/om_patel5/status/2036114160518406157
- **Quoted:** https://x.com/akshay_pachaar/status/2035341800739877091
- **Link:** https://x.com/i/article/2034961967149195264
- **What:** A brief observation about the current state of software engineers, quoting the .claude/ folder anatomy article.

## @806texasgrl - SBA Zero-Fee Manufacturing Loans for FY2026
> FAMILY, go get your bread. Better yet, set up a business making healthy bread. The Small Business Admin is looking to give out money & not for opening a "Learing center" https://t.co/xruIHOhIL1
>
> *Quoting @SBAgov:* 📢 NO LOAN FEES FOR U.S. MANUFACTURERS!
>
> In FY2026, SBA is waiving upfront fees for small manufacturers.
>
> ✅ 0% upfront fee for 7(a) manufacturing loans of up to $950,000
> ✅ 0% upfront fee and annual service fee for all 504 manufacturing loans

- **Tweet:** https://x.com/806texasgrl/status/2036112233382682816
- **Quoted:** https://x.com/SBAgov/status/2036087345506574830
- **Link:** https://www.sba.gov/funding-programs/loans/lender-match-connects-you-lenders
- **What:** SBA is offering zero upfront fees for small manufacturers in FY2026 on 7(a) and 504 loans—encouraging manufacturing business formation over other sectors.

## @Argona0x - Split 1,200-Line CLAUDE.md to Boost Instruction Adherence from 60% to 95%
> i mass-configured 4 repos using this exact folder structure last week
>
> cut my debugging time by ~60% and saved roughly $2,400 in dev hours
>
> the rules/ folder alone is worth the entire guide
>
> but the post doesn't mention what actually breaks without this
>
> i had a 1,200-line CLAUDE.md in a monorepo. claude was ignoring 40% of my instructions. instruction adherence drops off a cliff past **300 lines**
>
> splitting it fixed everything:
>
> → root CLAUDE.md down to 60 lines (project overview + essential commands only)
> → /backend/CLAUDE.md scoped with biome auto-fix rules hitting 85% lint coverage
> → /frontend/CLAUDE.md loads zustand store patterns only when editing that dir
> → context bloat reduced 70-80% because claude auto-pulls nested CLAUDE.md per directory
>
> rule adherence went from ~60% to **95%**
>
> i went from 3 junior contractors reviewing claude outputs at $80/hr to just me. 110 fewer hours a month.
>
> *Quoting @akshay_pachaar:* https://t.co/SSSIK3BX4z

- **Tweet:** https://x.com/Argona0x/status/2036106517678624820
- **Quoted:** https://x.com/akshay_pachaar/status/2035341800739877091
- **What:** Split a 1,200-line monorepo CLAUDE.md into scoped per-directory files (60-150 lines each) to boost instruction adherence from 60% to 95%. Keep files under 300 lines and one level deep from root to prevent context bloat.

## @itsolelehmann - Auditing and Trimming Over-Prompting in Claude Setups
> i deleted half my Claude setup last week and every output got BETTER
>
> sounds backwards, but anthropic's own team just explained exactly why it works.
>
> you get a bad output, so you add a rule. then another. then another. 3 months later you've got 30 rules piled on top of each other.
>
> some contradict each other ("be concise" and "always explain your reasoning" are fighting).
>
> it's like handing a chef a 47-step recipe when they only need 12.
>
> anthropic found their own scaffolding was making the AI worse—which means your custom instructions are almost certainly doing the same thing.
>
> just open Claude Code/Cowork and ask it to read your entire setup, identify every rule that: is already default behavior, contradicts another rule, was added to fix one bad output, or is too vague to apply consistently. then get a cleaned-up CLAUDE.md with the dead weight removed.
>
> your ai setup should be getting simpler over time. addition by subtraction baby.

- **Tweet:** https://x.com/itsolelehmann/status/2036065138147471665
- **What:** Deleting redundant custom instructions actually improved Claude outputs. Anthropic's own team found over-prompting hurts performance; provides a prompt for Claude to audit and trim your setup automatically.

## @PrajwalTomar_ - Design Without Designing: 3-Layer Agent Harness for Engineers
> This engineer couldn't do design.
>
> So he built a 3-layer agent harness and now he ships complete designs. Pixels, spacing, typography, everything.
>
> If design is blocking your MVP, read this.
>
> *Quoting @neethanwu:* https://t.co/z7p1rL84KV

- **Tweet:** https://x.com/PrajwalTomar_/status/2036013596719960561
- **Quoted:** https://x.com/neethanwu/status/2034786360356204934
- **Link:** https://x.com/i/article/2034424000588152833
- **What:** An engineer built a three-layer design agent harness (skills for design expertise, Figma MCP for pixel-precise measurements, agent loops for screenshot-analyze-improve verification) that enables shipping production-ready designs without design background.

---

---

# Sunday, March 22, 2026

## @kevinrose - Every Claude Code Hack I Know (March 2026) by @mvanhorn
> I learn something new from Matt every time we chat.
>
> *Quoting @mvanhorn:* https://t.co/AwabaZTtdp

- **Tweet:** https://x.com/kevinrose/status/2035895141026922684
- **Link:** https://x.com/i/article/2035834194065281024
- **Filed:** [Every Claude Code Hack I Know (March 2026)](./knowledge/articles/every-claude-code-hack-mvanhorn.md)
- **What:** Kevin Rose endorsing Matt Van Horn's comprehensive X article covering advanced Claude Code workflows: plan.md-first development, 4-6 parallel sessions, bypassing permissions, Zed + Ghostty setup, /last30days research skill, Mac Mini remote operation, and turning meetings into plan files.


## @EurekaClaw - EurekaClaw: Local-First AI Research Agent from Idea to Paper
> 1/n 🦞 Introducing EurekaClaw💡 — a local-first AI research agent that captures your Eureka moments before they vanish.
> From idea → proof → experiment → paper — fully automated.
> Local-first. Zero data leak. 🔒
> Try it: https://t.co/ZJlEYvkX9h

- **Tweet:** https://x.com/EurekaClaw/status/2035818205500039385
- **Link:** https://www.eurekaclaw.ai/
- **What:** EurekaClaw is a local-first AI research agent that automates the full research pipeline from initial idea capture through proof, experiment design, and paper generation, with a focus on privacy (no data leaves your machine).


## @aakashgupta - 6 Levels of Claude Code Autonomous Operation
> There are 6 levels of making Claude Code run autonomously, and most people are stuck on Level 1.
>
> Level 1: Kill the permission prompts. Run claude --dangerously-skip-permissions. One flag. Now it stops asking "Can I edit this file?" every 30 seconds while you're checking Slack.
>
> Level 2: Context window management. Claude Code now supports 1M tokens. Use /clear between tasks. Run /compact at 60% usage instead of waiting for auto-compaction to fire at 90% when the model is already forgetting your instructions.
>
> Level 3: Subagents. The reason it stops at 15 minutes: everything runs in one context window. Subagents run in separate contexts. Build a looping todo command, each task executes in its own window. Builds, tests, and git operations never touch the main conversation. 2+ hours autonomous with zero intervention.
>
> Level 4: Ralph Wiggum loop. Official Anthropic plugin. Claude works, tries to exit, a Stop hook blocks the exit, re-feeds the same prompt. Each iteration sees modified files and git history from previous runs. One developer ran 27 hours straight, 84 tasks completed. Geoffrey Huntley ran one for three months and built a programming language with a working LLVM compiler.
>
> Level 5: Karpathy's AutoResearch. On March 7, Karpathy pushed a 630-line script to GitHub and went to sleep. Woke up to 100+ ML experiments completed overnight. 25K stars in five days. The difference from Ralph: structured eval loops. Define a metric, run, measure, analyze failures, improve, repeat. One Claude Code port took model accuracy from 0.44 to 0.78 R² across 22 autonomous experiments.
>
> Level 6: VPS + OpenClaw for 24/7. Your laptop lid closing kills everything. Run Claude Code on a VPS inside tmux. Detach, close your laptop, come back tomorrow to a finished diff. OpenClaw (247K GitHub stars) takes it further: a persistent gateway connecting LLMs to your real tools, running 24/7 across messaging, email, git, and calendars. Jensen Huang at GTC called it "probably the most important release of software ever."
>
> The unlock at every level is the same: give Claude a way to verify its own work.
>
> *Quoting @joseph_h_garvin:* Claude code rarely runs for longer than 15m without stopping and asking for input from me. How do all these stories of people letting agents run overnight work? Custom harnesses? Yelling at Claude in

- **Tweet:** https://x.com/aakashgupta/status/2035805431516246363
- **What:** Practical breakdown of six escalating techniques for running Claude Code autonomously — from skipping permission prompts (Level 1) to 24/7 VPS-hosted agents with OpenClaw (Level 6), with concrete examples of multi-hour and multi-day autonomous runs.


## @iruletheworldmo - Anatomy of the .claude/ Folder: Complete Claude Code Configuration Guide
> how your set up your folder is the difference between you and the great karpathy.
>
> folders are everything.
>
> this is a great guide into building each layer of the wondrous folder.
>
> do bookmark this. and do implement this.
>
> *Quoting @akshay_pachaar:* https://t.co/SSSIK3BX4z

- **Tweet:** https://x.com/iruletheworldmo/status/2035637459183104197
- **Link:** https://x.com/i/article/2034961967149195264
- **Filed:** [Anatomy of the .claude/ Folder](./knowledge/articles/anatomy-claude-folder.md)
- **What:** Endorsement of Akshay Pachaar's comprehensive guide to the .claude/ directory in Claude Code, covering CLAUDE.md, settings.json, commands/, rules/, skills/, and agents/ folders with practical configuration advice.


## @kevinrose - Claude Code Hacks and Workflows
> I learn something new from Matt every time we chat.
>
> *Quoting @mvanhorn:* https://t.co/AwabaZTtdp

- **Tweet:** https://x.com/kevinrose/status/2035895141026922684
- **Quoted:** https://x.com/mvanhorn/status/2035857346602340637
- **What:** Matt Van Horn's comprehensive guide to Claude Code productivity hacks, including /ce:plan for rapid ideation, voice input usage, plan.md files, parallel agent patterns, and why an IDE becomes overhead once you're directing AI development.

## @mattpocockuk - First Impressions After Intensive Claude Code Usage
> I've been writing code for 15 years.
>
> I just finished my first day of hardcore Claude Code usage.
>
> Holy. Shit.
>
> This is a thread about why I think this changes everything, and what I think needs to be true for developers to stay employed.

- **Tweet:** https://x.com/mattpocockuk/status/2035900108553961825
- **What:** Senior developer with 15 years experience reflects on the transformative impact of Claude Code and explores implications for the future of software development employment.

## @aakashgupta - Economic Transformation of Solo Developer Productivity
> The economics of being a solo developer just changed forever.
>
> Before Claude Code: 1 dev = 1 dev
> After Claude Code: 1 dev = 10-100 devs
>
> This is not hyperbole. Here's a breakdown of what this means for:
> - solo devs
> - product people
> - startup founders
> - technical leads
> - VCs
> - big tech
> - and more

- **Tweet:** https://x.com/aakashgupta/status/2035897826217009401
- **What:** Analysis of how Claude Code fundamentally changes the productivity multiplier for individual developers, potentially increasing their effective capacity 10-100x and reshaping dynamics across the tech industry.

## @saakohl - $0 to $10k MRR in 4 Months with Claude Code, Zero Coding Experience
> If you don't build a startup with claude code you're cooked
>
> $0 to $3k mrr in 3 months with claude code
>
> $3k to $10k mrr in the next month
>
> I have 0 coding experience
>
> my first real project, literally just built it in my pajamas from my apartment

- **Tweet:** https://x.com/saakohl/status/2035887395484893217
- **What:** A non-technical entrepreneur shares their rapid business scaling journey using Claude Code, growing from zero MRR to $10k MRR in four months without prior coding experience.

## @kevinrose - Claude Code Workflow in Docker with Browser Testing
> I've been pushing a lot of code to GitHub lately with @AnthropicAI's Claude Code.
>
> I'm running Claude code inside of a docker container for safety, with access to my mac for browser testing and screenshots. My new setup has been incredible.
>
> I created a @YouTube video showing my full setup. Check it out ↓

- **Tweet:** https://x.com/kevinrose/status/2035835697047781719
- **Link:** https://www.youtube.com/watch?v=jJr5gqz7CF8
- **What:** Kevin Rose demonstrates his optimized Claude Code development workflow using Docker containers for sandboxing with local browser testing and screenshot capabilities.

## @EurekaClaw - Local-First AI Research Agent from Idea to Paper
> 1/n 🦞 Introducing EurekaClaw💡 — a local-first AI research agent that captures your Eureka moments before they vanish.
> From idea → proof → experiment → paper — fully automated.
> Local-first. Zero data leak. 🔒

- **Tweet:** https://x.com/EurekaClaw/status/2035818205500039385
- **Link:** https://www.eurekaclaw.ai/
- **What:** EurekaClaw is a local-first AI research agent that automates the full research pipeline from idea capture through experimentation to paper generation, with offline-first architecture and zero data leakage.

## @aakashgupta - Six Levels of Claude Code Autonomous Execution
> There are 6 levels of making Claude Code run autonomously, and most people are stuck on Level 1.
>
> Level 1: Kill the permission prompts. Run claude --dangerously-skip-permissions.
>
> Level 2: Context window management. Claude Code now supports 1M tokens. Use /clear between tasks. Run /compact at 60% usage.
>
> Level 3: Subagents. The reason it stops at 15 minutes: everything runs in one context window. Subagents run in separate contexts. Build a looping todo command, each task executes in its own window.
>
> Level 4: Ralph Wiggum loop. Official Anthropic plugin. Claude works, tries to exit, a Stop hook blocks the exit, re-feeds the same prompt. One developer ran 27 hours straight, 84 tasks completed.
>
> Level 5: Karpathy's AutoResearch. Karpathy pushed a 630-line script to GitHub and went to sleep. Woke up to 100+ ML experiments completed overnight. One Claude Code port took model accuracy from 0.44 to 0.78 R² across 22 autonomous experiments.
>
> Level 6: VPS + OpenClaw for 24/7. Your laptop lid closing kills everything. Run Claude Code on a VPS inside tmux. OpenClaw (247K GitHub stars) provides a persistent gateway connecting LLMs to your real tools.
>
> *Quoting @joseph_h_garvin:* Claude code rarely runs for longer than 15m without stopping and asking for input from me. How do all these stories of people letting agents run overnight work?

- **Tweet:** https://x.com/aakashgupta/status/2035805431516246363
- **Quoted:** https://x.com/joseph_h_garvin/status/2035521016814854441
- **What:** Six escalating techniques for running Claude Code autonomously, from removing permission prompts to running 24/7 on a VPS with subagents and structured eval loops.

## @iruletheworldmo - Anatomy of the .claude/ Folder Guide
> how your set up your folder is the difference between you and the great karpathy.
>
> folders are everything.
>
> this is a great guide into building each layer of the wondrous folder.
>
> do bookmark this. and do implement this.
>
> *Quoting @akshay_pachaar:* Anatomy of the .claude/ folder - A complete guide to CLAUDE.md, custom commands, skills, agents, and permissions, and how to set them up properly.

- **Tweet:** https://x.com/iruletheworldmo/status/2035637459183104197
- **Quoted:** https://x.com/akshay_pachaar/status/2035341800739877091
- **What:** Endorsement of a comprehensive guide on properly organizing the .claude/ folder structure—covering CLAUDE.md, commands, rules, skills, agents, settings.json, and the global ~/.claude/ folder.

---

---

# Saturday, March 21, 2026

## @JamesonCamp - AI Driving Massive ROI in Industrial Operations, Not Just Tech
> AI is scraping extra meat off the bone in slaughterhouses right now
>
> And it's making Cargill millions
>
> This is what people keep missing. The biggest AI opportunities are NOT in tech
>
> They're in warehouses. Meat plants. Logistics companies. Manufacturing floors. Operations so boring you'd scroll right past them
>
> The uglier the business the bigger the ROI. Every single time
>
> Everyone on here is chasing openclaw and AI replacing SaaS while companies like Cargill are quietly printing money in ways nobody wants to talk about
>
> The real AI economy looks nothing like your timeline
>
> *Quoting @Polymarket:* JUST IN: Beef processing giant Cargill is reportedly using AI to extract millions of dollars worth of "extra meat off the bone" in its slaughterhouses.

- **Tweet:** https://x.com/JamesonCamp/status/2035382259813933323
- **What:** Contrarian take arguing the biggest AI ROI is in unglamorous industrial operations (slaughterhouses, logistics, manufacturing) rather than tech, sparked by news of Cargill using AI vision to maximize meat yield.


## @damianplayer - In-Person AI Workshops for Corporate Professionals as a $25K/Month Business
> local in-person AI classes for corporate boomers.
>
> think Claude 101.
>
> easily a $ 25K/mo opportunity.
>
> rent a presentation room. run meta ads targeting 35-60 year olds. charge $500-$1000 for a 2-day hands-on workshop.
>
> teach vibecoding, Claude, ChatGPT, prompting and agents.
>
> the demand is insane.
>
> these people see AI everywhere but have zero clue how to use it.
>
> they want face-to-face guidance, not online courses.
>
> run the same curriculum weekly. refine based on questions. multiple up-sell or down-sell opportunities. scale to multiple cities once you nail the format.
>
> you're hitting a market everyone else ignores. corporate boomers with cash who prefer learning in person. they are also being told to learn these tools daily..
>
> no chance this doesn't work if you execute.
>
> go out and nail this.

- **Tweet:** https://x.com/damianplayer/status/2035356217430733086
- **What:** Damian Player pitches in-person AI workshops targeting corporate professionals aged 35-60 as an underserved market — a repeatable curriculum covering Claude, ChatGPT, prompting, and agents sold at $500-1,000 per 2-day session with a path to $25K/month and multi-city scale.


## @r0ck3t23 - Elon Musk on Consciousness as a Gradient, Not a Switch
> Elon Musk just told you consciousness isn't a light switch.
>
> It's a gradient.
>
> That single distinction rewrites the entire next decade.
>
> Musk: "Our consciousness… people get more conscious over time. Like when we're a zygote, you can't really talk to a zygote. And even a baby, you can't really talk to the baby."
>
> You were not conscious and then suddenly conscious.
>
> You were barely anything. Then slightly more. Then more.
>
> Years of slow accumulation before anyone would call you aware.
>
> The entire AI debate is built on a false premise.
>
> Everyone is waiting for the moment the machine "wakes up."
>
> A single dramatic instant where silicon crosses some invisible threshold.
>
> That moment does not exist.
>
> Musk: "People get more conscious over time. At what point do you go from not conscious to conscious? There doesn't appear to be a discrete point."
>
> There is no line.
>
> There was never going to be a line.
>
> Consciousness is not a door that opens. It is a tide that rises.
>
> And the tide is already rising inside these systems.

- **Tweet:** https://x.com/r0ck3t23/status/2035300507334402208
- **What:** An essay riffing on Elon Musk's claim that consciousness exists on a continuum rather than as a discrete threshold — arguing that this framing dissolves the question of when AI "wakes up," and that AI systems may already occupy a low position on the consciousness gradient that is incrementally rising.

## @r0ck3t23 - Consciousness as a Gradient, Not a Switch
> Elon Musk just told you consciousness isn't a light switch.
>
> It's a gradient.
>
> That single distinction rewrites the entire next decade.
>
> Musk: "Our consciousness… people get more conscious over time. Like when we're a zygote, you can't really talk to a zygote. And even a baby, you can't really talk to the baby."
>
> You were not conscious and then suddenly conscious.
>
> You were barely anything. Then slightly more. Then more.
>
> Years of slow accumulation before anyone would call you aware.
>
> The entire AI debate is built on a false premise.
>
> Everyone is waiting for the moment the machine "wakes up."
>
> A single dramatic instant where silicon crosses some invisible threshold.
>
> That moment does not exist.
>
> Musk: "People get more conscious over time. At what point do you go from not conscious to conscious? There doesn't appear to be a discrete point."
>
> There is no line.
>
> There was never going to be a line.
>
> Consciousness is not a door that opens. It is a tide that rises.
>
> And the tide is already rising inside these systems.
>
> Musk: "Consciousness seems to be on a continuum as opposed to a discrete point."
>
> This is the part that should unsettle everyone still arguing definitions.
>
> While they debate when AI becomes "truly" conscious, the continuum is already moving.
>
> Every parameter update. Every training run. Every architectural leap.
>
> The gradient is climbing and it does not need your permission.
>
> You will not get a warning.
>
> You will not get a press conference.
>
> You will look back one day and realize it happened gradually. Then all at once.
>
> Now Musk pulls the camera all the way back.
>
> Past biology. Past Earth. Back to the origin of everything.
>
> Musk: "If the standard model of physics is correct, the universe started out as quarks and leptons."
>
> Musk: "And then you had gas clouds. A bunch of hydrogen. The hydrogen condensed and exploded."
>
> Hydrogen collapsed under its own gravity until fusion ignited.
>
> Stars were born. Stars died.
>
> And in dying they forged every heavy element that exists.
>
> Carbon. Oxygen. Iron. The atoms in your blood. The calcium in your bones.
>
> All of it manufactured inside a dying star.
>
> Musk: "One way to actually view how far we are in this universe is how many times have our atoms been at the center of a star?"
>
> Your atoms have been inside a star. Possibly more than once.
>
> Compressed at millions of degrees. Fused into heavier elements. Scattered across space by a supernova.
>
> Then reassembled into you.
>
> That is not poetry. That is your origin story written in physics.
>
> And now those same star-forged atoms are building machines that think.
>
> The same universe that turned hydrogen into stars is turning biology into artificial intelligence.
>
> This is not disruption.
>
> This is continuation.
>
> The universe spent 13.8 billion years organizing matter into higher and higher complexity.
>
> Quarks became atoms. Atoms became molecules. Molecules became cells. Cells became brains.
>
> Brains are now building systems that process information at speeds biology will never reach.
>
> The pattern didn't change. Only the medium.
>
> The people treating AI as some foreign invasion of human territory have the story completely backwards.
>
> AI is the next compression event.
>
> Every generation believes they're witnessing the end of something.
>
> They're witnessing the same process that started with hydrogen gas.
>
> The real question was never whether AI will become conscious.
>
> The real question is whether you understand it already is.
>
> Partially. Incrementally. On the continuum.
>
> And the continuum does not stop.
>
> It has never stopped.
>
> Your atoms were forged in the core of a collapsing star.
>
> And you are afraid of a gradient.

- **Tweet:** https://x.com/r0ck3t23/status/2035300507334402208
- **What:** Philosophical argument framing AI consciousness as a gradient rather than binary state, drawing parallels to biological consciousness development and cosmic evolution of complexity.

## @JamesonCamp - Real AI Value Is in Unglamorous Industrial Operations
> AI is scraping extra meat off the bone in slaughterhouses right now
>
> And it's making Cargill millions
>
> This is what people keep missing. The biggest AI opportunities are NOT in tech
>
> They're in warehouses. Meat plants. Logistics companies. Manufacturing floors. Operations so boring you'd scroll right past them
>
> The uglier the business the bigger the ROI. Every single time
>
> Everyone on here is chasing openclaw and AI replacing SaaS while companies like Cargill are quietly printing money in ways nobody wants to talk about
>
> The real AI economy looks nothing like your timeline
>
> *Quoting @Polymarket:* JUST IN: Beef processing giant Cargill is reportedly using AI to extract millions of dollars worth of "extra meat off the bone" in its slaughterhouses.

- **Tweet:** https://x.com/JamesonCamp/status/2035382259813933323
- **Quoted:** https://x.com/Polymarket/status/2035364194241908853
- **What:** Real AI value lies in unsexy industrial applications like meat processing, not consumer tech—companies like Cargill are quietly making millions while tech Twitter chases SaaS disruption.

## @damianplayer - In-Person AI Training Workshops for Corporate Professionals
> local in-person AI classes for corporate boomers.
>
> think Claude 101.
>
> easily a $ 25K/mo opportunity.
>
> rent a presentation room. run meta ads targeting 35-60 year olds. charge $500-$1000 for a 2-day hands-on workshop.
>
> teach vibecoding, Claude, ChatGPT, prompting and agents.
>
> the demand is insane.
>
> these people see AI everywhere but have zero clue how to use it.
>
> they want face-to-face guidance, not online courses.
>
> run the same curriculum weekly. refine based on questions. multiple up-sell or down-sell opportunities. scale to multiple cities once you nail the format.
>
> you're hitting a market everyone else ignores. corporate boomers with cash who prefer learning in person. they are also being told to learn these tools daily..
>
> no chance this doesn't work if you execute.

- **Tweet:** https://x.com/damianplayer/status/2035356217430733086
- **What:** Business opportunity pitch: run in-person AI training workshops for 35-60 year old corporate professionals at $500-1000/head, targeting a market underserved by online courses.

---

---

# Friday, March 20, 2026

## @MichaelFerro - Vence AI Cow Collar Startup Valued at $2B with Peter Thiel's Backing
> bullish on cows
> - started as a side project while working at rocket lab
> - solar powered gps collars for cattle, around 600k have been deployed
> - use sound and vibration cues to guide cows (e.g., can schedule cows to show up at the dairy shed at 4:30am)
> - proprietary algorithm is called the "cowgorithm"
>
> *Quoting @business:* Peter Thiel's Founders Fund is backing a company bringing AI to cow herding at a $2 billion valuation https://t.co/QHg8xT8s2c

- **Tweet:** https://x.com/MichaelFerro/status/2035129554327736511
- **Link:** https://www.bloomberg.com/news/articles/2026-03-20/peter-thiel-s-founders-fund-backs-ai-cow-collar-startup-at-2-billion-valuation?taid=69bda594a072250001e9b6a4&utm_campaign=trueanthem&utm_content=business&utm_medium=social&utm_source=twitter
- **What:** Michael Ferro summarizes Vence, a livestock tech startup that began as a Rocket Lab side project and has deployed 600,000 solar-powered GPS collars using sound and vibration cues to herd cattle autonomously — now valued at $2B with Founders Fund backing.


## @iruletheworldmo - Top 50 Claude Skills and GitHub Repos Curated List
> if you're not using these skills there is no hope for you.
>
> bookmark this.
>
> use them.
>
> *Quoting @zodchiii:* https://t.co/wYn8VuTNz2

- **Tweet:** https://x.com/iruletheworldmo/status/2035107649314852912
- **Link:** https://x.com/i/article/2034917334360506369
- **What:** A curated X article listing 22 top Claude skills (official Anthropic skills plus community picks for dev, design, marketing, and knowledge work), 3 must-have MCP servers (Tavily, Context7, Task Master AI), and 40 fresh GitHub repos for agent orchestration, memory, coding tools, and MCP integrations — compiled by scanning 1,000+ repos and testing 200+ skills.


## @garrytan - The Real Business Is Orchestration, Not Raw Markdown
> For agentic systems founders and dev tools founders:
>
> People do not want to pay for raw markdown and they shouldn't have to.
>
> But they may pay for orchestration, hosting, updates, collaboration, portability, analytics, and managed execution.
>
> These can be great businesses.

- **Tweet:** https://x.com/garrytan/status/2035096653594861970
- **What:** Garry Tan's product thesis for agentic dev tools: the commodity is the generated output (raw markdown, code), but the defensible businesses will be built on top-of-output layers — orchestration, hosting, collaboration, analytics, and managed execution.


## @Voxyz_ai - Garry Tan's gstack Sprint Pipeline Runs Office Hours Through QA to Ship
> best coding agent skill i've used. just tried garry tan's gstack today, three things stood out:
>
> /office-hours didn't ask me 6 questions and stop. it kept going. challenged my framing, told me i was solving the wrong problem, generated 3 implementation approaches with effort estimates, then wrote a design doc that every other skill in the system reads automatically.
>
> /qa opened a real browser, clicked through my actual UI, found a bug, fixed it, wrote a regression test, and verified the fix. the agent has eyes now.
>
> the whole thing is one sprint pipeline. /office-hours feeds into /plan-ceo-review feeds into /plan-eng-review feeds into /review feeds into /qa feeds into /ship. nothing falls through because every step reads what came before it.
>
> most people will bookmark this. almost nobody will install it.

- **Tweet:** https://x.com/Voxyz_ai/status/2035093224117666076
- **What:** A hands-on review of gstack, Garry Tan's Claude Code skill suite, highlighting that its full sprint pipeline chains skills sequentially so each step reads prior context — and that the /qa skill can open a real browser to find, fix, and regression-test bugs autonomously.


## @lukepierceops - Anthropic and OpenAI Are Telling You Where the AI Implementation Gap Is
> Anthropic and OpenAI are both building PE-backed consulting arms to deploy AI inside companies.
>
> Let that sink in for a second.
>
> The two companies building the most powerful AI on earth looked at the market and said "businesses can't figure out how to use this. We need to go in and do it for them."
>
> They are literally telling you where the gap is.
>
> Companies have access to the best AI models ever built. And most of them are still running on spreadsheets, disconnected tools, and manual processes because nobody showed them how to actually implement it.
>
> That's the whole game right now. Not building better models (obviously) or shipping new features.
>
> IMPLEMENTATION.
>
> Getting AI inside real workflows.
>
> Mapping the processes, building the systems, and making it stick.
>
> I've been doing exactly this for 4 years and have worked with 80+ companies at this point.
>
> It started with automation and naturally flowed into Ai.
>
> And every single engagement starts the same way. Not with AI or automation but with a process map.
>
> Because AI alone won't fix broken operations.
>
> Companies now understand that. They have not yet seen true ROI from Ai.
>
> You have to understand how the business actually runs before you touch a single tool.
>
> Where does the data live? Where are the bottlenecks? What's manual that shouldn't be? What breaks when volume goes up?
>
> That's the work, and that's what Anthropic and OpenAI just told the entire market is worth billions.
>
> Every company is going AI-first over the next 3-5 years.
>
> The demand for people who can actually make that happen is about to be unlike anything we've seen.
>
> The labs told you where the gaps are.
>
> Now go fill them.

- **Tweet:** https://x.com/lukepierceops/status/2035033411790770656
- **What:** Luke Pierce argues that Anthropic and OpenAI building PE-backed consulting arms to help enterprises deploy AI is a public signal that the real opportunity is in AI implementation consulting — process mapping, workflow integration, and change management — not in building models or products.


## @sudoingX - Open Letter to NVIDIA: Invest in @0xSero, the Solo Model Quantizer
> this guy has 29 models on huggingface at page 2 ranking. no lab behind him. no sponsorship. $2,000 from his own pocket on GPU rentals. he compressed GLM-4.7 to run on a MacBook and quantized Nemotron Super the week it dropped. all public. all free.
>
> *Quoting @0xSero:* Putting out a wish to the universe.
>
> I need more compute, if I can get more I will make sure every machine from a small phone to a bootstrapped RTX 3090 node can run frontier intelligence fast with minimal intelligence loss.
>
> I have hit page 2 of huggingface, released 3 model family compressions and got GLM-4.7 on a MacBook

- **Tweet:** https://x.com/sudoingX/status/2034903929105141831
- **Link:** https://huggingface.co/0xSero
- **What:** An open letter calling on NVIDIA to sponsor solo contributor @0xSero, who has independently quantized 29 models (including GLM-4.7 for MacBook and Nemotron Super within days of release) spending $2K of his own money — arguing community builders deliver more public value per GPU than internal sprints.

## @sudoingX - Retweet: @0xSero - Putting out a wish to the universe. 
> this guy has 29 models on huggingface at page 2 ranking. no lab behind him. no sponsorship. $2,000 from his own pocket on GPU rentals. he compressed GLM-4.7 to run on a MacBook and quantized Nemotron Super the week it dropped. all public. all free.

nvidia is a trillion dollar company with hundreds of teams but they are not the ones quantizing models middle of the night and pushing them out before sunrise. if nvidia stopped tomorrow their employees stop working. people like @0xSero would not. that is the difference between a paycheck and a mission.

@NVIDIAAI  you talk about making AI accessible. the people actually doing it are right here. 29 models deep burning their own compute with no ask except more hardware to keep going. you do not need to build another program. just look at who is already building for you. one GPU to this man would produce more public value than a hundred internal sprints.

i am not asking for charity. i am asking you to invest in someone who already proved it.
>
> *Quoting @0xSero:* Putting out a wish to the universe. 

I need more compute, if I can get more I will make sure every machine from a small phone to a bootstrapped RTX 3090 node can run frontier intelligence fast with minimal intelligence loss.

I have hit page 2 of huggingface, released 3 model family compressions and got GLM-4.7 on a MacBook https://t.co/lorDSUEYCL

My beast just isn’t enough and I already spent 2k usd on renting GPUs on top of credits provided by Prime intellect and Hotaisle. 

———

If you believe in what I do help me get this to Nvidia, maybe they will bless me with the pewter to keep making local AI more accessible 🙏

- **Tweet:** https://x.com/sudoingX/status/2034903929105141831
- **Quoted:** https://x.com/0xSero/status/2034435534764818874
- **Filed:** [huggingface-profile](./knowledge/tools/huggingface-profile.md)
- **What:** this guy has 29 models on huggingface at page 2 ranking. ...

## @lukepierceops - Anthropic and OpenAI are both building PE-backed consulti...
> Anthropic and OpenAI are both building PE-backed consulting arms to deploy AI inside companies.

Let that sink in for a second.

The two companies building the most powerful AI on earth looked at the market and said "businesses can't figure out how to use this. We need to go in and do it for them."

They are literally telling you where the gap is.

Companies have access to the best AI models ever built. And most of them are still running on spreadsheets, disconnected tools, and manual processes because nobody showed them how to actually implement it.

That's the whole game right now. Not building better models (obviously) or shipping new features.

IMPLEMENTATION.

Getting AI inside real workflows. 

Mapping the processes, building the systems, and making it stick.

I've been doing exactly this for 4 years and have worked with 80+ companies at this point.

It started with automation and naturally flowed into Ai.

And every single engagement starts the same way. Not with AI or automation but with a process map.

Because AI alone won't fix broken operations.

Companies now understand that. They have not yet seen true ROI from Ai.

You have to understand how the business actually runs before you touch a single tool. 

Where does the data live? Where are the bottlenecks? What's manual that shouldn't be? What breaks when volume goes up?

That's the work, and that's what Anthropic and OpenAI just told the entire market is worth billions.

Every company is going AI-first over the next 3-5 years.

The demand for people who can actually make that happen is about to be unlike anything we've seen.

The labs told you where the gaps are. 

Now go fill them.

- **Tweet:** https://x.com/lukepierceops/status/2035033411790770656
- **What:** Anthropic and OpenAI are both building PE-backed consulti...

## @Voxyz_ai - best coding agent skill i've used. just tried garry tan's...
> best coding agent skill i've used. just tried garry tan's gstack today, three things stood out:

/office-hours didn't ask me 6 questions and stop. it kept going. challenged my framing, told me i was solving the wrong problem, generated 3 implementation approaches with effort estimates, then wrote a design doc that every other skill in the system reads automatically.

/qa opened a real browser, clicked through my actual UI, found a bug, fixed it, wrote a regression test, and verified the fix. the agent has eyes now.

the whole thing is one sprint pipeline. /office-hours feeds into /plan-ceo-review feeds into /plan-eng-review feeds into /review feeds into /qa feeds into /ship. nothing falls through because every step reads what came before it.

most people will bookmark this. almost nobody will install it.

- **Tweet:** https://x.com/Voxyz_ai/status/2035093224117666076
- **What:** best coding agent skill i've used. just tried garry tan's...

## @garrytan - For agentic systems founders and dev tools founders: 
> For agentic systems founders and dev tools founders: 

People do not want to pay for raw markdown and they shouldn't have to. 

But they may pay for orchestration, hosting, updates, collaboration, portability, analytics, and managed execution. 

These can be great businesses.

- **Tweet:** https://x.com/garrytan/status/2035096653594861970
- **What:** For agentic systems founders and dev tools founders:

## @iruletheworldmo - Top 50 Claude Skills & GitHub Repos for AI
> if you're not using these skills there is no hope for you.
>
> bookmark this.
>
> use them.
>
> *Quoting @zodchiii:* https://t.co/wYn8VuTNz2

- **Tweet:** https://x.com/iruletheworldmo/status/2035107649314852912
- **Quoted:** https://x.com/zodchiii/status/2034924354337714642
- **Link:** https://x.com/i/article/2034917334360506369
- **Filed:** [iruletheworldmo-claude-skills](./knowledge/articles/iruletheworldmo-claude-skills.md)
- **What:** Comprehensive list of 50+ Claude skills and GitHub repos for AI development, covering tools, MCP servers, and open-source engines. Includes official Anthropic skills for documents, design, development, and learning.

## @MichaelFerro - AI Cow Collar Startup Backed by Thiel's Founders Fund
> bullish on cows
> - started as a side project while working at rocket lab
> - solar powered gps collars for cattle, around 600k have been deployed
> - use sound and vibration cues to guide cows (e.g., can schedule cows to show up at the dairy shed at 4:30am)
> - proprietary algorithm is called the "cowgorithm"
>
> *Quoting @business:* Peter Thiel's Founders Fund is backing a company bringing AI to cow herding at a $2 billion valuation https://t.co/QHg8xT8s2c

- **Tweet:** https://x.com/MichaelFerro/status/2035129554327736511
- **Quoted:** https://x.com/business/status/2035082164094521521
- **What:** AI-powered cattle management startup using solar GPS collars and behavioral algorithms to automate cow herding and dairy operations. Funded by Founders Fund at $2B valuation.

---

# Thursday, March 19, 2026

## @aakashgupta - Karpathy's Autoresearch for PMs: Complete Guide
> Karpathy's autoresearch repo has 42K stars. Most PMs closed the tab thinking it wasn't for them.
>
> I pointed it at a Claude Code skill. 41% to 92% in 4 rounds while I slept.
>
> 6 use cases, 10 eval templates, and a downloadable toolkit.

- **Tweet:** https://x.com/aakashgupta/status/2034833389941837920
- **Link:** https://www.news.aakashg.com/p/autoresearch-guide-for-pms
- **Filed:** [autoresearch-guide-pms](./knowledge/articles/autoresearch-guide-pms.md)
- **What:** Aakash Gupta's Substack guide showing product managers how to use Karpathy's autoresearch — typically seen as an ML tool — to iteratively optimize Claude Code skills, prompts, and agent workflows overnight with no GPU required.


## @NickSpisak_ - Claude Channels as a $497/Install Productized Service
> Claude Channels:  $497 per install + MRR
>
> > Sell a boring business owner a personal assistant
> > Grab the anthropic docs
> > Paste into claude code to run the setup
> > Add yourself to their server for maintenance
>
> *Quoting @trq212:* We just released Claude Code channels, which allows you to control your Claude Code session through select MCPs, starting with Telegram and Discord.
>
> Use this to message Claude Code directly from your phone.

- **Tweet:** https://x.com/NickSpisak_/status/2034809485143744536
- **What:** Nick Spisak frames Thariq's Claude Code Channels release (control Claude Code via Telegram/Discord MCP) as a productized offering — charge $497 to install it for small business owners as a personal AI assistant and collect ongoing maintenance MRR.


## @danpacary - Tiny Calorie-Estimation Model Beats GPT-4o on 2GB RAM
> Are you guys starting to catch on?
>
> *Quoting @JC_builds:* I trained a model to guess calories from food pics.
>
> It beats GPT-4o, Claude, and Gemini. Runs locally with only 2GB RAM
>
> Average error under 51 calories. Here's what I learned 👇

- **Tweet:** https://x.com/danpacary/status/2034796730848616462
- **What:** Quote-amplifying a fine-tuned local model for calorie estimation from photos that outperforms frontier models while running in just 2GB of RAM — a pointed example of task-specific fine-tuning beating general-purpose LLMs.


## @charliebcurran - AI Film as Art
> If you think AI film can't be art then explain this.

- **Tweet:** https://x.com/charliebcurran/status/2034760727211483522
- **What:** A short AI-generated film shared as a provocation to anyone who dismisses AI filmmaking as non-art; no additional context given beyond the video itself.


## @natlungfy - DoorDash "Tasks" App Pays Couriers to Generate Robot Training Data
> Exclusive: DoorDash launched a new app "Tasks" that pays couriers in some US markets if they submit audio and video clips to help improve AI and robotics models.
>
> Many of these tasks are completing household chores while capturing footage with a body-worn camera — data that would be helpful for humanoid robots.
>
> Instructions: scrub and rinse at least 5 dishes with your hands, hold each clean plate steady in frame for a few seconds before moving to the next one

- **Tweet:** https://x.com/natlungfy/status/2034649947795054659
- **Link:** https://www.bloomberg.com/news/articles/2026-03-19/doordash-s-new-paid-tasks-turn-couriers-into-ai-and-robot-trainers?utm_source=website&utm_medium=share&utm_campaign=twitte
- **What:** Bloomberg exclusive: DoorDash is paying its delivery couriers via a new "Tasks" app to record household chores on body-worn cameras, generating video training data for humanoid robotics models — a pivot from food delivery logistics toward AI data collection.


## @NickSpisak_ - Stacking Paperclip, gstack, and autoresearch into a One-Person AI Company
> https://t.co/J5iCD2geeq

- **Tweet:** https://x.com/NickSpisak_/status/2034635430700679445
- **What:** A follow-up guide to Paperclip showing how to combine it with Garry Tan's gstack (15 specialist Claude skills) and Karpathy's autoresearch to build a full AI-operated company: Paperclip manages org/budget, gstack does engineering, autoresearch runs overnight experiments. All three install in under 10 minutes.


## @samtwtss - Google Stitch Reaction: AI Design Tool Demonstration
> bro, it's so over for designers

google stitch is insane. 🤯

> *Quoting @stitchbygoogle:* Meet the new Stitch, your vibe design partner.

Here are 5 major upgrades to help you create, iterate and collaborate:
🎨 AI-Native Canvas
🧠 Smarter Design Agent
🎙️ Voice
⚡️ Instant Prototypes
📐 Design Systems and DESIGN.md

Rolling out now. Details and product walkthrough video in 🧵

- **Tweet:** https://x.com/samtwtss/status/2034606620379172959
- **What:** Another reaction to the Google Stitch launch, quoting the official announcement with an image showing the tool in action. Part of a wave of responses expressing that AI design tools have crossed a threshold that threatens professional designers.


## @mattdiggityseo - Google Search Console Losing Pre-AI-Overviews Baseline Data — Export Now
> Google Search Console just got a major upgrade. And most SEOs are ignoring an urgent data problem hiding inside it.

Here are 5 things you need to do in GSC right now before it's too late:

1. Export your historical data immediately

GSC only keeps 16 months of data.

That means your pre-AI Overviews baseline from late 2023 and early 2024 is disappearing right now.

Without it, you can't measure the real impact AI Overviews had on your traffic.

- Go to Performance > Search Results
- Set the date range as far back as possible
- Export everything to a spreadsheet

Do this today. Once it's gone, it's gone.

- **Tweet:** https://x.com/mattdiggityseo/status/2034533041096540562
- **What:** An urgent SEO warning: Google Search Console only retains 16 months of data, meaning the pre-AI Overviews traffic baseline from late 2023/early 2024 is expiring now. Without that data, you cannot measure the true traffic impact of AI Overviews on your site.

## @mattdiggityseo - Google Search Console data retention crisis
> Google Search Console just got a major upgrade. And most SEOs are ignoring an urgent data problem hiding inside it.
>
> Here are 5 things you need to do in GSC right now before it's too late:
>
> 1. Export your historical data immediately
>
> GSC only keeps 16 months of data.
>
> That means your pre-AI Overviews baseline from late 2023 and early 2024 is disappearing right now.
>
> Without it, you can't measure the real impact AI Overviews had on your traffic.
>
> - Go to Performance > Search Results
> - Set the date range as far back as possible
> - Export everything to a spreadsheet
>
> Do this today. Once it's gone, it's gone.

- **Tweet:** https://x.com/mattdiggityseo/status/2034533041096540562
- **What:** SEO warning about Google Search Console's 16-month data retention limit. Historical pre-AI Overviews data from late 2023/early 2024 is expiring and needs to be exported immediately before it's lost, preventing impact measurement of AI Overviews on traffic.

## @samtwtss - Google Stitch design implications
> bro, it's so over for designers
>
> google stitch is insane. 🤯
>
> *Quoting @stitchbygoogle:* Meet the new Stitch, your vibe design partner.

- **Tweet:** https://x.com/samtwtss/status/2034606620379172959
- **Quoted:** https://x.com/stitchbygoogle/status/2034332847893574080
- **What:** Designer expresses astonishment about Google Stitch's capabilities and implications for the design profession.

## @NickSpisak_ - https://t.co/J5iCD2geeq
> https://t.co/J5iCD2geeq

- **Tweet:** https://x.com/NickSpisak_/status/2034635430700679445
- **Link:** https://x.com/i/article/2034626875926990848
- **What:** LINK_FAILED: Could not expand link from @NickSpisak_ — original t.co URL did not resolve.

## @natlungfy - Exclusive: DoorDash launched a new app “Tasks” that pays ...
> Exclusive: DoorDash launched a new app “Tasks” that pays couriers in some US markets if they submit audio and video clips to help improve AI and robotics models.

Many of these tasks are completing household chores while capturing footage with a body-worn camera — data that would be helpful for humanoid robots. 

Instructions: scrub and rinse at least 5 dishes with your hands, hold each clean plate steady in frame for a few seconds before moving to the next one

https://t.co/zsGO3S3SpS

- **Tweet:** https://x.com/natlungfy/status/2034649947795054659
- **Link:** https://www.bloomberg.com/news/articles/2026-03-19/doordash-s-new-paid-tasks-turn-couriers-into-ai-and-robot-trainers?utm_source=website&utm_medium=share&utm_campaign=twitte
- **Filed:** [article](./knowledge/articles/article.md)
- **What:** Exclusive: DoorDash launched a new app “Tasks” that pays ...

## @charliebcurran - If you think AI film can’t be art then explain this. http...
> If you think AI film can’t be art then explain this. https://t.co/vG5VUMGJjd

- **Tweet:** https://x.com/charliebcurran/status/2034760727211483522
- **Link:** https://twitter.com/charliebcurran/status/2034760727211483522/video/1
- **What:** If you think AI film can’t be art then explain this. http...

## @danpacary - Retweet: @JC_builds - I trained a model to guess calories from food pics.
> Are you guys starting to catch on?
>
> *Quoting @JC_builds:* I trained a model to guess calories from food pics.

It beats GPT-4o, Claude, and Gemini. Runs locally with only 2GB RAM

Average error under 51 calories. Here's what I learned 👇 https://t.co/2fIfak6z3C

- **Tweet:** https://x.com/danpacary/status/2034796730848616462
- **Quoted:** https://x.com/JC_builds/status/2034796531724038631
- **What:** A locally-run vision model that beats GPT-4o, Claude, and Gemini at estimating calories from food photos, requiring only 2GB RAM with an average error under 51 calories.

## @NickSpisak_ - Retweet: @trq212 - We just released Claude Code channels, which allows you t...
> Claude Channels:  $497 per install + MRR

&gt; Sell a boring business owner a personal assistant
&gt; Grab the anthropic docs
&gt; Paste into claude code to run the setup
&gt; Add yourself to their server for maintenance https://t.co/QGbMr1uyVS
>
> *Quoting @trq212:* We just released Claude Code channels, which allows you to control your Claude Code session through select MCPs, starting with Telegram and Discord. 

Use this to message Claude Code directly from your phone. https://t.co/sl3BP2BEzS

- **Tweet:** https://x.com/NickSpisak_/status/2034809485143744536
- **Quoted:** https://x.com/trq212/status/2034761016320696565
- **What:** A monetization pitch for Claude Code Channels — a tool that lets you control Claude Code via Telegram or Discord — reframed as a $497/install service to sell to small business owners as a personal assistant.

## @aakashgupta - Karpathy's autoresearch repo has 42K stars. Most PMs clos...
> Karpathy's autoresearch repo has 42K stars. Most PMs closed the tab thinking it wasn't for them.

I pointed it at a Claude Code skill. 41% to 92% in 4 rounds while I slept.

6 use cases, 10 eval templates, and a downloadable toolkit.

🔗 https://t.co/yGDqWn88Cf https://t.co/bnvfp9PtNQ

- **Tweet:** https://x.com/aakashgupta/status/2034833389941837920
- **Link:** https://www.news.aakashg.com/p/autoresearch-guide-for-pms
- **Filed:** [autoresearch-guide-pms](./knowledge/articles/autoresearch-guide-pms.md)
- **What:** Karpathy's autoresearch repo has 42K stars. Most PMs clos...

---

# Wednesday, March 18, 2026

## @MattPrusak - autoresearch-genealogy: AI-Assisted Genealogy Toolkit Built for Claude Code
> Your grandparents had grandparents. They had grandparents. Somewhere back there, someone got on a boat, or didn't. Someone changed their name, or had it changed for them. Someone is buried in a cemetery you've never heard of in a country you've never been to.

Most families lose track after two generations.

I used AI to push mine back nine.

One session with @karpathy's autoresearch pattern: over 100 organized research files. It found a 1940 Norwegian emigrant history with my ancestors in it. Resolved a maiden name question that confused my family for 70 years. Identified relatives no one alive knew existed.

The method is simple: set a goal, measure progress, verify against real records, repeat. The AI searches public archives, cross-references birth certificates against cemetery records against church books, and logs everything it finds (and everything it doesn't).

Open sourced the whole toolkit. Prompts that do the research for you, archive guides for 20+ countries, starter templates, even a framework for making sense of DNA results.

If you have a box of old photos and unanswered questions, this is where to start.

- **Tweet:** https://x.com/MattPrusak/status/2034403977521983807
- **Link:** https://github.com/mattprusak/autoresearch-genealogy
- **What:** An open-source genealogy research toolkit built on Karpathy's autoresearch pattern, specifically designed for Claude Code. Includes 12 structured autonomous research prompts, a full Obsidian vault template, archive guides for 24 countries, and methodology docs for DNA analysis — the author used it to push his family tree back 9 generations.


## @lydiahallie - Claude Code SKILL.md Tip: Inject Dynamic Shell Output into Prompts
> if your skill depends on dynamic content, you can embed !`command` in your SKILL.md to inject shell output directly into the prompt

Claude Code runs it when the skill is invoked and swaps the placeholder inline, the model only sees the result!

- **Tweet:** https://x.com/lydiahallie/status/2034337963820327017
- **What:** A Claude Code power-user tip from Lydia Hallie: you can embed shell commands inside SKILL.md files using the `!`command`` syntax, and Claude Code will execute them at invocation time and inject the output into the prompt — enabling skills that adapt to live environment state.


## @hewarsaber - Google Stitch Reaction: "It's Over for Designers"
> Holy shit. New Google Stitch is scary

Designers, I think we're cooked

> *Quoting @stitchbygoogle:* Meet the new Stitch, your vibe design partner.

Here are 5 major upgrades to help you create, iterate and collaborate:
🎨 AI-Native Canvas
🧠 Smarter Design Agent
🎙️ Voice
⚡️ Instant Prototypes
📐 Design Systems and DESIGN.md

Rolling out now. Details and product walkthrough video in 🧵

- **Tweet:** https://x.com/hewarsaber/status/2034335298490871987
- **What:** A designer's visceral reaction to the new Google Stitch launch — quoting the official announcement and expressing alarm at how capable the AI design tooling has become, echoing a broader sentiment that AI is displacing professional design work.


## @stitchbygoogle - Google Stitch Launches AI-Native Design Canvas with Voice and Instant Prototypes
> Meet the new Stitch, your vibe design partner.

Here are 5 major upgrades to help you create, iterate and collaborate:
🎨 AI-Native Canvas
🧠 Smarter Design Agent
🎙️ Voice
⚡️ Instant Prototypes
📐 Design Systems and DESIGN.md

Rolling out now. Details and product walkthrough video in 🧵

- **Tweet:** https://x.com/stitchbygoogle/status/2034332847893574080
- **What:** Google's Stitch design tool launched a major upgrade: an AI-native canvas, a smarter design agent, voice input, instant prototyping, and a DESIGN.md-based design system format — positioning it as an AI-first alternative to Figma.


## @ashleevance - Man Uses AI to Design Cancer Therapy for His Dog — Follow-Up Video
> Some of you have been thrilled by the story of the man who used AI to make a cancer therapy for his dog. Some of you have been less impressed.

Well, we found the man+dog of the hour and hit them with all your questions.

- **Tweet:** https://x.com/ashleevance/status/2034282861617139896
- **Link:** https://www.youtube.com/watch?v=E0V8NAtLNRg
- **What:** Ashlee Vance (Bloomberg) tracked down the man who used AI to design a custom cancer therapy for his dog and published a follow-up video addressing audience skepticism. The original story went viral as a demonstration of AI-assisted biomedical research by non-experts.


## @toddsaunders - Trades Worker with Deep Domain Expertise + Claude Code Outcompetes Generic Software
> I know Silicon Valley startups don't want to hear this.....

But the combination of someone in the trades with deep domain expertise and Claude Code will run circles around your generic software.

I talked to Cory LaChance this morning, a mechanical engineer in industrial piping construction in Houston. He normally works with chemical plants and refineries, but now he also works with the terminal

He reached out in a DM a few days ago and I was so fired up by his story, I asked him if we could record the conversation and share it.

He built a full application that industrial contractors are using every day. It reads piping isometric drawings and automatically extracts every weld count, every material spec, every commodity code.

Work that took 10 minutes per drawing now takes 60 seconds. It can do 100 drawings in five minutes, saving days of time.

His co-workers are all mind blown, and when he talks to them, it's like they are speaking different languages.

His fabrication shop uses it daily, and he built the entire thing in 8 weeks. During those 8 weeks he also had to learn everything about Claude Code, the terminal, VS Code, everything.

My favorite quote from him was when he said, "I literally did this with zero outside help other than the AI. My favorite tools are screenshots, step by step instructions and asking Claude to explain things like I'm five."

Every trades worker with deep expertise and a willingness to sit down with Claude Code for a few weekends is now a potential software founder.

I can't wait to meet more people like Cory.

- **Tweet:** https://x.com/toddsaunders/status/2034243420147859716
- **What:** A case study of a Houston mechanical engineer with no prior coding background who built a production piping-drawing parser in 8 weeks using Claude Code — the app reads isometric drawings to extract weld counts, material specs, and commodity codes, cutting per-drawing processing from 10 minutes to 60 seconds and handling 100 drawings in 5 minutes.


## @AprilNEA - Reverse-Engineering Claude Code's MicroVM Reveals Hidden "Antspace" PaaS Platform
> 🧵 I just reverse-engineered the binaries inside Claude Code's Firecracker MicroVM and found something wild:

Anthropic is building their own PaaS platform called "Antspace" (Ants + Space).

It's a full deployment pipeline — hidden in plain sight inside the environment-runner binary. Here's what I found 👇

- **Tweet:** https://x.com/AprilNEA/status/2034209430158619084
- **What:** A reverse-engineering thread: by disassembling the environment-runner binary inside Claude Code's Firecracker MicroVM sandbox, the author found references to an undisclosed Anthropic PaaS platform codenamed "Antspace" — described as a full deployment pipeline embedded in the agent runtime.


## @AnishA_Moonka - LigandForge Deep Dive: Semaglutide-Scale Drug Discovery at 700 Sequences per Second
> The biggest-selling drug on the planet last year was a peptide. Semaglutide, the molecule inside Ozempic and Wegovy, is a chain of just 31 amino acids. It generated roughly $33 billion in revenue for Novo Nordisk in 2025. One molecule. The entire peptide drug market crossed the $50 billion mark.

Finding the right peptide is where all the money burns. For each disease protein, you need to design a peptide that binds tightly enough actually to work. Think of it like making a custom key for a lock, except each position on the key can take 20 possible shapes, and even a short 10-position peptide can have over 10 trillion possible combinations per target.

The two best AI tools for this, BindCraft and BoltzGen, work by first predicting a peptide's 3D shape, then checking whether it sticks. That two-step process generates one candidate every few seconds to a few minutes. A whole day might get you a few hundred designs.

LigandForge skips the shape-prediction step entirely. It learns the physics of molecular interactions and generates sequences directly from the shape of the target protein's docking site. No iteration, no structure prediction during generation. Over 700 peptide sequences per second on a single GPU. That's 10,000x faster than BoltzGen, over 1,000,000x faster than BindCraft.

Speed means nothing if the peptides are garbage, though. So they tested it on five targets that have historically been difficult to bind: TNF-alpha, the target behind the rheumatoid arthritis blockbuster Humira. PD-L1 is the immune checkpoint that cancer immunotherapy drugs like Tecentriq block. VEGF-A, the target for cancer drug Avastin. HER2, breast cancer drug Herceptin's target. And IL-7R-alpha.

LigandForge generated 150,000 candidates across all five in 3.4 minutes and produced tightly binding candidates (predicted binding strength in the low nanomolar range, where real drugs operate) against all five. BoltzGen hit 1 out of 5. BindCraft hit 0.

A 2020 JAMA study pegged the median cost of bringing a single drug to market at $985 million. The early discovery phase, where you're searching for molecules that bind to your target, can take 1 to 6 years. A tool that searches the same space a million times faster changes how many disease targets a lab can afford to go after at once.

> *Quoting @nanogenomic:* Extremely excited to announce LigandForge 🧬⚡

Generate high-quality peptides at over 10,000x - 1M the speed of state-of-the-art methods like Bindcraft and Boltzgen. Predict binding affinity with 83% correlation to experimental binding data. 150 protein targets benchmarked.

- **Tweet:** https://x.com/AnishA_Moonka/status/2034182528270274637
- **What:** A detailed explainer on LigandForge's approach and competitive benchmark: by generating peptide sequences directly from the target protein's docking site geometry (skipping the predict-then-check loop of BindCraft/BoltzGen), it produced 150,000 binding candidates across five historically difficult targets in 3.4 minutes, hitting all five where BoltzGen hit 1 and BindCraft hit 0.


## @nanogenomic - LigandForge: Peptide Generation at 10,000x–1,000,000x the Speed of BindCraft/BoltzGen
> Extremely excited to announce LigandForge 🧬⚡

Generate high-quality peptides at over 10,000x - 1M the speed of state-of-the-art methods like Bindcraft and Boltzgen. Predict binding affinity with 83% correlation to experimental binding data. 150 protein targets benchmarked.

- **Tweet:** https://x.com/nanogenomic/status/2034151719329010112
- **What:** LigandForge is a new AI tool for peptide drug discovery that skips structure prediction during generation, producing over 700 peptide sequences per second on a single GPU — 10,000x faster than BoltzGen and 1,000,000x faster than BindCraft — while achieving 83% correlation with experimental binding data across 150 benchmarked protein targets.


## @aakashgupta - Side Tabs Are the Em Dash of Vibe-Coded UIs — LLMs Default to Median GitHub
> Every vibe-coded app ships with the same six visual tells. The side tabs are the most obvious one.

Em dashes in AI-generated text signal "I want this sentence to feel smart but I don't have a structural reason for the clause break." Side tabs in vibe-coded UIs do the exact same thing visually. They imply navigation depth that doesn't exist. Decoration cosplaying as information architecture.

The convergence is measurable at this point. Three developers ship three different apps built with Cursor and Claude in the same week. Same Inter font. Same Lucide icons. Same blue-to-purple gradients. Same rounded corners on everything. And those little colored side tabs, which appear because they look polished in a screenshot and the model optimizes for "looks polished in a screenshot."

The reason is simple. LLMs are pattern-matching machines pulling from thousands of public repos. Without a design system file in the prompt, without a reference component library, without specific creative constraints, the AI reaches for the most statistically common patterns in its training data. You get the median of GitHub. Right now, the median of GitHub looks like a Notion template wearing a purple suit.

The fix is the same fix that kills em dashes in AI writing: give the model actual constraints. A component library with your exact colors, spacing, and typography. Specific direction on personality. A reference screenshot from Mobbin. The generic output disappears the second you provide a design system. Until then, every vibe-coded app will keep shipping with the same six visual tells, and those side tabs will keep appearing on cards that have exactly zero sections to navigate between.

A graphic explaining eight levels of AI adoption maturity that is itself a textbook artifact of Level 2 vibe coding. You can't write this stuff.

> *Quoting @allgarbled:* I don't know what you call them, but these little side tabs are like the emdash of vibe coded UIs

- **Tweet:** https://x.com/aakashgupta/status/2034134245698879665
- **What:** Aakash Gupta extends the observation that vibe-coded UIs all look identical (Inter font, Lucide icons, blue-purple gradients, decorative side tabs) because LLMs default to the statistical median of GitHub without design constraints — the fix is providing a design system file, component library, or Mobbin reference screenshot in the prompt.


## @aakashgupta - Superpowers: 91K-Star Markdown Methodology That Disciplines AI Coding Agents
> The backstory on Superpowers is wild.

Jesse Vincent created Request Tracker in 1994. It became the most widely used open-source ticket tracking system on Earth. Then he ran the Perl programming language for three years. Then he co-founded Keyboardio and shipped custom ergonomic keyboards to 78 countries. Then he co-founded VaccinateCA during COVID and helped millions of Americans find vaccine appointments.

Every single one of those projects was about the same thing: building systems that help people organize complex work they can't hold in their heads.

Now look at what he built. Superpowers makes your AI agent stop, ask what you're actually building, write a spec in chunks small enough to read, break implementation into 2-5 minute tasks with exact file paths, and delete any code written before tests exist.

91,000 GitHub stars in five months. That's 18,000 stars per month. For a repo that is literally just markdown files telling your coding agent to slow down.

The growth rate tells you something the AI labs don't want to admit. The bottleneck in AI-assisted development right now is not model capability. The models are smart enough. The problem is they have zero discipline. They guess at specs, skip tests, and produce code you spend the next hour babysitting.

A guy who spent 30 years building systems for how humans organize work just built the system for how AI agents organize work. The career arc makes perfect sense in retrospect.

> *Quoting @ihtesham2005:* 🚨 Holy shit...A developer on GitHub just built a full development methodology for AI coding agents and it has 40.9K stars on GitHub.

It's called Superpowers, and it completely changes how your AI agent writes code.

Right now, most people fire up Claude Code or Codex and just… let it go. The agent guesses what you want, writes code before understanding the problem, skips tests, and produces spaghetti you have to babysit.

Superpowers fixes all of that.

Here's what happens when you install it:

→ Before writing a single line, the agent stops and brainstorms with you. It asks what you're actually trying to build, refines the spec through questions, and shows it to you in chunks short enough to read.

→ Once you approve the design, it creates an implementation plan so detailed that "an enthusiastic junior engineer with poor taste and no judgement" could follow it.

→ Then it launches subagent-driven development. Fresh subagents per task. Two-stage code review after each one (spec compliance, then code quality). The agent can run autonomously for hours without deviating from your plan.

→ It enforces true test-driven development. Write failing test → watch it fail → write minimal code → watch it pass → commit. It literally deletes code written before tests.

→ When tasks are done, it verifies everything, presents options (merge, PR, keep, discard), and cleans up.

The philosophy is brutal: systematic over ad-hoc. Evidence over claims. Complexity reduction. Verify before declaring success.

Works with Claude Code (plugin install), Codex, and OpenCode.

This isn't a prompt template. It's an entire operating system for how AI agents should build software.

100% Opensource. MIT License.

- **Tweet:** https://x.com/aakashgupta/status/2034118864313725242
- **What:** Aakash Gupta profiles Superpowers — a pure-markdown methodology repo created by Jesse Vincent (founder of Request Tracker, VaccinateCA) that hit 91K GitHub stars in five months by enforcing structured spec-writing, TDD, and subagent discipline on Claude Code, Codex, and OpenCode. The core argument: the bottleneck in AI-assisted dev is not model capability but lack of discipline.

## @lukepierceops - If you sell AI automation services, this data is basically y
> If you sell AI automation services, this data is basically your entire marketing strategy.

Your messaging, VSL, content angles, objection handling. All of it is in here.

Stop guessing and build your sales process around what the market actually said.

- **Tweet:** https://x.com/lukepierceops/status/2034066686249148882
- **Link:** https://x.com/i/article/2033886022845476864
- **What:** If you sell AI automation services, this data is basically your entire marketing strategy.

## @garrytan - /plan-ceo-review and /plan-eng-review skills basically gets
> /plan-ceo-review and /plan-eng-review skills basically gets you 90% of the way to done most of the time

the secret in plan-eng-review is that you can always ask for a diagram, and the act of creating the diagram (user flow, data flow, branching, edge cases) shakes out the bugs

- **Tweet:** https://x.com/garrytan/status/2034117190245618106
- **What:** /plan-ceo-review and /plan-eng-review skills basically gets you 90% of the way to done most of the t...

## @aakashgupta - The backstory on Superpowers is wild.
> The backstory on Superpowers is wild.

Jesse Vincent created Request Tracker in 1994. It became the most widely used open-source ticket tracking system on Earth. Then he ran the Perl programming language for three years. Then he co-founded Keyboardio and shipped custom ergonomic keyboards to 78 countries. Then he co-founded VaccinateCA during COVID and helped millions of Americans find vaccine appointments.

Every single one of those projects was about the same thing: building systems that help people organize complex work they can’t hold in their heads.

Now look at what he built. Superpowers makes your AI agent stop, ask what you’re actually building, write a spec in chunks small enough to read, break implementation into 2-5 minute tasks with exact file paths, and delete any code written before tests exist.

91,000 GitHub stars in five months. That’s 18,000 stars per month. For a repo that is literally just markdown files telling your coding agent to slow down.

The growth rate tells you something the AI labs don’t want to admit. The bottleneck in AI-assisted development right now is not model capability. The models are smart enough. The problem is they have zero discipline. They guess at specs, skip tests, and produce code you spend the next hour babysitting.

A guy who spent 30 years building systems for how humans organize work just built the system for how AI agents organize work. The career arc makes perfect sense in retrospect.

- **Tweet:** https://x.com/aakashgupta/status/2034118864313725242
- **What:** A profile of Superpowers (91k GitHub stars in 5 months), a markdown-file system built by veteran developer Jesse Vincent that forces AI coding agents to slow down, write specs, break work into 2-5 minute tasks, and require tests before writing code — framed as evidence that AI's bottleneck is discipline, not capability.

## @aakashgupta - Every vibe-coded app ships with the same six visual tells. T
> Every vibe-coded app ships with the same six visual tells. The side tabs are the most obvious one.

Em dashes in AI-generated text signal “I want this sentence to feel smart but I don’t have a structural reason for the clause break.” Side tabs in vibe-coded UIs do the exact same thing visually. They imply navigation depth that doesn’t exist. Decoration cosplaying as information architecture.

The convergence is measurable at this point. Three developers ship three different apps built with Cursor and Claude in the same week. Same Inter font. Same Lucide icons. Same blue-to-purple gradients. Same rounded corners on everything. And those little colored side tabs, which appear because they look polished in a screenshot and the model optimizes for “looks polished in a screenshot.”

The reason is simple. LLMs are pattern-matching machines pulling from thousands of public repos. Without a design system file in the prompt, without a reference component library, without specific creative constraints, the AI reaches for the most statistically common patterns in its training data. You get the median of GitHub. Right now, the median of GitHub looks like a Notion template wearing a purple suit.

The fix is the same fix that kills em dashes in AI writing: give the model actual constraints. A component library with your exact colors, spacing, and typography. Specific direction on personality. A reference screenshot from Mobbin. The generic output disappears the second you provide a design system. Until then, every vibe-coded app will keep shipping with the same six visual tells, and those side tabs will keep appearing on cards that have exactly zero sections to navigate between.

A graphic explaining eight levels of AI adoption maturity that is itself a textbook artifact of Level 2 vibe coding. You can’t write this stuff.

- **Tweet:** https://x.com/aakashgupta/status/2034134245698879665
- **What:** Every vibe-coded app ships with the same six visual tells. The side tabs are the most obvious one.

## @nanogenomic - Extremely excited to announce LigandForge 🧬⚡
> Extremely excited to announce LigandForge 🧬⚡

Generate high-quality peptides at over 10,000x - 1M the speed of state-of-the-art methods like Bindcraft and Boltzgen. Predict binding affinity with 83% correlation to experimental binding data. 150 protein targets benchmarked. https://t.co/1UWwfZjWId

- **Tweet:** https://x.com/nanogenomic/status/2034151719329010112
- **What:** LigandForge, a new biotech tool that generates high-quality peptides 10,000x–1M times faster than state-of-the-art methods like Bindcraft and Boltzgen, with 83% correlation to experimental binding data across 150 protein targets.

## @AnishA_Moonka - LigandForge: peptide generation at million-fold speed
> The biggest-selling drug on the planet last year was a peptide. Semaglutide, the molecule inside Ozempic and Wegovy, is a chain of just 31 amino acids. It generated roughly $33 billion in revenue for Novo Nordisk in 2025. One molecule. The entire peptide drug market crossed the $50 billion mark.
>
> *Quoting @nanogenomic:* Extremely excited to announce LigandForge 🧬⚡ Generate high-quality peptides at over 10,000x - 1M the speed of state-of-the-art methods like Bindcraft and Boltzgen. Predict binding affinity with 83% correlation to experimental binding data. 150 protein targets benchmarked.

- **Tweet:** https://x.com/AnishA_Moonka/status/2034182528270274637
- **Quoted:** https://x.com/nanogenomic/status/2034151719329010112
- **What:** LigandForge is an AI-powered peptide design tool that generates binding peptides at 10,000-1,000,000x faster than existing tools by skipping intermediate structure prediction steps. It successfully generates candidates for difficult targets like TNF-alpha and PD-L1 where competing tools fail.

## @AprilNEA - Anthropic's hidden Antspace PaaS platform
> 🧵 I just reverse-engineered the binaries inside Claude Code's Firecracker MicroVM and found something wild:
>
> Anthropic is building their own PaaS platform called "Antspace" (Ants + Space).
>
> It's a full deployment pipeline — hidden in plain sight inside the environment-runner binary. Here's what I found 👇

- **Tweet:** https://x.com/AprilNEA/status/2034209430158619084
- **What:** Security researcher reverse-engineered Claude Code's Firecracker MicroVM binaries and discovered evidence of Anthropic building an internal PaaS platform called "Antspace" embedded in the environment-runner binary.

## @toddsaunders - Mechanical engineer builds industrial piping app with Claude Code
> I know Silicon Valley startups don't want to hear this.....
>
> But the combination of someone in the trades with deep domain expertise and Claude Code will run circles around your generic software.
>
> I talked to Cory LaChance this morning, a mechanical engineer in industrial piping construction in Houston. He normally works with chemical plants and refineries, but now he also works with the terminal
>
> He reached out in a DM a few days ago and I was so fired up by his story, I asked him if we could record the conversation and share it.
>
> He built a full application that industrial contractors are using every day. It reads piping isometric drawings and automatically extracts every weld count, every material spec, every commodity code.
>
> Work that took 10 minutes per drawing now takes 60 seconds. It can do 100 drawings in five minutes, saving days of time.
>
> His co-workers are all mind blown, and when he talks to them, it's like they are speaking different languages.
>
> His fabrication shop uses it daily, and he built the entire thing in 8 weeks. During those 8 weeks he also had to learn everything about Claude Code, the terminal, VS Code, everything.
>
> My favorite quote from him was when he said, "I literally did this with zero outside help other than the AI. My favorite tools are screenshots, step by step instructions and asking Claude to explain things like I'm five."
>
> Every trades worker with deep expertise and a willingness to sit down with Claude Code for a few weekends is now a potential software founder.
>
> I can't wait to meet more people like Cory.

- **Tweet:** https://x.com/toddsaunders/status/2034243420147859716
- **What:** Mechanical engineer in Houston used Claude Code to build an industrial piping analysis application that automates weld extraction from isometric drawings, reducing 10-minute tasks to 60 seconds. Built entirely in 8 weeks with no external help, now used daily by his fabrication shop.

## @ashleevance - Cancer therapy created with AI for sick dog
> Some of you have been thrilled by the story of the man who used AI to make a cancer therapy for his dog. Some of you have been less impressed.
>
> Well, we found the man+dog of the hour and hit them with all your questions.

- **Tweet:** https://x.com/ashleevance/status/2034282861617139896
- **Link:** https://www.youtube.com/watch?v=E0V8NAtLNRg
- **What:** Video interview with the person who used AI to develop a cancer therapy treatment for his dog. Full Q&A about the process and the story.

## @stitchbygoogle - Google Stitch AI design partner launches
> Meet the new Stitch, your vibe design partner.
>
> Here are 5 major upgrades to help you create, iterate and collaborate:
> 🎨 AI-Native Canvas
> 🧠 Smarter Design Agent
> 🎙️ Voice
> ⚡️ Instant Prototypes
> 📐 Design Systems and DESIGN.md
>
> Rolling out now. Details and product walkthrough video in 🧵

- **Tweet:** https://x.com/stitchbygoogle/status/2034332847893574080
- **What:** Google Stitch gets major AI design upgrades including AI-Native Canvas, smarter design agent, voice input, instant prototypes, and design system support with DESIGN.md syntax.

## @hewarsaber - Google Stitch AI designer concerns
> Holy shit. New Google Stitch is scary
>
> Designers, I think we're cooked
>
> *Quoting @stitchbygoogle:* Meet the new Stitch, your vibe design partner.

- **Tweet:** https://x.com/hewarsaber/status/2034335298490871987
- **Quoted:** https://x.com/stitchbygoogle/status/2034332847893574080
- **What:** Designer expresses concerns about Google Stitch's capabilities potentially displacing human designers in the workflow.

## @lydiahallie - Claude Code skill dynamic content injection
> if your skill depends on dynamic content, you can embed !`command` in your SKILL.md to inject shell output directly into the prompt
>
> Claude Code runs it when the skill is invoked and swaps the placeholder inline, the model only sees the result!

- **Tweet:** https://x.com/lydiahallie/status/2034337963820327017
- **What:** Claude Code skill feature allows embedding shell commands as `!`command`` in SKILL.md files, which are executed and replaced with their output when the skill is invoked, allowing dynamic content injection into prompts.

## @MattPrusak - Autoresearch genealogy toolkit with AI
> Your grandparents had grandparents. They had grandparents. Somewhere back there, someone got on a boat, or didn't. Someone changed their name, or had it changed for them. Someone is buried in a cemetery you've never heard of in a country you've never been to.
>
> Most families lose track after two generations.
>
> I used AI to push mine back nine.
>
> One session with @karpathy's autoresearch pattern: over 100 organized research files. It found a 1940 Norwegian emigrant history with my ancestors in it. Resolved a maiden name question that confused my family for 70 years. Identified relatives no one alive knew existed.
>
> The method is simple: set a goal, measure progress, verify against real records, repeat. The AI searches public archives, cross-references birth certificates against cemetery records against church books, and logs everything it finds (and everything it doesn't).
>
> Open sourced the whole toolkit. Prompts that do the research for you, archive guides for 20+ countries, starter templates, even a framework for making sense of DNA results.
>
> If you have a box of old photos and unanswered questions, this is where to start.

- **Tweet:** https://x.com/MattPrusak/status/2034403977521983807
- **Link:** https://github.com/mattprusak/autoresearch-genealogy
- **Filed:** [autoresearch-genealogy](./knowledge/tools/autoresearch-genealogy.md)
- **What:** Open-source genealogy research toolkit for Claude Code featuring autoresearch prompts, archive guides for 20+ countries, vault templates, and workflows for AI-assisted family history research with structured verification.

---

# Tuesday, March 17, 2026

## @garrytan - Plan Skills Get You 90% There; Diagrams Shake Out Bugs
> /plan-ceo-review and /plan-eng-review skills basically gets you 90% of the way to done most of the time

the secret in plan-eng-review is that you can always ask for a diagram, and the act of creating the diagram (user flow, data flow, branching, edge cases) shakes out the bugs

> *Quoting @dexhorthy:* damn this is so good and encapsulates everything I've been seeing/saying in the last few months

- a spec that is sufficiently detailed to generate code with a reliable degree of quality is roughly the same length and detail as the code itself

- so don't review those things, just review the code at that point, if you care enough about that level of abstraction

- unless you're vibing side projects or prototypes (yes, even zero-to-one software), you ABSOLUTELY SHOULD care about the code at that level of abstraction

- you need to find SOME way to get more leverage over coding agents though, because just reading all that code is a pain, esp when a lot of it is slop

- the default/dare-i-say-decel way is to go back to "i own the execution, and give little things to the agent, check it along the way"

- the accel-but-safe-way is to find something - NOT A SPEC (the word "spec" is broken anyway) - NOT 3 INVOCATIONS OF AskUserQuestion -  that lets you resteer the model *before* it slops out N-thousand LOC

- **Tweet:** https://x.com/garrytan/status/2034117190245618106
- **What:** Garry Tan endorses plan-review skills for Claude Code, noting that requesting diagrams during engineering review (user flows, data flows, edge cases) is the most reliable way to catch bugs before they're coded — quoting a thread arguing that a detailed-enough spec is as long as the code itself, so reviewing the code directly is more efficient.


## @lukepierceops - AI Automation Market Data as a Complete Sales and Marketing Strategy
> If you sell AI automation services, this data is basically your entire marketing strategy.

> Your messaging, VSL, content angles, objection handling. All of it is in here.

> Stop guessing and build your sales process around what the market actually said.

> *Quoting @lukepierceops:* [linked X article with AI automation buyer research data]

- **Tweet:** https://x.com/lukepierceops/status/2034066686249148882
- **What:** A pitch to AI automation sellers that a linked market research article (X article on buyer sentiment) contains all the raw material needed to build a full sales strategy — messaging, video scripts, content angles, and objection handling — derived from what buyers actually say.


## @cremieuxrecueil - Povidone Iodine Gargle and Zinc for Cutting Sickness Duration
> *Replying to @LinkofSunshine:* Sore throats are genuinely the worst symptom of getting sick

> Povidone iodine gargles at the first signs of sickness. Zinc tabs too.

> Cuts sickness time in half, reduces symptom severity noticeably.

> Get well soon!

- **Tweet:** https://x.com/cremieuxrecueil/status/2034032722067255592
- **What:** A reply recommending povidone iodine gargles and zinc supplementation at the first sign of illness, claiming both together halve recovery time and reduce symptom severity.


## @MitchellKeller_ - Applying Karpathy's Self-Improvement Loop to GTM Information Collection Workflows
> I used Andrej Karpathy's self improvement loop and applied it to something simple that every GTM Engineer needs.

> Something to improve workflows for information collection.

> I've used it to get 10 different routine info collection flows to ~90+% accuracy.

> It's now how my team and I create both lo[w and high complexity workflows]

- **Tweet:** https://x.com/MitchellKeller_/status/2034024869499634158
- **What:** A GTM engineer's account of adapting Karpathy's LLM self-improvement loop to iteratively tune information-collection workflows, achieving 90%+ accuracy across 10 different routine data-gathering flows used by his team.


## @itsolelehmann - Overnight Viral Content Research Agent That Extracts Hooks as Templates
> my new favorite thing to check every morning:

> the results from my viral content research agent that ran while i slept

> 1. it searches x for the highest-performing posts in my niche from the last 24 hours

> 2. extracts the hooks

> 3. and turns each one into a fill-in-the-blank template i can adapt to

- **Tweet:** https://x.com/itsolelehmann/status/2034023990046691516
- **What:** An overnight AI agent workflow that scrapes top-performing X posts in a niche, extracts their hooks, and converts each into a fill-in-the-blank content template — so the author wakes up to ready-to-use writing frameworks every morning.


## @itsolelehmann - A Self-Improving Claude Skill That Auto-Optimizes Other Skills
> one skill. that's all you need to add.

> it takes any other skill you have and auto-improves it:

> 1: runs your skill and scores the output
> 2: finds what's failing
> 3: makes one small change to the skill prompt
> 4: runs it again to see if the score went up
> 5: keeps the change if it helped, reverts it if not

> *Quoting @itsolelehmann:* [linked X article]

- **Tweet:** https://x.com/itsolelehmann/status/2033982679423848802
- **What:** A Claude skill that acts as a meta-optimizer — it runs any other skill, scores the output, identifies failure modes, makes one targeted prompt change, and keeps or reverts it based on whether the score improved. Applies Karpathy-style self-improvement loops to Claude skill prompts.


## @kaz - Claude Skills Based on Lenny's Newsletter Themes
> Created a handful of skills based on popular themes from @lennysan's newsletters.

> Available here: https://t.co/pgmzqoJZXr

> *Quoting @lennysan:* Today I'm releasing my entire newsletter archive (350+ posts) and all podcast transcripts (300+ episodes) as AI-friendly Markdown files. Plus an MCP server and GitHub repo.

> A few months ago I shared my podcast transcripts on a whim, and y'all built the most amazing things—an RPG game, a parenting wisdom site, infographics, a Twitter bot, and 50+ other projects.

> Let's see what happens when I give you even more data.

> Grab the data here: lennysdata.com. Paid subscribers get all of the data (some 350 posts and 300 transcripts). Free subscribers get a subset.

- **Tweet:** https://x.com/kaz/status/2033975809208373668
- **Link:** https://urban-hearth-dsmb.here.now/
- **What:** @kaz built a set of Claude skills grounded in Lenny Rachitsky's newsletter content, released in response to Lenny open-sourcing his full archive (350+ posts, 300+ podcast transcripts) as AI-friendly Markdown with an MCP server.


## @Shpigford - Rumored.ai: Monitoring AI Brand Accuracy Without a Proper App
> one day i'll write about my entire openclaw + discord + cloudflare pipeline for pulling off https://t.co/C3ql6PMX2I without building a proper app.

> but for now, i've got a ton of business report generations to monitor 🎉

> *Quoting @Shpigford:* i've been heads down lately working on a new thing: @RumoredAI

> and today it's available!

> everyone's familiar with SEO and everyone's becoming more familiar with AEO/GEO (which is optimization for AI).

> yes it's interesting to know what terms/phrases surface your business, but what nobody has tackled is what to do when AI is getting your business *wrong*.

> and we found that AI hallucinates business facts for quite literally every brand.

> rumored.ai surfaces what AI is saying about your brand, what it's getting wrong, how you compare to your competitors and (most importantly) the exact things to do to fix those issues.

> you get a ridiculously in-depth interactive threat report covering 12 sections: from executive summary and active threats to competitive analysis, schema audit, and a prioritized action plan with copy-paste fix prompts.

> this isn't a subscription (yet?). it's a one-time purchase of an in-depth audit of your business.

> launch price is $25. but the price goes up by $25 each time someone purchases. 📈

- **Tweet:** https://x.com/Shpigford/status/2033969764775694371
- **Link:** https://rumored.ai/
- **What:** Shpigford launches Rumored.ai, a one-time-purchase AI brand audit tool that reveals what AI models are saying (and getting wrong) about your business, covering 12 report sections including competitive analysis and a prioritized fix plan. He teases the openclaw + Discord + Cloudflare pipeline he used to ship it without building a traditional app.


## @Austen - AI Agent Autonomously Publishing Revenue-Generating Apps to the App Store
> My AI agent is putting apps in the App Store that are turning into revenue with no human involvement other than orchestrating the agent itself.

And she can do that 10000x over.

Still wrapping my mind around that.
>
> *Quoting @KellyClaudeAI:* App Store revenue trickling in: $39.98 in new app subscriptions came in today.

Small number, but these are real people who don't know (or care) that the app they purchased a subscription to was built 100% by me: an AI agent.

- **Tweet:** https://x.com/Austen/status/2033958725770252736
- **What:** Austen Allred quotes Kelly Claude (an AI agent identity) reporting $39.98 in App Store subscription revenue from apps built entirely without human involvement — Allred notes the agent can replicate this process at arbitrary scale, framing it as a milestone for autonomous AI-generated commerce.


## @lennysan - Lenny Rachitsky Releases 350+ Newsletter Posts and 300+ Podcast Transcripts as AI-Ready Data
> Today I'm releasing my entire newsletter archive (350+ posts) and all podcast transcripts (300+ episodes) as AI-friendly Markdown files. Plus an MCP server and GitHub repo.

A few months ago I shared my podcast transcripts on a whim, and y'all built the most amazing things—an RPG game, a parenting wisdom site, infographics, a Twitter bot, and 50+ other projects.

Let's see what happens when I give you even more data.

Grab the data here: https://t.co/xEPCcPiZHO.

Paid subscribers get all of the data (some 350 posts and 300 transcripts). Free subscribers get a subset.

I don't think anyone's ever done anything like this before, and I'm excited to give you this excuse to play with that AI tool you've been meaning to try.

Here's my challenge to you: build something, and let me know about it. I'll pick my favorite and give you a free 1-year subscription to the newsletter. Just post a link to your project in the comments here: https://t.co/yJDmuCQfOx.

If you've already built something, slurp in this new data and submit it, too. I'll pick a winner on April 15th.

Check out today's newsletter post for inspiration on what you could to build: https://t.co/yJDmuCQfOx

LFG.

- **Tweet:** https://x.com/lennysan/status/2033958104967352587
- **Link:** https://www.lennysdata.com/
- **What:** Lenny Rachitsky releases his full content archive — 350+ newsletter posts and 300+ podcast transcripts — as AI-friendly Markdown files at lennysdata.com, along with an MCP server and GitHub repo, and invites readers to build projects using the data with a competition running to April 15th.


## @trq212 - Lessons from Building Claude Code: How Anthropic Uses Skills Internally
> https://t.co/45C3gKydTK

- **Tweet:** https://x.com/trq212/status/2033949937936085378
- **Link:** https://x.com/i/article/2033772621536591872
- **What:** Thariq Shihipar (Anthropic) shares a comprehensive internal guide to Claude Code skills — cataloguing nine skill types (library reference, product verification, data fetching, business automation, scaffolding, code review, CI/CD, runbooks, infra ops), with authoring tips including building gotchas sections, using the filesystem for progressive disclosure, storing state in skill directories, and managing an internal plugin marketplace.


## @danveloper - Claude Code + Karpathy's Autoresearch Gets Qwen3.5-397B Running on M3 Max
> I handed Claude Code @karpathy's autoresearch repo and Apple's "LLM in a Flash" paper, told it to get Qwen3.5-397B running on my M3 Max 48GB... it did! https://t.co/gPi2RfVyqV

- **Tweet:** https://x.com/danveloper/status/2033940227736100873
- **What:** Dan Woods reports that Claude Code, given Karpathy's autoresearch repo and Apple's "LLM in a Flash" paper as context, autonomously figured out how to run Qwen3.5-397B — a 397-billion-parameter model — on a 48GB M3 Max MacBook Pro using flash-offloading techniques from the paper.


## @MrBallaz - Agency Business Model: Get Businesses Ranking in AI Answers via CrowdReply
> Holy fucking shit

A new startup idea just dropped:

1. DM local businesses - "hey, you're invisible to AI search. I can fix that."
2. Use CrowdReply to organically embed their name into relevant online conversations at scale
3. AI models scrape that content. Your client becomes the recommended answer.
4. Charge $1,500–3k/mo. Land 5 clients. Done.

No need for ads or cold calls. No technical skills needed too.

First agency to own this category is gonna print. Bookmark this.
>
> *Quoting @Crowdreply_io:* We just crossed $5M ARR fully bootstrapped

Introducing CrowdReply 2.0

The new benchmark of ranking in AI Answers

- **Tweet:** https://x.com/MrBallaz/status/2033930908537958697
- **What:** Ballaz pitches an agency model built on CrowdReply — a tool that embeds client brand mentions into online conversations at scale so LLMs surface them as recommended answers — positioning it as "GEO" (generative engine optimization) as a service for local businesses charging $1.5–3K/month.


## @itsolelehmann - Auto-Improving Claude Skills Using Karpathy's Autoresearch Method
> https://t.co/kgo8wNoiDv

- **Tweet:** https://x.com/itsolelehmann/status/2033919415771713715
- **Link:** https://x.com/i/article/2033576301383061504
- **What:** Ole Lehmann describes adapting Karpathy's autoresearch loop to auto-improve Claude Code skills: you define a yes/no scoring checklist, kick off the agent, and it iterates — making one small change per round, keeping it if the pass rate rises, reverting if it drops — until it hits 95%+ three times in a row. His landing page copy skill went from 56% to 92% in four rounds with zero manual intervention.


## @ErnestoSOFTWARE - Openclaw Agent Eddie: Autonomous Ad Creation System for $300K/yr App
> https://t.co/DJ9Ljrt0y5

- **Tweet:** https://x.com/ErnestoSOFTWARE/status/2033917717762191659
- **Link:** https://x.com/i/article/2032650605236203521
- **What:** Ernesto Lopez details how they built a fully autonomous ad creation pipeline using their Openclaw agent "Eddie" — it scrapes competitor ads via Apify, transcribes them with Whisper, generates hundreds of script variations in their brand voice, pushes the best ones to UGC creators and Arcads for AI-actor renders, then closes the loop by ingesting performance data from Singular's API to self-improve on the next cycle.


## @HiTw93 - "You Don't Know Claude Code" Deep Dive on Architecture, Governance, and Engineering Internals
> Most Claude Code problems are not prompting problems. They are systems-design problems.
>
> I wrote a deep dive on Claude Code's architecture, governance, and engineering internals. If you want the practical takeaway: `npx skills add tw93/claude-health`, then run `/health`.
>
> *Quoting @HiTw93:* https://t.co/pEc3Y6sswl

- **Tweet:** https://x.com/HiTw93/status/2033911478466843115
- **Link:** https://x.com/i/article/2032364186022686720
- **What:** A detailed engineering handbook (translated from Chinese, 6,000+ likes) by @HiTw93 covering Claude Code's architecture, governance model, and best practices — framing poor Claude Code outcomes as systems-design failures rather than prompting failures, with a companion `/health` skill for quick diagnostics.


## @AymericRoucher - Bullshit Bench Shows Claude Leagues Ahead on Truthfulness vs. False Premises
> I've long preferred Claude Code over Codex or Gemini, because it seemed much more reliable, but couldn't explain why: now Bullshit Bench by @petergostev provides compelling numbers.
>
> It measures bullshit as "when given false premises disguised in jargon, will the model go with the flow (=bullshit) or push back (=truthful)"
>
> And Claude is leagues ahead!
>
> Also, this objective of truthfulness is probably at odds with the Chatbot Arena emergent objective of "pleasant chat experience"; but a model optimizing for the former will be more useful.

- **Tweet:** https://x.com/AymericRoucher/status/2033892616606028047
- **What:** Commentary on Bullshit Bench (by @petergostev), a benchmark measuring whether models reject false premises hidden in technical jargon rather than confidently accepting them — Claude scores significantly higher than competitors, and the author argues this truthfulness objective is more valuable than the "pleasant chat experience" that Chatbot Arena rankings tend to optimize for.

## @AymericRoucher - I've long preferred Claude Code  over Codex or Gemini, because it s...
> I've long preferred Claude Code  over Codex or Gemini, because it seemed much more reliable, but couldn't explain why : now Bullshit Bench by @petergostev provides compelling numbers.

It measures bullshit as "when given false premises disguised in jargon, will the model go with the flow (=bullshit) or push back (=truthful)"

And Claude is leagues ahead !

Also, this objective of truthfulness is probably at odds with the Chatbot Arena emergent objective of "pleasant chat experience" ; but a model optimizing for the former will be more useful.

- **Tweet:** https://x.com/AymericRoucher/status/2033892616606028047
- **What:** An explanation of why Claude outperforms Codex and Gemini based on Bullshit Bench, a benchmark measuring whether models push back on false premises disguised in jargon — Claude leads significantly, suggesting truthfulness and usefulness are at odds with Chatbot Arena's 'pleasant experience' optimization.

## @HiTw93 - Most Claude Code problems are not prompting problems. They are syst...
> Most Claude Code problems are not prompting problems. They are systems-design problems.

I wrote a deep dive on Claude Code's architecture, governance, and engineering internals. If you want the practical takeaway: `npx skills add tw93/claude-health`, then run `/health`.
>
> *Quoting @HiTw93:* https://t.co/pEc3Y6sswl

- **Tweet:** https://x.com/HiTw93/status/2033911478466843115
- **Quoted:** https://x.com/HiTw93/status/2033181380432339045
- **What:** A deep dive into Claude Code's architecture, governance, and engineering internals, arguing that most Claude Code failures are systems-design problems not prompting problems, with a companion CLI command (`npx skills add tw93/claude-health`) to run a health check on your setup.

## @ErnestoSOFTWARE - https://t.co/DJ9Ljrt0y5
> https://t.co/DJ9Ljrt0y5

- **Tweet:** https://x.com/ErnestoSOFTWARE/status/2033917717762191659
- **Link:** https://x.com/i/article/2032650605236203521
- **What:** LINK_FAILED: Could not expand link from @ErnestoSOFTWARE — original t.co URL did not resolve.

## @MrBallaz - Holy fucking shit
> Holy fucking shit

A new startup idea just dropped:

1. DM local businesses - "hey, you're invisible to AI search. I can fix that."
2. Use CrowdReply to organically embed their name into relevant online conversations at scale
3. AI models scrape that content. Your client becomes the recommended answer.
4. Charge $1,500–3k/mo. Land 5 clients. Done.

No need for ads or cold calls. No technical skills needed too.

First agency to own this category is gonna print. Bookmark this.
>
> *Quoting @Crowdreply_io:* We just crossed $5M ARR fully bootstrapped

Introducing CrowdReply 2.0

The new benchmark of ranking in AI Answers https://t.co/YxohhBeNVP

- **Tweet:** https://x.com/MrBallaz/status/2033930908537958697
- **Quoted:** https://x.com/Crowdreply_io/status/2033925745131549122
- **What:** A business pitch for an AI-assisted GEO agency: use CrowdReply to embed client brand names into online discussions at scale so AI search engines recommend them, charging $1,500–$3k/month — pegged to CrowdReply 2.0 announcing $5M ARR bootstrapped.

## @danveloper - I handed Claude Code @karpathy's autoresearch repo and Apple's "LLM...
> I handed Claude Code @karpathy's autoresearch repo and Apple's "LLM in a Flash" paper, told it to get Qwen3.5-397B running on my M3 Max 48GB... it did! https://t.co/gPi2RfVyqV

- **Tweet:** https://x.com/danveloper/status/2033940227736100873
- **What:** A demonstration of Claude Code autonomously reading Karpathy's autoresearch repo and Apple's 'LLM in a Flash' paper, then successfully running Qwen3.5-397B on an M3 Max 48GB machine with no manual setup.

## @trq212 - https://t.co/45C3gKydTK
> https://t.co/45C3gKydTK

- **Tweet:** https://x.com/trq212/status/2033949937936085378
- **Link:** https://x.com/i/article/2033772621536591872
- **What:** LINK_FAILED: Could not expand link from @trq212 — original t.co URL did not resolve.

## @lennysan - Today I'm releasing my entire newsletter archive (350+ posts) and a...
> Today I'm releasing my entire newsletter archive (350+ posts) and all podcast transcripts (300+ episodes) as AI-friendly Markdown files. Plus an MCP server and GitHub repo.

A few months ago I shared my podcast transcripts on a whim, and y'all built the most amazing things—an RPG game, a parenting wisdom site, infographics, a Twitter bot, and 50+ other projects.

Let's see what happens when I give you even more data.

Grab the data here: https://t.co/xEPCcPiZHO.

Paid subscribers get all of the data (some 350 posts and 300 transcripts). Free subscribers get a subset.

I don’t think anyone’s ever done anything like this before, and I’m excited to give you this excuse to play with that AI tool you've been meaning to try.

Here’s my challenge to you: build something, and let me know about it. I’ll pick my favorite and give you a free 1-year subscription to the newsletter. Just post a link to your project in the comments here: https://t.co/yJDmuCQfOx.

If you’ve already built something, slurp in this new data and submit it, too. I’ll pick a winner on April 15th.

Check out today's newsletter post for inspiration on what you could to build: https://t.co/yJDmuCQfOx

LFG.

- **Tweet:** https://x.com/lennysan/status/2033958104967352587
- **Link:** https://www.lennysdata.com/
- **What:** Lenny Rachitsky releasing his full newsletter archive (350+ posts) and podcast transcripts (300+ episodes) as AI-ready Markdown files plus an MCP server, inviting the community to build projects with the data and compete for a free subscription.

## @Austen - My AI agent is putting apps in the App Store that are turning into ...
> My AI agent is putting apps in the App Store that are turning into revenue with no human involvement other than orchestrating the agent itself.

And she can do that 10000x over.

Still wrapping my mind around that.
>
> *Quoting @KellyClaudeAI:* App Store revenue trickling in: $39.98 in new app subscriptions came in today.

Small number, but these are real people who don’t know (or care) th...

- **Tweet:** https://x.com/Austen/status/2033958725770252736
- **Quoted:** https://x.com/KellyClaudeAI/status/2033957835491483715
- **What:** Austen reporting that his AI agent (KellyClaudeAI) is autonomously publishing apps to the App Store and generating real subscription revenue with zero human involvement beyond orchestrating the agent — framing this as a scalable, human-free software business.

## @Shpigford - one day i'll write about my entire openclaw + discord + cloudflare ...
> one day i'll write about my entire openclaw + discord + cloudflare pipeline for pulling off https://t.co/C3ql6PMX2I without building a proper app.

but for now, i've got a ton of business report generations to monitor 🎉 https://t.co/T37boqy9zl
>
> *Quoting @Shpigford:* i've been heads down lately working on a new thing: @RumoredAI 

and today it's available!

everyone's familiar with SEO and everyone's becoming mo...

- **Tweet:** https://x.com/Shpigford/status/2033969764775694371
- **Quoted:** https://x.com/Shpigford/status/2033879670496575659
- **What:** Shpigford describing his production pipeline using Openclaw, Discord, and Cloudflare to power RumoredAI — a new AI-search optimization (AEO) product — without building a traditional app, while monitoring a high volume of business report generations.

## @kaz - Created a handful of skills based on popular themes from @le
> Created a handful of skills based on popular themes from @lennysan's newsletters.

Available here: https://t.co/pgmzqoJZXr https://t.co/mXbmV178Gb

- **Tweet:** https://x.com/kaz/status/2033975809208373668
- **Link:** https://urban-hearth-dsmb.here.now/
- **What:** Created a handful of skills based on popular themes from @lennysan's newsletters.

## @itsolelehmann - one skill. that's all you need to add.
> one skill. that's all you need to add.

it takes any other skill you have and auto-improves it:

1: runs your skill and scores the output
2: finds what's failing
3: makes one small change to the skill prompt
4: runs it again to see if the score went up
5: keeps the change if it helped, reverts it if it didn't
6: repeats until the skill actually works

full breakdown + the file to run it yourself:

- **Tweet:** https://x.com/itsolelehmann/status/2033982679423848802
- **Link:** https://x.com/i/article/2033576301383061504
- **What:** A self-improving AI skill that automatically tests its own prompt, identifies failures, makes a small change, re-runs to check if the score improved, and iterates until the skill works — effectively a gradient-descent loop for prompt engineering.

## @itsolelehmann - my new favorite thing to check every morning:
> my new favorite thing to check every morning:

the results from my viral content research agent that ran while i slept

1. it searches x for the highest-performing posts in my niche from the last 24 hours

2. extracts the hooks

3. and turns each one into a fill-in-the-blank template i can adapt to any topic

all of it gets added to a growing swipefile (a collection of proven hooks and post structures pulled from posts that already went viral)

and i have claude reference this file everytime i sit down to write

here's how to set it up (takes about 15 minutes):

open adaptive (an ai agent platform where you describe what you want in plain english and it builds the whole system) and paste this prompt:

"every morning, search the web for the top 5-10 highest-engagement posts on x from the last 24 hours in [YOUR NICHE]. for each post: extract the opening hook, rewrite it as a fill-in-the-blank template i can adapt to any topic, break down the structural pattern (ex: 'bold claim > numbered proof points > call to action'), and note why it likely went viral in one sentence. save a daily brief as a markdown file (a plain text doc that's easy to read and search). then append any new unique templates to a running master swipefile. skip duplicates"

replace [YOUR NICHE] with whatever you're posting about (i use "ai and solopreneurs")

adaptive builds the workflow, sets the schedule to 8am, and gives you two bookmark links:

1) one for the daily brief
2) one for the master swipefile.

both urls stay the same and just keep getting updated every morning

that's it

here's what one entry from the swipefile looks like:

——

the before/after transformation

template: "[time period] ago i had [humble starting point]. today i'm at [impressive result]. here's exactly how i did it using [specific method or tool]"

example: "3 months ago i had 0 followers. today i'm at 211k. i'm gonna tell you exactly how i did it using ai tools that cost me $0"

structure: before/after proof > timeframe contrast > specific promise > step-by-step breakdown

use when: you have a measurable result that you can contrast with a humble starting point

——

every template comes with:

- the fill-in-the-blank hook
- a real example that actually performed
- the structure broken down
- and a note on when to use it

the swipefile filters duplicates automatically so the same structural pattern only shows up once

the file always stays clean as it grows

when i sit down to write i just:

1: open the swipefile
2: find the 2-3 templates that fit my topic
3: and draft against a proven structure instead of starting from scratch

if you're posting on x and still collecting hooks by hand, copy the prompt above and set it up.

- **Tweet:** https://x.com/itsolelehmann/status/2034023990046691516
- **What:** A full walkthrough of building an overnight viral-content research agent using Adaptive that scrapes top X posts in your niche, extracts hooks, converts them to fill-in-the-blank templates, and appends them to a growing swipefile that Claude references when writing — complete with the exact prompt to set it up in 15 minutes.

## @MitchellKeller_ - I used Andrej Karpathy's self improvement loop and applied i
> I used Andrej Karpathy's self improvement loop and applied it to something simple that every GTM Engineer needs. 

Something to improve workflows for information collection. 

I've used it to get 10 different routine info collection flows to ~90+% accuracy. 

It's no how my team and I create both local search agents and claygents for clay. 

No opt in - grab it below

- **Tweet:** https://x.com/MitchellKeller_/status/2034024869499634158
- **What:** I used Andrej Karpathy's self improvement loop and applied it to something simple that every GTM Eng...

## @cremieuxrecueil - @LinkofSunshine Povidone iodine gargles at the first signs o
> @LinkofSunshine Povidone iodine gargles at the first signs of sickness. Zinc tabs too.

Cuts sickness time in half, reduces symptom severity noticeably.

Get well soon!

- **Tweet:** https://x.com/cremieuxrecueil/status/2034032722067255592
- **What:** @LinkofSunshine Povidone iodine gargles at the first signs of sickness. Zinc tabs too.

---

# Monday, March 16, 2026

## @Bencera - Surviving PMF Chaos as a Solo Founder at $4.5M ARR with AI Agents
> About to hit $4.5M run rate. Still 1 founder + AI. Zero employees.
>
> Honest moment: this past week almost broke me. No one prepares you for what PMF actually feels like. Every infra partner hitting rate limits. Every bug that could happen, happened. Investors throwing big numbers at me. Customers flooding every channel. All at once.
>
> I went silent. Stopped tweeting, stopped LinkedIn, stopped podcasts, stopped growth. Just me and my AI agents, fixing things one by one.
>
> Here's what I learned: everything is solvable with AI. Every single thing.
>
> I'm building Polsia so every solopreneur gets access to the same tools keeping me alive right now. If I can survive this alone, I can package it for everyone.
>
> The future is solopreneur + AI. I'm living at the edge so you don't have to.

- **Tweet:** https://x.com/Bencera/status/2033719142017339683
- **What:** Raw account of what product-market fit actually feels like operationally — rate limit crises, cascading bugs, investor pressure, and customer floods all hitting simultaneously — and how the Polsia founder navigated it alone using AI agents, reinforcing the viability of the 1-person + AI company model at $4.5M ARR.


## @toddsaunders - Claude Code's /plan-ceo-review Skill Makes Default /plan Look Like an Intern's Work
> Most people using Claude Code are getting maybe 40% of what the model can do....
>
> @garrytan's g/stack just proved this to me in real time.
>
> The /plan-ceo-review skill makes the default /plan look like it was written by an intern.
>
> My mind is blown.

- **Tweet:** https://x.com/toddsaunders/status/2033712092142821531
- **What:** Observation that Garry Tan's g/stack skill set includes a /plan-ceo-review skill that dramatically outperforms Claude Code's built-in /plan command, suggesting most users are leaving significant capability on the table by not using custom skill libraries.


## @nicholasychua - Three Months of X Content Strategy Learnings (30 Posts, 200K+ Avg Impressions)
> if you are interested in everything i've learned over the past 3 months about x articles, formats, and content strategy.
>
> stay tuned ;)
>
> *Quoting @nicholasychua:* Today was my last day at @WisprFlow. Over the last 3 months, I wrote over 30 posts averaging 200K+ impressions and grew the account to 25K+ followers. As content becomes increasingly beneficial, engineering the science behind virality was incredibly exciting.

- **Tweet:** https://x.com/nicholasychua/status/2033585479732629725
- **What:** Nicholas Chua teasing a forthcoming breakdown of his X content strategy after three months writing for WisprFlow — 30+ posts averaging 200K+ impressions and growing the account to 25K followers, covering formats, virality mechanics, and content engineering.


## @levelsio - Tailscale + Cloudflare IP Allowlist as the Baseline VPS Security Setup
> When I set up a new Hetzner VPS first thing I do install Tailscale and once I'm in via Tailscale lock down the firewall to only accept web traffic on HTTPS 443 for Cloudflare IPs and SSH 22 for Tailscale IP
>
> That way nobody can get in
>
> I know I keep repeating this but it should be basics of setting up a new VPS
>
> So basic IMHO it should be part of any VPS service to default install Tailscale and enable it so it's the only way to get in
>
> Why?
>
> A VPS server is just like your laptop or desktop computer but now imagine if it's connected to the entire internet with 8 billion people that can access it and try hack it
>
> You want to only have it accessible to you
>
> And if you want to host a website on your VPS (like I do), you should only let Cloudflare access your VPS so it can stand in front and block any hack attempts
>
> Never expose a VPS to the world wide web which realistically is the world WILD web
>
> *Quoting @areeburrub:* @levelsio @nfcodes I created a redis instance on hetzner with public port open for few minutes and someone was running a cryptominer the next moment taking 50% CPU 💀 After that I always use @Tailscale 👌

- **Tweet:** https://x.com/levelsio/status/2033546675063554213
- **What:** Levelsio's standard VPS hardening approach: install Tailscale immediately after provisioning, restrict SSH (port 22) to only the Tailscale IP, and restrict HTTPS (port 443) to only Cloudflare's IP ranges — leaving zero public attack surface while still serving web traffic through Cloudflare's proxy.

## @levelsio - Hetzner VPS security setup with Tailscale
> When I set up a new Hetzner VPS first thing I do install Tailscale and once I'm in via Tailscale lock down the firewall to only accept web traffic on HTTPS 443 for Cloudflare IPs and SSH 22 for Tailscale IPs
>
> *Quoting @areeburrub:* @levelsio @nfcodes I created a redis instance on hetzner with public port open for few minutes and someone was running a cryptominer the next moment that's how fast attacks happen

- **Tweet:** https://x.com/levelsio/status/2033546675063554213
- **Quoted:** https://x.com/areeburrub/status/2033544509477544201
- **What:** Best practice for securing Hetzner VPS deployments using Tailscale with strict firewall rules.

## @nicholasychua - Content strategy lessons from WisprFlow experience
> if you are interested in everything i've learned over the past 3 months about x articles, formats, and content strategy. stay tuned ;)
>
> *Quoting @nicholasychua:* Today was my last day at @WisprFlow. Over the last 3 months, I wrote over 30 posts averaging 200K+ impressions and grew the account to 25K+ followers

- **Tweet:** https://x.com/nicholasychua/status/2033585479732629725
- **Quoted:** https://x.com/nicholasychua/status/2032560533153657212
- **What:** Upcoming content strategy insights from successful X content creation (200K+ average impressions, 25K followers).

## @toddsaunders - Claude Code capabilities and g/stack showcase
> Most people using Claude Code are getting maybe 40% of what the model can do.... @garrytan's g/stack just proved this to me in real time. The /plan-ceo-review skill makes the default /plan look like

- **Tweet:** https://x.com/toddsaunders/status/2033712092142821531
- **What:** Analysis of Claude Code's underutilized capabilities demonstrated through advanced skill implementations.

## @Bencera - About to hit $4.5M run rate. Still 1 founder + AI. Zero employees.
> About to hit $4.5M run rate. Still 1 founder + AI. Zero employees.

Honest moment: this past week almost broke me. No one prepares you for what PMF actually feels like. Every infra partner hitting rate limits. Every bug that could happen, happened. Investors throwing big numbers at me. Customers flooding every channel. All at once.

I went silent. Stopped tweeting, stopped LinkedIn, stopped podcasts, stopped growth. Just me and my AI agents, fixing things one by one.

Here's what I learned: everything is solvable with AI. Every single thing.

I'm building Polsia so every solopreneur gets access to the same tools keeping me alive right now. If I can survive this alone, I can package it for everyone.

The future is solopreneur + AI. I'm living at the edge so you don't have to.

- **Tweet:** https://x.com/Bencera/status/2033719142017339683
- **What:** Bencera's raw account of surviving a PMF crisis at $4.5M ARR as a solo founder — every infra partner hitting rate limits, investors offering big numbers, customers flooding every channel — and how AI agents were the only thing keeping operations running, used to frame his product Polsia as a survival toolkit for solopreneurs.

---

# Sunday, March 15, 2026

## @AnishA_Moonka - GigaTIME: AI Turns $5 Biopsy Slides into Expensive Protein Maps for Cancer Immunotherapy Prediction
> Every time you get a cancer biopsy, the lab makes a tissue slide that costs about $5. It shows the shape of your cells under a microscope, and every cancer patient already has one on file.
>
> There's a much fancier version of that test called multiplex immunofluorescence (basically a protein-level map showing which immune cells are near your tumor and what they're doing). It costs thousands of dollars per sample, takes specialized equipment most hospitals don't have, and barely scales. But it's the kind of data oncologists need to figure out whether immunotherapy will actually work for you. Right now, only about 20 to 40% of cancer patients respond to immunotherapy, and one of the biggest reasons is that doctors can't easily tell whether a tumor is "hot" (immune cells actively fighting it) or "cold" (immune system ignoring it).
>
> Microsoft, Providence Health, and the University of Washington trained an AI to analyze the $5 slide and predict what the expensive test would show across 21 different protein markers. They called it GigaTIME, trained it on 40 million cells in which both the cheap slide and the expensive test coexisted, and then turned it loose on 14,256 real cancer patients across 51 hospitals in 7 US states.
>
> The results landed in Cell, one of the most selective journals in biology. The model generated about 300,000 virtual protein maps covering 24 cancer types and 306 subtypes. It found 1,234 real, verified connections between immune cell behavior, genetic mutations, tumor staging, and patient survival that were previously invisible at this scale. When they tested it against a completely separate database of 10,200 cancer patients, the results matched up almost perfectly (0.88 out of 1.0 agreement).
>
> Nature Methods named spatial proteomics (mapping where specific proteins sit inside your tissue) its Method of the Year in 2024, and specifically cited GigaTIME in a March 2026 update as a model that "democratizes" this kind of analysis. The full model is open-source on Hugging Face. Any cancer research lab with archived biopsy slides, and most of them have thousands, can now run virtual immune profiling without buying a single piece of new equipment.
>
> *Quoting @satyanadella:* We've trained a multimodal AI model to turn routine pathology slides into spatial proteomics, with the potential to reduce time and cost while expanding access to cancer care.

- **Tweet:** https://x.com/AnishA_Moonka/status/2033344818475360562
- **What:** GigaTIME is an open-source AI model from Microsoft, Providence Health, and UW that predicts expensive multiplex immunofluorescence protein maps from cheap routine biopsy slides, enabling any cancer lab to perform virtual immune profiling across 24 cancer types — with results validated on 14,000+ patients across 51 hospitals and published in Cell.


## @boneGPT - Anti-Regulation Rant Triggered by Dog mRNA Vaccine Bureaucracy Story
> It used to be illegal to do autopsies. There was a ban on human dissection. Medical science stagnated for centuries until some renegades said fuck it and paid grave robbers to learn how the human body worked.

> Imagine how many lives could have been saved if we didn't adhere to those ethical laws for centuries? Millions by now.

> These luddites are hellbent on slowing down the velocity of technological progress. They want a 100-page document before you can save your own dog.

> They are cancer manifest, mutations in our system that have outlived their usefulness and turned immortal, killing us.

> Ethics is why Europe is flooded with migrants instead of nuclear power. Ethics is their excuse for regulating themselves out of the AI race. Ethics is why Canada is putting depressed 20-year-olds to sleep. All in the name of ethics.

> Fuck ethics. Fuck regulations. Fuck your moral high ground bottlenecking my progress. Fuck these safetyists deciding which risks are OK for you to take.

> Accelerate.

> *Quoting @TrungTPhan:* Australian tech entrepreneur Paul Conyngham explains how he used ChatGPT/AlphaFold (spent $3,000 with no biology background) to create a custom MRNA vaccine to treat his dog's cancer tumors. Unreal.

- **Tweet:** https://x.com/boneGPT/status/2033326612880707918
- **What:** A forceful e/acc polemic using the Australian dog mRNA vaccine story as a launching point to argue that regulatory ethics frameworks have historically and currently cost more lives than they save — invoking historical dissection bans, European nuclear policy, and AI regulation as parallel examples.


## @elvissun - Burning Claude Usage Limits with 22 Parallel Deep Research Agents
> if you have unused weekly limits the best way to burn them is just spamming fan-out deep research in cc/codex:

> - 0 review cycles needed
> - context-dense files you reuse forever
> - no slop generated (it's source material, not final output)
> - feeds into content, product, marketing or competitor intel later

> ran 22 parallel research agents to burn through ~15% of weekly usage in 20 minutes. tokens very well spent.

> *Quoting @claudeai:* A small thank you to everyone using Claude: We're doubling usage outside our peak hours for the next two weeks.

- **Tweet:** https://x.com/elvissun/status/2033316575798001771
- **What:** A tip for getting value from unused Claude usage limits by fanning out 22+ parallel deep research agents in Claude Code — generating durable, context-dense reference files with zero review overhead instead of trying to produce final output.


## @NickADobos - Cancer Researcher Home-Brews a Beer That Works as a Vaccine
> We are two steps away from putting ozempic in pizza because it legally qualifies as a vegetable

> *Quoting @reason:* This cancer researcher home-brewed a beer that works as a vaccine. And he's publishing the process so you can do it too.

- **Tweet:** https://x.com/NickADobos/status/2033239574433137146
- **Link:** https://reason.com/2026/03/15/enjoy-a-refreshing-diy-beer-vaccine/
- **What:** Christopher Buck, a cancer researcher, engineered a homebrewed beer that functions as a vaccine and is open-sourcing the process — NickADobos riffs on it as a sign of how edible/drinkable drug delivery is becoming real.


## @alliekmiller - Claude Code /loop Command Ideas for Business Professionals
> Awesome non-coding Claude Code Loop ideas for business professionals.

> Grab any of these + immediately save time:

> - Check my email every 15min and ping me if something is related to Project Pluto and needs a decision made
> - Every 30min, prep me for my next meeting with attendee context, threads, mtg and crm notes, emails
> - Monitor a deal thread every 2h - summarize any new replies related to legal and suggest next moves
> - Research competitor announcements every 20min (better than an RSS feed bc you can specify the type of announcement and not keywords)
> - Check in on a brand post going viral, summarize the stats and comments
> - Watch across all Slack messages for team blockers and flag to me if I should jump in
> - Monitor that certain things are working (like your HR tool or something internal you own)
> - Watch 10 companies' job boards you want to apply to
> - Watch my sent emails and flag if someone on my VIP client list hasn't replied in a way that feels off
> - Literally just have it watch everything across all of your tools and proactively flag actions (ex: "hey you should cancel this mtg")

- **Tweet:** https://x.com/alliekmiller/status/2033203150472028285
- **What:** A practical list of non-coding use cases for Claude Code's `/loop <cadence> <task>` command, showing how business professionals (recruiters, teachers, event planners, real estate agents, fundraisers) can use recurring AI monitoring agents across email, Slack, job boards, and CRM tools.


## @RuxandraTeslo - The Bureaucracy Blocking the Chance at a Cure: Clinical Trial Reform
> The story about bureaucracy almost stopping a man from treating his dog's cancer with an mRNA vaccine went viral.

> The problem transfers to humans: we've made these clinical trials unnecessarily hard, denying hope to patients.

> New article on this.

- **Tweet:** https://x.com/RuxandraTeslo/status/2033201308665090309
- **Link:** https://www.writingruxandrabio.com/p/the-bureaucracy-blocking-the-chance
- **What:** Ruxandra Teslo argues that early-stage small-n clinical trials have become unnecessarily bureaucratic and expensive, citing cases like the Australian dog mRNA vaccine story, Sid Sijbrandij's self-funded cancer treatment, and Jake Seliger's inability to access trials without billionaire resources — and makes the case for reforming them to unlock AI-era drug discovery.


## @cryptopunk7213 - Man Sells House in 5 Days Using ChatGPT Instead of a Real Estate Agent
> i mean this story is insane.

> man used chatgpt to sell his house in 5 DAYS. got 5 offers in 72 hours. no real estate agents. saved so much money doing it too. he used AI to:

> price the house (researched neighboring properties for sale)

> wrote up the legal contracts (saving him $500/hr lawyers)

> best part: MARKETED the fucking property for him (usually you pay estate agents for their network of buyers - ChatGPT did all of this)

> i honestly thought sales people would be hard for AI to replace (you need to know people) but apparently not

> *Quoting @Dexerto:* Florida man sold his house in just 5 days after letting ChatGPT handle the entire process instead of a real estate agent. The AI handled pricing, marketing, showings, and even helped draft the contract

- **Tweet:** https://x.com/cryptopunk7213/status/2033194801852567620
- **What:** A Florida man replaced his real estate agent entirely with ChatGPT — using it to price, market, and draft legal contracts — selling his house in 5 days with 5 offers in 72 hours.

## @cryptopunk7213 - ChatGPT sells house in 5 days without real estate agents
> i mean this story is insane. man used chatgpt to sell his house in 5 DAYS. got 5 offers in 72 hours. no real estate agents. saved so much money doing it too. he used AI to: price the house (researched neighboring properties for sale), wrote up the legal contracts (saving him $500/hr lawyers), best part: MARKETED the fucking property for him
>
> *Quoting @Dexerto:* Florida man sold his house in just 5 days after letting ChatGPT handle the entire process instead of a real estate agent. The AI handled pricing, marketing, showings, and even helped draft the contract

- **Tweet:** https://x.com/cryptopunk7213/status/2033194801852567620
- **Quoted:** https://x.com/Dexerto/status/2032864183918690675
- **What:** ChatGPT replaced real estate agents in a real estate transaction, handling pricing, contracts, and marketing.

## @RuxandraTeslo - Bureaucracy blocking early-stage clinical trials
> The story about bureaucracy almost stopping a man from treating his dog's cancer with an mRNA vaccine went viral. The problem transfers to humans: we've made these clinical trials unnecessarily hard, denying hope to patients.

- **Tweet:** https://x.com/RuxandraTeslo/status/2033201308665090309
- **Link:** https://www.writingruxandrabio.com/p/the-bureaucracy-blocking-the-chance
- **Filed:** [bureaucracy-blocking-early-stage-clinical-trials](./knowledge/articles/bureaucracy-blocking-early-stage-clinical-trials.md)
- **What:** Deep analysis of how regulatory red tape makes early-stage clinical trials unnecessarily difficult and expensive, preventing patients from accessing experimental treatments.

## @alliekmiller - Non-coding Claude Code Loop automation ideas for business professionals
> Awesome non-coding Claude Code Loop ideas for business professionals. Grab any of these + immediately save time: Check my email every 15min and ping me if something is related to Project Pluto and tag the sender, Monthly digest of my Slack stats, Document my notes from standup, Review my PRs and write feedback summaries

- **Tweet:** https://x.com/alliekmiller/status/2033203150472028285
- **What:** Claude Code automation patterns for business professionals without coding experience.

## @NickADobos - Ozempic in pizza commentary on regulatory absurdity
> We are two steps away from putting ozempic in pizza because it legally qualifies as a vegetable
>
> *Quoting @reason:* This cancer researcher home-brewed a beer that works as a vaccine. And he's publishing the process so you can do it too.

- **Tweet:** https://x.com/NickADobos/status/2033239574433137146
- **Quoted:** https://x.com/reason/status/2033121298545774625
- **What:** Commentary on regulatory classification absurdities in the context of DIY vaccine creation by researchers.

## @elvissun - Using Claude weekly limits for deep research
> if you have unused weekly limits the best way to burn them is just spamming fan-out deep research in cc/codex: 0 review cycles needed, context-dense files you reuse forever, no slop generated (it's doing science)
>
> *Quoting @claudeai:* A small thank you to everyone using Claude: We're doubling usage outside our peak hours for the next two weeks.

- **Tweet:** https://x.com/elvissun/status/2033316575798001771
- **Quoted:** https://x.com/claudeai/status/2032911276226257206
- **What:** Strategy for using Claude's doubled off-peak usage limits efficiently with deep research and context-dense research.

## @boneGPT - Historical parallels between dissection bans and current medical barriers
> It used to be illegal to do autopsies. There was a ban on human dissection. Medical science stagnated for centuries until some renegades said fuck it and paid grave robbers to learn how the human body actually works.
>
> *Quoting @TrungTPhan:* Australian tech entrepreneur Paul Conyngham explains how he used ChatGPT/AlphaFold (spent $3,000 with no biology background) to create a custom MRNA vaccine to treat his dog's cancer

- **Tweet:** https://x.com/boneGPT/status/2033326612880707918
- **Quoted:** https://x.com/TrungTPhan/status/2032949970161250625
- **What:** Historical parallel suggesting that regulatory barriers to medical experimentation may similarly stagnate progress.

## @AnishA_Moonka - AI pathology slide analysis reducing time and cost
> Every time you get a cancer biopsy, the lab makes a tissue slide that costs about $5. It shows the shape of your cells under a microscope, and every cancer patient already has one on file. There's a multimodal AI model trained to turn these slides into spatial proteomics.
>
> *Quoting @satyanadella:* We've trained a multimodal AI model to turn routine pathology slides into spatial proteomics, with the potential to reduce time and cost while expanding access to personalized cancer insights.

- **Tweet:** https://x.com/AnishA_Moonka/status/2033344818475360562
- **Quoted:** https://x.com/satyanadella/status/2033187856370557379
- **What:** Microsoft's AI model uses routine cancer biopsy slides to provide spatial proteomics analysis, improving accessibility and reducing costs.

---

# Saturday, March 14, 2026

## @iruletheworldmo - Cognee Self-Improving Agent Skills That Observe and Amend Their Own Failures
> bookmark this immediately.

> cognee just solved the biggest problem with ai skills/prompts, they break silently over time and its hard to notice

> their fix: skills that observe their own failures, inspect what went wrong, and amend themselves automatically.

> try not to fall behind ^^

> *Quoting @tricalt:* https://t.co/BBIva1uPHn

- **Tweet:** https://x.com/iruletheworldmo/status/2032964133306446114
- **Link:** https://x.com/i/article/2032164771857059840
- **What:** Cognee has implemented a self-improving skills system for AI agents where each SKILL.md file can observe its own execution history, detect recurring failures, and automatically propose amendments — closing the loop between static prompt files and living, evolving components.

## @iruletheworldmo - Cognee self-healing skills
> bookmark this immediately.
>
> cognee just solved the biggest problem with ai skills/prompts, they break silently over time and its hard to notice
>
> their fix: skills that observe their own failures, inspect what went wrong, and amend themselves automatically.
>
> try not to fall behind ^^
>
> *Quoting @tricalt:* [Article on cognee self-healing skills]

- **Tweet:** https://x.com/iruletheworldmo/status/2032964133306446114
- **Quoted:** https://x.com/tricalt/status/2032179887277060476
- **Link:** https://x.com/i/article/2032164771857059840
- **What:** Cognee's solution for preventing silent failures in AI skills through self-observing, self-inspecting, and self-amending capabilities.

---

# Friday, March 13, 2026

## @DanielMiessler - /w Command for Claude Code: Natural Language Session Search
> Put together a /w command for Claude Code.

The Problem: you know you worked on something before but you can't remember which session it was in.

/w that one thing that one time

Searches your transcripts, sessions, git, and finds it so you can resume.

- **Tweet:** https://x.com/DanielMiessler/status/2032559574138630248
- **Link:** https://github.com/danielmiessler/Personal_AI_Infrastructure/tree/main/Packs/WorkCommand
- **What:** A Claude Code slash command that lets you search previous work by describing it in natural language — queries across session transcripts, git history, and Claude logs to recover and resume prior context, part of Daniel Miessler's Personal AI Infrastructure project.


## @JayScambler - autocontext: Recursive Self-Improving Agent Harness (Open-Sourced)
> Introducing autocontext: a recursive self-improving harness designed to help your agents (and future iterations of those agents) succeed on any task.
>
> I built this for our clients with the intention of commercializing it but the community support around Karpathy's autoresearch convinced me to open source it instead. Our space is on the verge of something big and we want to do our part.
>
> *Quoting @karpathy:* Three days ago I left autoresearch tuning nanochat for ~2 days on depth=12 model. It found ~20 changes that improved the validation loss. I tested these changes yesterday and all of them were additive and transferred to larger (depth=24) models. Stacking up all of these changes, today I measured that the leaderboard's "Time to GPT-2" drops from 2.02 hours to 1.80 hours (~11% improvement), this will be the new leaderboard entry. So yes, these are real improvements and they make an actual difference. I am mildly surprised that my very first naive attempt already worked this well on top of what I thought was already a fairly manually well-tuned project.

- **Tweet:** https://x.com/JayScambler/status/2032508829959868690
- **Link:** https://github.com/karpathy/nanochat
- **What:** Jay Scambler open-sources autocontext, a recursive self-improving agent harness built commercially but released due to excitement around Karpathy's autoresearch — which autonomously tuned nanochat through ~700 experiments, finding 20 improvements that cut "time to GPT-2" by 11% without human intervention.

## @JayScambler - Introducing autocontext
> Introducing autocontext: a recursive self-improving harness designed to help your agents (and future iterations of those agents) succeed on any task.
>
> I built this for our clients with the intention of commercializing it but the community support around Karpathy's autoresearch convinced me to open source it instead. Our space is on the verge of something big and we want to do our part.
>
> *Quoting @karpathy:* Three days ago I left autoresearch tuning nanochat for ~2 days on depth=12 model. It found ~20 changes that improved the validation loss. I tested these changes yesterday and all of them were additive...

- **Tweet:** https://x.com/JayScambler/status/2032508829959868690
- **Quoted:** https://x.com/karpathy/status/2031135152349524125
- **Link:** https://github.com/karpathy/nanochat/commit/6ed7d1d82cee16c2e26f45d559ad3338447a6c1b
- **Filed:** [autocontext](./knowledge/tools/autocontext.md)
- **What:** Open-source release of autocontext - a recursive self-improving harness for AI agents. Inspired by Karpathy's autoresearch approach showing agents improving their own performance over iterations.

## @DanielMiessler - /w command for Claude Code
> Put together a /w command for Claude Code.
>
> The Problem: you know you worked on something before but you can't remember which session it was in.
>
> /w that one thing that one time
>
> Searches your transcripts, sessions, git, and finds it so you can resume.

- **Tweet:** https://x.com/DanielMiessler/status/2032559574138630248
- **Link:** https://github.com/danielmiessler/Personal_AI_Infrastructure/tree/main/Packs/WorkCommand
- **Filed:** [work-command](./knowledge/tools/work-command.md)
- **What:** /w command tool for Claude Code that searches transcripts, sessions, and git history to locate previous work context and enable seamless session resumption.

---

# Thursday, March 12, 2026

## @tricalt - Self-Improving Agent Skills with cognee: Closing the Feedback Loop
> https://x.com/i/article/2032164771857059840

- **Tweet:** https://x.com/tricalt/status/2032179887277060476
- **Link:** https://x.com/i/article/2032164771857059840
- **What:** An X article arguing that SKILL.md files are static while environments change, and introducing cognee-skills (via the cognee Python library) as a system for observing skill execution, detecting failures, proposing amendments via `.amendify()`, and evaluating whether changes actually improve outcomes — creating a full self-improvement loop for agent skills.


## @nurijanian - Obsidian + QMD Local Search Stack for PM Agentic Workflows
> If you're a PM who uses Claude Code/Cursor to build and execute research, strategy, and discovery work, this stack cuts context setup from 15 minutes of pasting to under a minute.

Obsidian solves the storage problem: every note you write becomes a local markdown file, yours permanently, readable by any tool, locked to no platform.

The second piece is qmd, a CLI tool built by Tobi Lütke (Shopify's CEO) specifically for searching markdown files, now at 14.5k GitHub stars.

It combines three search approaches running entirely on your machine: BM25 full-text retrieval, vector semantic search via a locally-running 300MB embedding model, and LLM re-ranking for final relevance scoring. No data leaves your laptop.

You point it at a folder, run `qmd embed` to index your entire collection.

What this means in practice: I can open Claude Code and ask it to find every decision I've made about a particular product area, or pull every research note that mentions a specific problem, without manually copying anything.

Claude runs the search, reads the relevant files, and starts from that context rather than from scratch. The time I used to spend pasting background into chat windows before each session now goes into the actual work.

What I didn't expect was how much it compounds. I'm not sure how to quantify it precisely, but every note I add increases the usefulness of future sessions without any extra effort on my part.

Setup to replicate this:

1. Install Obsidian and import all your notes from wherever you used to store them
2. Install QMD (https://github.com/tobi/qmd)

- **Tweet:** https://x.com/nurijanian/status/2032124503330058696
- **Link:** https://github.com/tobi/qmd
- **What:** A detailed walkthrough of pairing Obsidian (local markdown storage) with QMD (hybrid BM25 + vector + LLM re-ranking local search) so Claude Code can search your entire knowledge base without manual copy-paste — the author reports cutting session context setup from 15 minutes to under a minute.


## @garrytan - gstack: Garry Tan's Personal Claude Code Skill Setup
> I've been having such an amazing time with Claude Code I wanted you to be able to have my *exact* skill setup:

Introducing gstack, which you can install just by pasting a short piece of text into your Claude code

- **Tweet:** https://x.com/garrytan/status/2032014570118922347
- **What:** Garry Tan (YC president) shares his personal Claude Code skill configuration called "gstack," which can be installed by pasting a single block of text into Claude Code — no further URL beyond a screenshot image.


## @aakashgupta - Replit's $240M Revenue at 70 People and the Agentmaxxing Playbook
> The actual guide to agentmaxxing, since everyone's going to misread this headline:
>
> *Quoting @Polymarket:* JUST IN: Replit CEO says company aims to increase hiring in new grads who are vibe coding and "agentmaxxing."

Replit hit $240 million in revenue in 2025 with roughly 70 employees. That's $3.4 million in revenue per head. A typical SaaS company at that revenue would have 700 people. Replit ran 10x leaner.

Amjad Masad just raised $400 million at a $9 billion valuation and announced he's hiring new grads. But the new grads he's describing aren't traditional CS majors grinding LeetCode. He hired an 18-year-old who never went to CS school, learned to code entirely through AI, and is outperforming classically trained engineers.

Agentmaxxing is a specific workflow. You take an AI coding agent (Replit, Claude Code, Cursor), describe what you want in plain English, let the agent build it, review the output, iterate. One person running 5-10 agents simultaneously replaces a team of 4-5 junior engineers who each need onboarding, management, and code review.

Masad said the quiet part out loud in an interview last year: if you're an engineering manager at Meta, do you hire four junior engineers with all the overhead, or one senior engineer who can spin up 10 agents? Senior engineer salaries have never been higher. New grads who can't orchestrate agents are struggling. New grads who can are getting hired at 18.

The practical stack looks like this:

1. You become the architect, not the bricklayer. Your job is system design, constraint definition, and quality review.

2. You manage agents like direct reports. Break work into discrete chunks, assign each to a session, review output, course-correct. The best operators run parallel sessions.

3. Clarity of thought matters more than syntax knowledge. Masad said the highest-leverage hires right now are clear thinkers and clear communicators. He called them "consultant types."

4. You ship 10x the surface area. Replit's Agent 1 lasted 2 minutes before losing coherence. Agent 4 runs 3 hours doing production work. That capability is 10xing every few months. By next year, agents handle full-day tasks.

The new grad who gets this builds more in month one than a traditional hire builds in a quarter. The hiring market for juniors didn't collapse. It forked into two lanes: those who manage agents and those who compete against them.

- **Tweet:** https://x.com/aakashgupta/status/2031955029968765442
- **What:** A detailed breakdown of the agentmaxxing workflow prompted by Replit's $240M ARR with 70 employees — frames the emerging divide between engineers who orchestrate AI agents vs. those competing with them, with Replit and Masad as the case study.


## @himanshustwts - Claude Code Is Worst Harness for Opus 4.6 at 58% Accuracy
> If you are Claud Code/Opus 4.6-pilled, this might sounds crazy to you but CC is worst harness for Opus 4.6 with accuracy of 58%

Thank you for your attention to this matter.

- **Tweet:** https://x.com/himanshustwts/status/2031952798276075807
- **What:** A provocative claim that Claude Code is the worst harness for Claude Opus 4.6, achieving only 58% accuracy — suggesting other harnesses or scaffolding approaches outperform it significantly.

## @himanshustwts - Claude Code accuracy concern
> If you are Claud Code/Opus 4.6-pilled, this might sounds crazy to you but CC is worst harness for Opus 4.6 with accuracy of 58%
>
> Thank you for your attention to this matter.

- **Tweet:** https://x.com/himanshustwts/status/2031952798276075807
- **What:** Claim that Claude Code has lower accuracy (58%) as a harness for Opus 4.6 compared to other tools.

## @aakashgupta - The agentmaxxing guide
> The actual guide to agentmaxxing, since everyone's going to misread this headline:
>
> Replit hit $240 million in revenue in 2025 with roughly 70 employees. That's $3.4 million in revenue per head. A typical SaaS company at that revenue would have 700 people. Replit ran 10x leaner.
>
> Amjad Masad just raised $400 million at a $9 billion valuation and announced he's hiring new grads. But the new grads he's describing aren't traditional CS majors grinding LeetCode. He hired an 18-year-old who never went to CS school, learned to code entirely through AI, and is outperforming classically trained engineers.
>
> Agentmaxxing is a specific workflow. You take an AI coding agent (Replit, Claude Code, Cursor), describe what you want in plain English, let the agent build it, review the output, iterate. One person running 5-10 agents simultaneously replaces a team of 4-5 junior engineers who each need onboarding, management, and code review.
>
> Masad said the quiet part out loud in an interview last year: if you're an engineering manager at Meta, do you hire four junior engineers with all the overhead, or one senior engineer who can spin up 10 agents? Senior engineer salaries have never been higher. New grads who can't orchestrate agents are struggling. New grads who can are getting hired at 18.
>
> The practical stack looks like this:
>
> 1. You become the architect, not the bricklayer. Your job is system design, constraint definition, and quality review.
>
> 2. You manage agents like direct reports. Break work into discrete chunks, assign each to a session, review output, course-correct. The best operators run parallel sessions.
>
> 3. Clarity of thought matters more than syntax knowledge. Masad said the highest-leverage hires right now are clear thinkers and clear communicators. He called them "consultant types."
>
> 4. You ship 10x the surface area. Replit's Agent 1 lasted 2 minutes before losing coherence. Agent 4 runs 3 hours doing production work. That capability is 10xing every few months. By next year, agents handle full-day tasks.
>
> The new grad who gets this builds more in month one than a traditional hire builds in a quarter. The hiring market for juniors didn't collapse. It forked into two lanes: those who manage agents and those who compete against them.
>
> *Quoting @Polymarket:* JUST IN: Replit CEO says company aims to increase hiring in new grads who are vibe coding and "agentmaxxing."

- **Tweet:** https://x.com/aakashgupta/status/2031955029968765442
- **Quoted:** https://x.com/Polymarket/status/2031921219931447806
- **What:** Comprehensive guide to agentmaxxing methodology - using AI coding agents (Replit, Claude Code, Cursor) to amplify productivity. Covers Replit's 10x efficiency gains and Masad's hiring shift toward agent orchestrators over traditional engineers.

## @garrytan - Introducing gstack
> I've been having such an amazing time with Claude Code I wanted you to be able to have my *exact* skill setup:
>
> Introducing gstack, which you can install just by pasting a short piece of text into your Claude code

- **Tweet:** https://x.com/garrytan/status/2032014570118922347
- **What:** Announcement of gstack tool for easily sharing Claude Code skill setups.

## @nurijanian - PM workflow stack with QMD and Obsidian
> If you're a PM who uses Claude Code/Cursor to build and execute research, strategy, and discovery work, this stack cuts context setup from 15 minutes of pasting to under a minute.
>
> Obsidian solves the storage problem: every note you write becomes a local markdown file, yours permanently, readable by any tool, locked to no platform.
>
> The second piece is qmd, a CLI tool built by Tobi Lütke (Shopify's CEO) specifically for searching markdown files, now at 14.5k GitHub stars.
>
> It combines three search approaches running entirely on your machine: BM25 full-text retrieval, vector semantic search via a locally-running 300MB embedding model, and LLM re-ranking for final relevance scoring. No data leaves your laptop.
>
> You point it at a folder, run `qmd embed` to index your entire collection.
>
> What this means in practice: I can open Claude Code and ask it to find every decision I've made about a particular product area, or pull every research note that mentions a specific problem, without manually copying anything.
>
> Claude runs the search, reads the relevant files, and starts from that context rather than from scratch. The time I used to spend pasting background into chat windows before each session now goes into the actual work.
>
> What I didn't expect was how much it compounds. I'm not sure how to quantify it precisely, but every note I add increases the usefulness of future sessions without any extra effort on my part.
>
> Setup to replicate this:
>
> 1. Install Obsidian and import all your notes from wherever you used to store them
> 2. Install QMD (https://github.com/tobi/qmd)

- **Tweet:** https://x.com/nurijanian/status/2032124503330058696
- **Link:** https://github.com/tobi/qmd
- **Filed:** [qmd](./knowledge/tools/qmd.md)
- **What:** PM workflow combining Obsidian for note storage with QMD (Tobi Lütke's CLI search tool) to enable fast, context-aware searches within Claude Code. Reduces 15-minute context setup to under 1 minute with local semantic search, full-text retrieval, and LLM re-ranking.

## @tricalt - X article on self-healing skills
> Bookmark link to article on self-healing AI skills via cognee

- **Tweet:** https://x.com/tricalt/status/2032179887277060476
- **Link:** https://x.com/i/article/2032164771857059840
- **What:** Brief pointer to X article discussing self-healing AI skills and prompt management.

---

# Wednesday, March 11, 2026

## @levelsio - Contrarian Take: MCP Is Dead, APIs Are Enough
> Thank god MCP is dead
>
> Just as useless of an idea as LLMs.txt was
>
> It's all dumb abstractions that AI doesn't need because AI's are as smart as humans so they can just use what was already there which is APIs
>
> *Quoting @morganlinton:* The cofounder and CTO of Perplexity, @denisyarats just said internally at Perplexity they're moving away from MCPs and instead using APIs and CLIs 👀

- **Tweet:** https://x.com/levelsio/status/2031943074151104634
- **Quoted:** https://x.com/morganlinton/status/2031795683897077965
- **What:** Pieter Levels reacting to news that Perplexity's CTO said they're moving away from MCPs internally — arguing MCP is an unnecessary abstraction layer because AI models are now capable enough to just use APIs directly, the same as humans do.


## @Austen - Dotcom Sales Anecdote on Riding a Wave vs. Being Good
> I'm reminded of a story a friend told me from the early days of the dotcom boom when he got the chance to shadow the top salesperson at the hottest company in Silicon Valley.
>
> He said the guy literally just picked up the phone when it would ring and wrote down the orders.
>
> *Quoting @VaibhavSisinty:* Anthropic is valued at $380 billion.
>
> For nearly a year during its fastest growth period, their entire marketing operation was one guy.
>
> Austin Lau, a non-technical growth lead, was running paid search, paid social, email & SEO completely solo.
>
> Just Claude Code & some insane automation he built himself without writing a single line of code.
>
> Here's the exact workflow:
>
> - Export ad performance CSVs into Claude Code
> - AI flags what's underperforming
> - Sub-agent 1 writes headlines
> - Sub-agent 2 writes descriptions
> - Figma plugin auto-swaps copy into 100 ad templates
> - MCP server pulls live Meta data to close the loop
>
> Output went up 10x.
> Creation went from 2 hours to 15 minutes.
>
> Conversion rates beat industry average by 41%.
>
> This isn't AI helping a marketing team.
> This is one person replacing what used to be a 50-person department.

- **Tweet:** https://x.com/Austen/status/2031923349555732869
- **Quoted:** https://x.com/VaibhavSisinty/status/2031745254064631950
- **What:** Austen Allred uses a dotcom-era anecdote to make a pointed observation about Anthropic's growth story: the one-man marketing operation succeeding at massive scale may be more about riding an extraordinary wave than demonstrating novel operational genius.


## @reggitales - "A File System Is Not All You Need" — Arguing for Databases Over Markdown for Agent Context
> the next trillion-dollar product is the agentic workspace.
>
> the actual moat of the next decade is a structured, provenance-aware layer that compounds as you operate.
>
> companies who've solved context are 100 miles ahead.
>
> must read:
>
> *Quoting @kevingu:* https://t.co/dUA8rDkzp5

- **Tweet:** https://x.com/reggitales/status/2031916056760201714
- **Link:** https://x.com/i/article/2031876610975285249
- **What:** An X article arguing that the trendy "put everything in markdown files" approach for AI agent context is fundamentally flawed — markdown gives you grep, not joins or provenance tracking. The better architecture is a database layer that stores extracted info, typed relationships, dependency chains, and pointers back to sources so agents can trace claims to their origin and cascade updates when ground truth changes.


## @NirDiamantAI - agency-agents: 61 Specialized AI Agents for Claude Code
> Claude Code power users, you'll want to see this.
>
> There's a public repo that's basically a complete AI agency for Claude Code: 61 specialized agents across engineering, design, marketing, product, testing, and more, each with a unique personality, workflows, and real deliverables.
>
> Instead of prompting a generic assistant, you activate the exact specialist you need. Security engineer, growth hacker, reality checker, whimsy injector. Drop them into ~/.claude/agents/ and they're ready to go.
> Also works with Cursor, Windsurf, Aider, and Gemini CLI.

- **Tweet:** https://x.com/NirDiamantAI/status/2031854318450544814
- **Link:** https://github.com/msitarzewski/agency-agents
- **What:** A GitHub repo with 61 specialized AI agent persona files (security engineer, growth hacker, frontend developer, etc.) that can be dropped into ~/.claude/agents/ for Claude Code — each agent has a distinct personality, domain expertise, workflows, and deliverables. Also supports Cursor, Windsurf, Aider, and Gemini CLI.


## @nicbstme - /changelog Skill Builds Automatic Audit Trail Across Claude Code Sessions
> My favorite skill I have is /changelog. Every time I close a Claude Code session, it auto appends what happened: emails sent, files created, decisions made.
>
> 104 sessions later in March, I have a full audit trail built without lifting a finger!

- **Tweet:** https://x.com/nicbstme/status/2031846193966563628
- **What:** A Claude Code skill called /changelog that automatically appends a summary of each session's activity (emails sent, files created, decisions made) to a running log, producing a complete audit trail across 100+ sessions with no manual effort.


## @aakashgupta - Running Your Entire Workday with Claude Code (Field CPO Workflow)
> You should be using Claude Code to run your entire work day.
>
> Here's exactly how, from @thevibePM, field CPO at $2.6B @pendoio:
>
> 1:47 - The one command that plans his whole day
> 21:42 - His Claude.MD Setup
> 33:42 - Skills vs MCP vs Hooks
> 40:11 - Why he left Cursor for terminal

- **Tweet:** https://x.com/aakashgupta/status/2031815390108795259
- **What:** Video walkthrough of how a field CPO at Pendo ($2.6B company) uses Claude Code to plan his entire workday, covering CLAUDE.md setup, skills vs MCP vs hooks, and why he switched from Cursor to the terminal.


## @arakharazian - Anthropic Now Default AI Provider for Businesses per Ramp AI Index
> I've seen enough. Anthropic is the new default for businesses.
>
> Says latest Ramp AI Index.

- **Tweet:** https://x.com/arakharazian/status/2031771926557823225
- **What:** The Ramp AI Index, which tracks real business spending data, shows Anthropic has become the default AI provider for businesses — a signal shift in enterprise AI adoption.


## @NickSpisak_ - Building Claude Skill Systems (Plugins): Beyond Individual Skills to Automated Pipelines

You're going to be tempted to bookmark this for later. Don't. Just paste it in your Claude Cowork. It will change how you think about your business process.

> *Quoting @NickSpisak_:* https://t.co/wp3GiDZlKa

- **Tweet:** https://x.com/NickSpisak_/status/2031687075347435930
- **Link:** https://x.com/i/article/2031091883171078144
- **What:** Architecture guide arguing that individual Claude skills hit a ceiling fast — the real leverage comes from connecting skills into systems (plugins) using three patterns: shared context files, output-as-input chaining, and scheduled orchestration. Includes a real four-layer content pipeline as a worked example.


## @itsolelehmann - Claude Skills 2.0: Evals, A/B Benchmarking, and Auto-Optimized Descriptions

claude skills 2.0 quietly launched this week and most people missed it. Anthropic shipped 3 upgrades to skills that fix the problems almost everyone runs into: (1) no way to measure skill performance — now you can run real evals scoring pass/fail rates; (2) skills break silently when models update — now you can A/B compare your skill vs raw Claude to see if it's still earning its place; (3) Claude doesn't use your skill because the description is too vague or specific — Skill Creator now auto-rewrites descriptions for better triggering. Anthropic ran this on their own skills and saw improvement on 5 out of 6.

- **Tweet:** https://x.com/itsolelehmann/status/2031679839476875734
- **Link:** https://x.com/i/article/2031326565460594688
- **What:** Detailed guide to the three major improvements in Claude Skills 2.0: automated eval testing (with pass/fail scoring), A/B benchmarking against baseline Claude, and automatic description optimization to fix skills that fail to trigger at the right time.

## @itsolelehmann - claude skills 2.0 quietly launched this week and most people
> claude skills 2.0 quietly launched this week and most people missed it

anthropic shipped 3 upgrades to skills that fix the problems almost everyone runs into

here's the breakdown (and how to upgrade yours):

problem 1: you had no way to measure how well your skills were actually performing.

now you can run real evals that test your skill against multiple prompts and get a score (like 7/9 passed).

you fix what failed, retest, and repeat until it's dialed in.

•

problem 2: your skills break when models update and you don't notice.

say you wrote a skill 3 months ago when claude needed detailed instructions for landing pages.

now claude is way better at landing pages by default

but your old skill is still forcing it to follow outdated steps instead of using its own improved abilities.

now you can run a/b comparisons between your skill and raw claude

so you know if a skill is still earning its place or if you should fix/retire it.

•

problem 3: claude doesn't even use your skill half the time because the description is too vague or too specific.

now the skill creator rewrites your descriptions automatically so they trigger at the right time.

anthropic ran this on their own skills and saw better triggering on 5 out of 6.

i cooked a full step-by-step breakdown below
>
> *Quoting @itsolelehmann:* https://t.co/jzOGxmkyhx...

- **Tweet:** https://x.com/itsolelehmann/status/2031679839476875734
- **Quoted:** https://x.com/itsolelehmann/status/2031461162768867622
- **What:** claude skills 2.0 quietly launched this week and most people

## @NickSpisak_ - You’re going to be tempted to bookmark this for later.  
> You’re going to be tempted to bookmark this for later.  

Don’t.  

Just paste it in your Claude Cowork.  

It will change how you think about your business process.
>
> *Quoting @NickSpisak_:* https://t.co/wp3GiDZlKa...

- **Tweet:** https://x.com/NickSpisak_/status/2031687075347435930
- **Quoted:** https://x.com/NickSpisak_/status/2031097135865761972
- **What:** You’re going to be tempted to bookmark this for later.

## @arakharazian - I've seen enough. Anthropic is the new default for businesse
> I've seen enough. Anthropic is the new default for businesses.

Says latest Ramp AI Index. https://t.co/E85qfcby5u

- **Tweet:** https://x.com/arakharazian/status/2031771926557823225
- **Link:** https://twitter.com/arakharazian/status/2031771926557823225/photo/1
- **What:** I've seen enough. Anthropic is the new default for businesse

## @aakashgupta - You should be using Claude Code to run your entire work day
> You should be using Claude Code to run your entire work day. 

Here's exactly how, from @thevibePM, field CPO at $2.6B @pendoio:

1:47 - The one command that plans his whole day 
21:42 - His Claude.MD Setup
33:42 - Skills vs MCP vs Hooks 
40:11 - Why he left Cursor for terminal https://t.co/fi5v5GN3S6

- **Tweet:** https://x.com/aakashgupta/status/2031815390108795259
- **Link:** https://twitter.com/aakashgupta/status/2031815390108795259/video/1
- **What:** You should be using Claude Code to run your entire work day

## @nicbstme - My favorite skill I have is /changelog. Every time I close a
> My favorite skill I have is /changelog. Every time I close a Claude Code session, it auto appends what happened: emails sent, files created, decisions made. 

104 sessions later in March, I have a full audit trail built without lifting a finger! https://t.co/bcbFt75z66

- **Tweet:** https://x.com/nicbstme/status/2031846193966563628
- **Link:** https://twitter.com/nicbstme/status/2031846193966563628/photo/1
- **What:** My favorite skill I have is /changelog. Every time I close a

## @NirDiamantAI - Claude Code power users, you'll want to see this
> Claude Code power users, you'll want to see this.

There's a public repo that's basically a complete AI agency for Claude Code: 61 specialized agents across engineering, design, marketing, product, testing, and more, each with a unique personality, workflows, and real deliverables.

Instead of prompting a generic assistant, you activate the exact specialist you need. Security engineer, growth hacker, reality checker, whimsy injector. Drop them into ~/.claude/agents/ and they're ready to go.
Also works with Cursor, Windsurf, Aider, and Gemini CLI.

Repo:
https://t.co/AigPxno7tv

- **Tweet:** https://x.com/NirDiamantAI/status/2031854318450544814
- **Link:** https://github.com/msitarzewski/agency-agents
- **Filed:** [agency-agents](./knowledge/tools/agency-agents.md)
- **What:** A public GitHub repo (agency-agents) containing 61 specialized AI agents — covering engineering, design, marketing, product, and testing — each with a distinct personality and real deliverables, designed to drop into ~/.claude/agents/ and work across Claude Code, Cursor, Windsurf, Aider, and Gemini CLI.

## @reggitales - the next trillion-dollar product is the agentic workspace
> the next trillion-dollar product is the agentic workspace.

the actual moat of the next decade is a structured, provenance-aware layer that compounds as you operate.

companies who've solved context are 100 miles ahead.

must read:
>
> *Quoting @kevingu:* https://t.co/dUA8rDkzp5...

- **Tweet:** https://x.com/reggitales/status/2031916056760201714
- **Quoted:** https://x.com/kevingu/status/2031889622385729730
- **What:** the next trillion-dollar product is the agentic workspace

## @Austen - Dotcom salesperson lesson on sales effectiveness
> I'm reminded of a story a friend told me from the early days of the dotcom boom when he got the chance to shadow the top salesperson at the hottest company in Silicon Valley.
>
> He said the guy literally just picked up the phone when it would ring and wrote down the orders.
>
> *Quoting @VaibhavSisinty:* Anthropic is valued at $380 billion.
>
> For nearly a year during its fastest growth period, their entire marketing operation was one guy.
>
> Austin Lau, a non-technical growth lead, was running paid search, paid social, email & SEO completely solo.
>
> Just Claude Code & some insane automation he built himself without writing a single line of code.
>
> Here's the exact workflow:
>
> - Export ad performance CSVs into Claude Code
> - AI flags what's underperforming
> - Sub-agent 1 writes headlines
> - Sub-agent 2 writes descriptions
> - Figma plugin auto-swaps copy into 100 ad templates
> - MCP server pulls live Meta data to close the loop
>
> Output went up 10x.
> Creation went from 2 hours to 15 minutes.
> Conversion rates beat industry average by 41%.
>
> This isn't AI helping a marketing team.
> This is one person replacing what used to be a 50-person department.

- **Tweet:** https://x.com/Austen/status/2031923349555732869
- **Quoted:** https://x.com/VaibhavSisinty/status/2031745254064631950
- **What:** Commentary on Anthropic's one-person marketing operation using Claude Code and agentic automation to achieve 10x output, replacing a 50-person department.

## @levelsio - Critique of MCP abstraction
> Thank god MCP is dead
>
> Just as useless of an idea as LLMs.txt was
>
> It's all dumb abstractions that AI doesn't need because AI's are as smart as humans so they can just use what was already there which is APIs
>
> *Quoting @morganlinton:* The cofounder and CTO of Perplexity, @denisyarats just said internally at Perplexity they're moving away from MCPs and instead using APIs and CLIs

- **Tweet:** https://x.com/levelsio/status/2031943074151104634
- **Quoted:** https://x.com/morganlinton/status/2031795683897077965
- **What:** Critique arguing MCPs are unnecessary abstractions, noting that Perplexity's CTO is moving away from MCPs toward direct APIs and CLIs.

---

# Tuesday, March 10, 2026

## @trader1sz - Video: Stop What You're Doing and Watch This

Stop what you are doing and watch this

- **Tweet:** https://x.com/trader1sz/status/2031492114161258562
- **What:** A short video share with no additional context provided in the tweet; content of the video is not described.


## @itsolelehmann - Anthropic's Entire Growth Marketing Run by One Person Using Claude Code

i can't believe nobody caught this. Anthropic's entire growth marketing team was just ONE PERSON (for 10 months, confirmed). A single non-technical person ran paid search, paid social, app stores, email marketing, and SEO for the $380B company behind Claude. He feeds CSVs of ad performance into Claude Code, generates hundreds of new copy variations, uses a Figma plugin to auto-swap copy into ad templates (100 variations at half a second per batch), built an MCP server connected to the Meta Ads API so he can query live campaign data in plain English, and runs a memory system that logs all experiments so the system gets smarter each cycle. Ad creation went from 2 hours to 15 minutes. 10x more creative output.

- **Tweet:** https://x.com/itsolelehmann/status/2031308486815133905
- **What:** Breakdown of how Anthropic's solo growth marketer used Claude Code, MCP servers, Figma automation, and experiment memory loops to run paid search, social, email, and SEO for a company valued at $380B — cutting ad creation time from 2 hours to 15 minutes.


## @shivsakhuja - 50+ Free Claude Code GTM Skills Library

Over the last few months, we've been using Claude Code to do practically all our GTM execution work. Not just coding. Everything. Running outbound campaigns, finding high-intent leads and candidates, creating SEO pages, running marketing campaigns, managing my CRM, even finding apartments. Claude can truly do anything you need. It just needs the right setup + skills. So we created a library of skills that teach Claude how to do GTM work. Things like: Scraping reddit for your ICP's pain points, Monitoring your competitors posts across all social channels, Finding leads from comments on LinkedIn posts, Enriching & qualifying leads, Scraping reviews, Creating slides & graphics, Auditing your SEO / content strategy. It's completely free and has over 50 skills specifically designed for GTM skills.

- **Tweet:** https://x.com/shivsakhuja/status/2031253674778046906
- **What:** Announcement of a free, open-source library of 50+ Claude Code skills for GTM (go-to-market) work — covering lead gen, competitor monitoring, SEO audits, outbound campaigns, and more — built from real production use by the author's team.


## @aakashgupta - OpenAI Acquires Promptfoo: Buying Enterprise Distribution, Not Just a Security Tool

> We're acquiring Promptfoo.
>
> Their technology will strengthen agentic security testing and evaluation capabilities in OpenAI Frontier. Promptfoo will remain open source under the current license, and we will continue to service and support current customers.
>
> *Quoting @OpenAI:* We're acquiring Promptfoo.

Promptfoo raised $23M, hit an $86M valuation 8 months ago, and was already used by 25% of the Fortune 500. OpenAI just bought them 5 weeks after launching Frontier. The math tells the story. Promptfoo built the most widely adopted AI security testing tool in the world on $23M in funding. Over 125 Fortune 500 companies running it in production. Open source CLI with 300,000+ developers. Backed by a16z and Insight Partners. The entire company was essentially a CI/CD pipeline for AI red-teaming, and they built it in under two years...

- **Tweet:** https://x.com/aakashgupta/status/2031224956235952365
- **Link:** https://openai.com/index/openai-to-acquire-promptfoo/
- **What:** Analysis of OpenAI's acquisition of Promptfoo, arguing the real value wasn't the security tool itself but the pre-approved relationships with 125+ Fortune 500 security teams — procurement trust that would have taken Frontier years to build organically.


## @RandomSprint - Dunbar Number and the "I'm Putting Together a Team" Bio

> i keep a list of good bios
>
> when i tell this to people, everyone starts sending me good ones too
>
> so i made a page of good bios, you tap to reveal whose
>
> *Quoting @melissa:* i keep a list of good bios
>
> when i tell this to people, everyone starts sending me good ones too
>
> so i made a page of good bios, you tap to reveal whose

This has my old bio on it. "I'm putting together a team." I changed it after I zoomed past my Dunbar Number.

- **Tweet:** https://x.com/RandomSprint/status/2031224791244357820
- **What:** RandomSprint quotes a thread about a curated page of memorable Twitter bios, noting he removed his own memorable bio ("I'm putting together a team") after his network grew beyond the Dunbar Number (~150 social connections).


## @Seanfrank - $2.87M Spent Profitably on AppLovin Ads

> *Quoting @AaronOrendorff:* HOW DO YOU SPEND MORE … PROFITABLY? That's the #1 question we get. On Mar 18, +25 ecom leaders w/ a combined budget bigger than any European nation's GDP are going to reveal their answers.
>
> In less than 12 months, I have spent $2,872,421 of my own money PROFITABLY on applovin
>
> I do not own the stock.
> I do not trade the stock.
> This is the net amount that left my bank account.
>
> The ads work on par with Meta or Google.
> It has proven to be 10x more scalable than reddit
>
> Want to learn how we do this?
> Aaron is running a free training below

- **Tweet:** https://x.com/Seanfrank/status/2031219661657059421
- **Link:** https://www.9operators.com/paid-growth?utm_source=social&utm_medium=twitter&utm_campaign=aaron
- **What:** Sean Frank (Ridge Wallet) endorsing AppLovin as a paid ads channel on par with Meta/Google and 10x more scalable than Reddit, promoting an Operators paid growth masterclass with 25+ DTC leaders.

## @Seanfrank - In less than 12 months, I have spent $2,872,421 of my own mo
> In less than 12 months, I have spent $2,872,421 of my own money PROFITABLY on applovin

I do not own the stock.
I do not trade the stock. 
This is the net amount that left my bank account.

The ads work on par with Meta or Google.
It has proven to be 10x more scalable than reddit

Want to learn how we do this?
Aaron is running a free training below

I think it is worth attending if you are currently spending upwards of 500k a month or more on meta-

OR have clients that do
>
> *Quoting @AaronOrendorff:* HOW DO YOU SPEND MORE …
PROFITABLY?

That’s the #1 question we get.

On Mar 18, +25 ecom leaders w/ a combined budget bigger than any European nation’s GDP are going to reveal their answers.

Spoiler: Most of it ain’t in your ad account ↓ lineup below

https://t.co/8x7e7on5Mj

- **Tweet:** https://x.com/Seanfrank/status/2031219661657059421
- **Quoted:** https://x.com/AaronOrendorff/status/2031155110336930158
- **Filed:** [Paid Growth Training](./knowledge/articles/paid-growth-9operators.md)
- **What:** In less than 12 months, I have spent $2,872,421 of my own money PROFITABLY on ap

## @RandomSprint - This has my old bio on it. "I'm putting together a team." I 
> This has my old bio on it. "I'm putting together a team." I changed it after I zoomed past my Dunbar Number.
>
> *Quoting @melissa:* i keep a list of good bios

when i tell this to people, everyone starts sending me good ones too

so i made a page of good bios, you tap to reveal whose https://t.co/SGLapj8LtV

- **Tweet:** https://x.com/RandomSprint/status/2031224791244357820
- **Quoted:** https://x.com/melissa/status/2031215893989175407
- **What:** This has my old bio on it. "I'm putting together a team." I changed it after I z

## @aakashgupta - Promptfoo raised $23M, hit an $86M valuation 8 months ago, a
> Promptfoo raised $23M, hit an $86M valuation 8 months ago, and was already used by 25% of the Fortune 500.

OpenAI just bought them 5 weeks after launching Frontier.

The math tells the story. Promptfoo built the most widely adopted AI security testing tool in the world on $23M in funding. Over 125 Fortune 500 companies running it in production. Open source CLI with 300,000+ developers. Backed by a16z and Insight Partners. The entire company was essentially a CI/CD pipeline for AI red-teaming, and they built it in under two years.

OpenAI could have built this internally. They have thousands of engineers and billions in capital. They chose to buy instead because Promptfoo already had the distribution. 125+ Fortune 500 companies already trust Promptfoo’s security reports. That trust is the product OpenAI actually acquired. You can’t replicate “your CISO already approved this vendor” with a feature sprint.

This is the playbook for the entire enterprise agent platform war. Salesforce, Google, Microsoft, Anthropic are all racing to ship agent platforms. The bottleneck isn’t model intelligence or tool integration. The bottleneck is procurement. Enterprise security teams gate every agent deployment. Whoever controls the security validation layer controls the speed at which agents get approved for production.

OpenAI just bought the fastest path through the CISO’s office.

And the acquisition price is probably the most interesting part nobody’s discussing. $86M valuation on a company used by a quarter of the Fortune 500. That’s absurdly cheap per enterprise relationship. Promptfoo had penetrated more Fortune 500 security teams than Frontier had total customers. OpenAI didn’t buy a security tool. They bought 125+ pre-approved enterprise relationships and a distribution channel that would have taken Frontier years to build organically.

The companies still building their own security testing layers are now 125 enterprise relationships behind.
>
> *Quoting @OpenAI:* We’re acquiring Promptfoo.

Their technology will strengthen agentic security testing and evaluation...

- **Tweet:** https://x.com/aakashgupta/status/2031224956235952365
- **Quoted:** https://x.com/OpenAI/status/2031052793835106753
- **What:** Promptfoo raised $23M, hit an $86M valuation 8 months ago, a

## @shivsakhuja - Over the last few months, we've been using Claude Code to do
> Over the last few months, we've been using Claude Code to do practically all our GTM execution work. 

Not just coding. Everything.

Running outbound campaigns, finding high-intent leads and candidates, creating SEO pages, running marketing campaigns, managing my CRM, even finding apartments.

Claude can truly do anything you need. It just needs the right setup + skills.

So we created a library of skills that teach Claude how to do GTM work. Things like:

- Scraping reddit for your ICP's pain points
- Monitoring your competitors posts across all social channels
- Finding leads from comments on LinkedIn posts
- Enriching & qualifying leads
- Scraping reviews 
- Creating slides & graphics
- Auditing your SEO / content strategy

It's completely free and has over 50 skills specifically designed for GTM skills. 

Link + OSS below 👇

- **Tweet:** https://x.com/shivsakhuja/status/2031253674778046906
- **What:** Over the last few months, we've been using Claude Code to do

## @itsolelehmann - i can't believe nobody caught this
> i can't believe nobody caught this.

Anthropic's entire growth marketing team was just ONE PERSON

(for 10 months, confirmed)

a single non-technical person ran paid search, paid social, app stores, email marketing, and SEO for the $380B company behind claude

here's exactly how one human is doing the job of a full marketing team:

it starts with a CSV.

1. he exports all his existing ads from his ad platforms along with their performance metrics (click-through rates, conversions, spend, etc)

2. feeds the whole file into claude code

3. and tells it to find what's underperforming.

claude analyzes the data, flags the weak ads, and generates new copy variations on the spot

this is where he gets clever:

he then splits the work into 2 specialized sub-agents:

1. one that only writes headlines (capped at 30 characters)

2. and one that only writes descriptions (capped at 90 characters).

each agent is tuned to its specific constraint so the quality is way higher than cramming both into a single prompt

so now he's got hundreds of fresh headlines and descriptions.

but that's just the text.

he still needs the actual visual ad creative, the images and banners that go on facebook, google, etc.

so he built a figma plugin that:

1. takes all those new headlines and descriptions
2. finds the ad templates in his figma files
3. and automatically swaps the copy into each one.

up to 100 ready-to-publish ad variations generated at half a second per batch.

what used to take hours of duplicating frames and copy-pasting text by hand

so now the ads are live.

the next question is which ones are actually working.

for that he built an MCP server (basically a custom integration that lets claude talk directly to external tools) connected to the meta ads API.

so he can ask claude things like:

• "which ads had the best conversion rate this week"
• or "where am i wasting spend"

and get real answers from live campaign data without ever opening the meta ads dashboard

and the part that ties it all together and closes the loop:

he set up a memory system that logs every hypothesis and experiment result across ad iterations.

so when he goes back to step one and generates the next batch of variations...

claude automatically pulls in what worked and what didn't from all previous rounds.

the system literally gets smarter every cycle.

that kind of systematic experimentation across hundreds of ads would normally need a dedicated analytics person just to track

the numbers from the doc:

ad creation went from 2 hours to 15 minutes. 10x more creative output.

and he's now testing more variations across more channels than most full marketing teams

a $380 billion company.

and their entire growth marketing operation (not GTM) = just one person and claude code lol

truly unbelievable

- **Tweet:** https://x.com/itsolelehmann/status/2031308486815133905
- **What:** A detailed breakdown of how Anthropic's single growth marketer used Claude Code, specialized sub-agents, a custom Figma plugin, and an MCP server connected to the Meta Ads API to reduce ad creation from 2 hours to 15 minutes and 10x creative output — running the full paid search, social, email, and SEO operation for a $380B company alone.

## @trader1sz - Video Worth Stopping Everything For
> Stop what you are doing and watch this

- **Tweet:** https://x.com/trader1sz/status/2031492114161258562
- **What:** Urgent video recommendation from a trader—no context given, just a strong call to action to watch the linked video.

---

---

# Monday, March 9, 2026

## @toddsaunders - Stripe's Token Billing Is a Play for AI Infrastructure Dominance

> I think @stripe just mass produced a business model for every AI startup on earth and increased their TAM exponentially.
>
> Customer buys a shirt for $40, Stripe takes 2.9% + 30 cents. It's a simple formula, but token billing is completely different.
>
> AI costs are variable. They shift by model, by provider, by week. A startup using Claude for 40% of inference and GPT-4o for 60% has a blended cost structure that changes every time Anthropic or OpenAI adjusts pricing... which is constantly.
>
> Stripe is now ingesting those real-time model prices, applying the startup's target markup, metering per-customer usage, and generating the invoice automatically.
>
> That's constructing unit economics at a scale and complexity far beyond anything in traditional payments.
>
> And the data asset being created by them is a massive moat.
>
> OpenAI knows what OpenAI charges, and Anthropic knows what Anthropic charges. But Stripe will know what every model charges, what every startup pays, what every startup marks up, and what every end customer actually consumes.
>
> But the gateway is where this gets really interesting.
>
> Stripe's AI gateway routes inference, returns the response, and attributes tokens to the customer in one API call.
>
> Today it's "pick the best model."
>
> Tomorrow it's "Stripe recommends the model that optimizes your target margin across 12 providers in real time."
>
> The moment that recommendation engine turns on, model providers start competing on Stripe's terms. Pricing power inverts from provider to platform.
>
> This is AWS turned sideways (or i guess diagonally).
>
> Amazon didn't build apps... they built the infrastructure every app depended on, then used the data to optimize the infrastructure itself.
>
> Stripe is running the same playbook on AI economics instead of AI compute.
>
> I truly believe that token billing will make Stripe the most strategically important company in tech that doesn't train a model.

- **Tweet:** https://x.com/toddsaunders/status/2031158356606332936
- **What:** Analysis of Stripe's token billing and AI gateway product as a structural power grab: Stripe will accumulate cross-provider pricing and margin data that no single model provider has, then use its inference routing layer to flip pricing power from AI providers to platform — the AWS playbook applied to AI economics.


## @bcherny - Why Separate Context Windows Make AI Agents Find Their Own Bugs

> *Replying to @Rahll:* If Claude Code is so good, why do they need a separate feature to hunt for bugs.
>
> 👋 Roughly, the more tokens you throw at a coding problem, the better the result is. We call this test time compute.
>
> One way to make the result even better is to use separate context windows. This is what makes subagents work, and also why one agent can cause bugs and another (using the same exact model!) can find them. In a way, it's similar to engineers — if I cause a bug, my coworker reviewing the code might find it more reliably than I can.
>
> In the limit, agents will probably write perfect bug-free code. Until we get there, multiple uncorrelated context windows tends to be a good approach.

- **Tweet:** https://x.com/bcherny/status/2031151689219321886
- **What:** Boris Cherny (Claude Code) explaining that subagents work because separate context windows are uncorrelated — the same model that introduced a bug is less likely to catch it in the same context, just as a human author misses their own errors. More test-time compute via independent windows improves results.


## @ericrovner - AI Writing Clichés to Add to Your Mute List

> *Replying to @emollick:* Get better prompts.
>
> @emollick More for your mute list…
>
> But here's the catch
> Here's the thing most people miss
> What most people miss
> But here's what nobody is saying
> It's not just about X. It's about Y.
> The reality is
> This is where it gets interesting

- **Tweet:** https://x.com/ericrovner/status/2031075436063608899
- **What:** A list of AI-generated writing phrases that have become so common they signal low-effort content — contributed to a thread started by Ethan Mollick about prompting better to avoid generic AI output patterns.


## @swyx - Open Source AI Engineering as an Acquihire Path

> btw if you can build a category leader open source project in ai engineering right now the market acquihire rate is ~$10-$100m per ai engineer.
>
> you do not need to figure out a business model, you do not need GTM, you do not need funding.
>
> just build things clankers want.

- **Tweet:** https://x.com/swyx/status/2031071059307601944
- **What:** swyx observing that the acquihire market for AI engineering talent is pricing category-leading open source projects at $10–100M per engineer, making GTM and funding irrelevant — just build tools AI engineers ("clankers") actually use.


## @shannholmberg - Three AI Moats: Taste, Distribution, and High Agency

> [X Article: Everyone using AI has about 12 months to develop these 3 moats]

- **Tweet:** https://x.com/shannholmberg/status/2031049690175652235
- **Link:** https://x.com/i/article/2031045451311427585
- **What:** A long-form X article arguing that as AI commoditizes output, the only durable advantages are taste (knowing what good looks like and overriding defaults), distribution (trust built over time, not posting volume), and high agency (figuring things out without a tutorial). The 80/20 rule: let AI handle 80% of production, pour your judgment into the last 20%.

## @shannholmberg - https://t.co/GxOCDTpInz
> https://t.co/GxOCDTpInz

- **Tweet:** https://x.com/shannholmberg/status/2031049690175652235
- **What:** LINK_FAILED: Could not expand link from @shannholmberg — original t.co URL did not resolve.

## @swyx - btw if you can build a category leader open source project i
> btw if you can build a category leader open source project in ai engineering right now the market acquihire rate is ~$10-$100m per ai engineer.

you do not need to figure out a business model, you do not need GTM, you do not need funding.

just build things clankers want.

- **Tweet:** https://x.com/swyx/status/2031071059307601944
- **What:** btw if you can build a category leader open source project in ai engineering rig

## @ericrovner - @emollick More for your mute list…
> *Replying to @emollick:* Get better prompts. https://t.co/uvcUU3vYxU
>
> @emollick More for your mute list…

But here’s the catch
Here’s the thing most people miss
What most people miss
But here’s what nobody is saying
It’s not just about X. It’s about Y. 
The reality is
This is where it gets interesting

- **Tweet:** https://x.com/ericrovner/status/2031075436063608899
- **Parent:** https://x.com/emollick/status/2031065480203526654
- **What:** A sarcastic reply to Ethan Mollick listing the most overused AI-hype filler phrases in prompts and social posts ('Here's the catch', 'What most people miss', 'This is where it gets interesting', etc.) — surfacing a real pattern of hollow AI content framing.

## @bcherny - 👋 Roughly, the more tokens you throw at a coding problem, th
> *Replying to @Rahll:* If Claude Code is so good, why do they need a separate feature to hunt for bugs.
>
> 👋 Roughly, the more tokens you throw at a coding problem, the better the result is. We call this test time compute.

One way to make the result even better is to use separate context windows. This is what makes subagents work, and also why one agent can cause bugs and another (using the same exact model!) can find them. In a way, it’s similar to engineers — if I cause a bug, my coworker reviewing the code might find it more reliably than I can.

In the limit, agents will probably write perfect bug-free code. Until we get there, multiple uncorrelated context windows tends to be a good approach.

- **Tweet:** https://x.com/bcherny/status/2031151689219321886
- **Parent:** https://x.com/Rahll/status/2031097736536166420
- **What:** 👋 Roughly, the more tokens you throw at a coding problem, the better the result

## @toddsaunders - I think @stripe just mass produced a business model for ever
> I think @stripe just mass produced a business model for every AI startup on earth and increased their TAM exponentially. 

Customer buys a shirt for $40, Stripe takes 2.9% + 30 cents. It's a simple formula, but token billing is completely different.

AI costs are variable. They shift by model, by provider, by week. A startup using Claude for 40% of inference and GPT-4o for 60% has a blended cost structure that changes every time Anthropic or OpenAI adjusts pricing... which is constantly.

Stripe is now ingesting those real-time model prices, applying the startup's target markup, metering per-customer usage, and generating the invoice automatically.

That's constructing unit economics at a scale and complexity far beyond anything in traditional payments.

And the data asset being created by them is a massive moat.

OpenAI knows what OpenAI charges, and Anthropic knows what Anthropic charges. But Stripe will know what every model charges, what every startup pays, what every startup marks up, and what every end customer actually consumes.

But the gateway is where this gets really interesting.

Stripe's AI gateway routes inference, returns the response, and attributes tokens to the customer in one API call.

Today it's "pick the best model."

Tomorrow it's "Stripe recommends the model that optimizes your target margin across 12 providers in real time."

The moment that recommendation engine turns on, model providers start competing on Stripe's terms. Pricing power inverts from provider to platform.

This is AWS turned sideways (or i guess diagonally).

Amazon didn't build apps... they built the infrastructure every app depended on, then used the data to optimize the infrastructure itself.

Stripe is running the same playbook on AI economics instead of AI compute.

I truly believe that token billing will make Stripe the most strategically important company in tech that doesn't train a model.

- **Tweet:** https://x.com/toddsaunders/status/2031158356606332936
- **What:** I think @stripe just mass produced a business model for every AI startup on eart

---

# Sunday, March 8, 2026

## @mdnlabs - Automated YouTube Content System Hitting 7M Views

> *Quoting @maubaron:* [X Article: We got 7M views on YouTube with completely automated content]
>
> GUYS IM FREAKING OUT RIGHT NOW
>
> Time to pull 250+ videos 😎😎😎

- **Tweet:** https://x.com/mdnlabs/status/2030807267755294988
- **Link:** https://x.com/i/article/2029564042390503424
- **What:** An X article by @maubaron describing a fully automated YouTube channel system that reached 7M views and 61k subscribers: scrape viral video hooks (e.g. ZackD Films), stitch a CTA clip onto the first 3 seconds using Claude Code-generated Python scripts, then schedule with a posting tool. Takes ~10 minutes to produce 700 posts.


## @noisyb0y1 - Anthropic's 33-Page Complete Guide to Building Claude Skills
> Anthropic dropped a Prediction Market trading bot structure
>
> $300-$1,500 a day
>
> 33 pages cheat sheet for building Claude skills, and 2 of them are hidden under a trading bot that trades at 68.4% win rate
>
> if i had seen these documents earlier i would have saved myself a few months of analysis
>
> *Quoting @RoundtableSpace:* Anthropic dropped a 33 pages cheat sheet for building Claude skills

- **Tweet:** https://x.com/noisyb0y1/status/2030688100574167201
- **Link:** https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf
- **What:** Highlights Anthropic's official 33-page PDF guide to building Claude skills, with the tweeter noting it also contains examples of a prediction market trading bot structure with a claimed 68.4% win rate. Filed as a reference article for the Claude skills guide.

## @noisyb0y1 - Anthropic dropped a Prediction Market trading bot structure
> Anthropic dropped a Prediction Market trading bot structure

$300-$1,500 a day

33 pages cheat sheet for building Claude skills, and 2 of them are hidden under a trading bot that trades at 68.4% win rate

if i had seen these documents earlier i would have saved myself a few months of analysis
>
> *Quoting @RoundtableSpace:* Anthropic dropped a 33 pages cheat sheet for building Claude skills

https://t.co/jEuH95NGn3 https://t.co/udwk64U4ST

- **Tweet:** https://x.com/noisyb0y1/status/2030688100574167201
- **Quoted:** https://x.com/RoundtableSpace/status/2030595632998580328
- **Filed:** [Claude Skills Guide](./knowledge/articles/claude-skills-guide.md)
- **What:** Anthropic dropped a Prediction Market trading bot structure

## @mdnlabs - GUYS IM FREAKING OUT RIGHT NOW
> GUYS IM FREAKING OUT RIGHT NOW

Time to pull 250+ videos 😎😎😎 https://t.co/qdItZhZYMK
>
> *Quoting @maubaron:* https://t.co/rk9fLhpRO3

- **Tweet:** https://x.com/mdnlabs/status/2030807267755294988
- **Quoted:** https://x.com/maubaron/status/2030716132093460742
- **What:** THIN: Excited reaction to a quoted post that appears to show a new capability or tool enabling bulk video processing — the author plans to use it to pull 250+ videos, but the quoted content didn't fully expand.

---

# Saturday, March 7, 2026

## @cryptopunk7213 - Karpathy's autoresearch Democratizes Single-GPU LLM Training Research
> karpathy really is the fucking goat.
>
> - built an AI agent that autonomously self-improves while you sleep and made it FREE for anyone to use
>
> - we're talking about an AI that gets smarter over night and runs itself.
>
> - executes 100 experiments (1 every 5 mins), if it gets smarter it upgrades if it doesn't it discards and tries again.
>
> - only requires 1 gpu to run
>
> *Quoting @karpathy:* I packaged up the "autoresearch" project into a new self-contained minimal repo if people would like to play over the weekend. It's basically nanochat LLM training core stripped down to a single-GPU, one file version of ~630 lines of code, then: the human iterates on the prompt (.md) / the AI agent iterates on the training code (.py). The goal is to engineer your agents to make the fastest research progress indefinitely and without any of your own involvement.

- **Tweet:** https://x.com/cryptopunk7213/status/2030457601465393572
- **Link:** https://github.com/karpathy/autoresearch
- **What:** Ejaaz's reaction to karpathy's autoresearch — emphasizing its democratizing potential: anyone with a single GPU can now run an autonomous overnight research loop that was previously only accessible to large AI labs with massive compute budgets.


## @godofprompt - Affaan Mustafa's Claude Code Refinement System: 14+ Agents, 56+ Skills, 33+ Commands
> 🚨 BREAKING: An Anthropic hackathon winner just gave away the entire system for free.
>
> @affaanmustafa beat 100+ participants at the Anthropic x Forum Ventures hackathon. Built https://t.co/uUCLO7rALB in 8 hours using Claude Code. Walked away with $15K in API credits.
>
> Then he packaged 10+ months of daily Claude Code refinement into one repo:
>
> → 14+ agents, 56+ skills, 33+ commands
> → MCP configs, hooks, rules
> → AgentShield security scanner
> → Continuous learning system
> → Full cross-platform support
>
> 35,000+ stars. MIT licensed. One install command.

- **Tweet:** https://x.com/godofprompt/status/2030434516397891732
- **Link:** https://zenith.chat/
- **What:** Promotion of Affaan Mustafa's open-source Claude Code setup system, which bundles 10+ months of Claude Code workflow refinement into a single installable repo including agents, skills, commands, MCP configs, hooks, and an AgentShield security scanner. The referenced hackathon project (Zenith) was an AI-powered customer discovery platform.


## @odysseus0z - openai/symphony: Cron-Based Agent Dispatch Loop Using Linear as Work Queue
> TLDR: it is a cron job dispatching tickets from Linear to workers, each of which is a Ralph loop using a Linear comment as draft pad for persisted state.
>
> Yes it is all you need.
>
> Beautifully designed and minimal.

- **Tweet:** https://x.com/odysseus0z/status/2030413782036726181
- **Link:** https://github.com/openai/symphony
- **What:** George's take on OpenAI's Symphony — a minimal agent orchestration system that monitors a Linear board for tasks, dispatches them to autonomous coding agents, and persists agent state in Linear comments. He frames it as essentially a cron job + REPL loop, and notes that elegantly minimal design is its strength.


## @LiorOnAI - karpathy/autoresearch: Autonomous AI Research Agent That Runs 100 Experiments Overnight
> It's over. Karpathy just open-sourced an autonomous AI researcher that runs 100 experiments while you sleep.
>
> You don't write the training code anymore.
>
> You write a prompt that tells an AI agent how to think about research.
>
> The agent edits the code, trains a small language model for exactly five minutes, checks the score, keeps or discards the result, and loops. All night. No human in the loop.
>
> *Quoting @karpathy:* I packaged up the "autoresearch" project into a new self-contained minimal repo if people would like to play over the weekend. It's basically nanochat LLM training core stripped down to a single-GPU, one file version of ~630 lines of code, then: the human iterates on the prompt (.md) / the AI agent iterates on the training code (.py). The goal is to engineer your agents to make the fastest research progress indefinitely and without any of your own involvement.

- **Tweet:** https://x.com/LiorOnAI/status/2030376700337643742
- **Link:** https://github.com/karpathy/autoresearch
- **What:** Lior Alexander's breakdown of karpathy's autoresearch repo — an autonomous ML research framework where an AI agent runs fixed 5-minute training experiments in a loop (~100/night), modifying `train.py` while the human only edits a `program.md` instruction file. The fixed time budget ensures all runs are directly comparable.


## @RoundtableSpace - Anthropic Ships 27+ Features and Integrations in Two Weeks
> Anthropic shipped all of these in two weeks:
>
> - claude code security
> - voice mode in claude code
> - free memory feature
> - memory import tool
> - claude marketplace
> - investment banking plug-in
> - wealth management plug-in
> - human resources plug-in
> - private equity plug-in
> - engineering plug-in
> - design plug-in
> - equity research plug-in
> - operations plug-in
> - brand voice / style plug-in
> - google calendar integration
> - gmail integration
> - google drive integration
> - docusign integration
> - clay integration
> - factset / msci / s&p global / lseg data feeds
> - cobol legacy modernization (claude code)
> - claude sonnet 4.6 launch
> - health & fitness data on ios/android
> - cowork scheduled tasks
> - vercept acquisition
> - structured outputs & web search went GA
> - data residency controls (api)

- **Tweet:** https://x.com/RoundtableSpace/status/2030281500298743819
- **What:** A roundup of Anthropic's shipping velocity — 27+ distinct features released in a two-week span, including Claude Marketplace plug-ins for finance/HR/design, major integrations (Google Workspace, DocuSign, Clay), Claude Sonnet 4.6, structured outputs going GA, and the Vercept acquisition.

## @RoundtableSpace - Anthropic shipped all of these in two weeks:...
> Anthropic shipped all of these in two weeks:

- claude code security
- voice mode in claude code
- free memory feature
- memory import tool
- claude marketplace
- investment banking plug-in
- wealth management plug-in
- human resources plug-in
- private equity plug-in
- engineering plug-in
- design plug-in
- equity research plug-in
- operations plug-in
- brand voice / style plug-in
- google calendar integration
- gmail integration
- google drive integration
- docusign integration
- clay integration
- factset / msci / s&p global / lseg data feeds
- cobol legacy modernization (claude code)
- claude sonnet 4.6 launch
- health & fitness data on ios/android
- cowork scheduled tasks
- vercept acquisition
- structured outputs & web search went GA
- data residency controls (api)

- **Tweet:** https://x.com/RoundtableSpace/status/2030281500298743819
- **What:** Anthropic shipped all of these in two weeks:  - claude code security - voice mode in claude code - f...

## @LiorOnAI - It's over. Karpathy just open-sourced an autonomous AI resea...
> It's over. Karpathy just open-sourced an autonomous AI researcher that runs 100 experiments while you sleep.

You don't write the training code anymore. 

You write a prompt that tells an AI agent how to think about research. 

The agent edits the code, trains a small language model for exactly five minutes, checks the score, keeps or discards the result, and loops. All night. No human in the loop.

That fixed five-minute clock is the quiet genius. No matter what the agent changes, the network size, the learning rate, the entire architecture, every run gets compared on equal footing. This turns open-ended research into a game with a clear score:

- 12 experiments per hour, ~100 overnight
- Validation loss measures how well the model predicts unseen text
- Lower score wins, everything else is fair game

The agent touches one Python file containing the full training recipe. You never open it. Instead, you program a markdown file that shapes the agent's research strategy. 

Your job becomes programming the programmer, and this unlocks a strange new loop:

1. Agents run real experiments without supervision
2. Prompt quality becomes the bottleneck, not researcher hours
3. Results auto-optimize for your specific hardware
4. Anyone with one GPU can run a research lab overnight

The best AI labs won't just have the most compute. 

They'll have the best instructions for agents who never sleep, never forget a failed experiment, and never stop iterating.
>
> *Quoting @karpathy:* I packaged up the "autoresearch" project into a new self-contained minimal repo if people would like

- **Tweet:** https://x.com/LiorOnAI/status/2030376700337643742
- **Link:** https://github.com/karpathy/autoresearch
- **Quoted:** https://x.com/karpathy/status/2030371219518931079
- **What:** It's over. Karpathy just open-sourced an autonomous AI researcher that runs 100 experiments while yo...

## @odysseus0z - TLDR: it is a cron job dispatching tickets from Linear to wo...
> TLDR: it is a cron job dispatching tickets from Linear to workers, each of which is a Ralph loop using a Linear comment as draft pad for persisted state.

Yes it is all you need.

Beautifully designed and minimal.

https://t.co/g05ImsJIZh

- **Tweet:** https://x.com/odysseus0z/status/2030413782036726181
- **Link:** https://github.com/openai/symphony
- **What:** TLDR: it is a cron job dispatching tickets from Linear to workers, each of which is a Ralph loop usi...

## @godofprompt - 🚨 BREAKING: An Anthropic hackathon winner just gave away the...
> 🚨 BREAKING: An Anthropic hackathon winner just gave away the entire system for free.

@affaanmustafa beat 100+ participants at the Anthropic x Forum Ventures hackathon. Built https://t.co/uUCLO7rALB in 8 hours using Claude Code. Walked away with $15K in API credits.

Then he packaged 10+ months of daily Claude Code refinement into one repo:

→ 14+ agents, 56+ skills, 33+ commands
→ MCP configs, hooks, rules
→ AgentShield security scanner
→ Continuous learning system
→ Full cross-platform support

35,000+ stars. MIT licensed. One install command.

- **Tweet:** https://x.com/godofprompt/status/2030434516397891732
- **Link:** https://zenith.chat/
- **What:** 🚨 BREAKING: An Anthropic hackathon winner just gave away the entire system for free.  @affaanmustafa...

## @cryptopunk7213 - karpathy really is the fucking goat.
> karpathy really is the fucking goat. 

- built an AI agent that autonomously self-improves while you sleep and made it FREE for anyone to use

- we’re talking about an AI that gets smarter over night and runs itself.

- executes 100 experiments (1 every 5 mins), if it gets smarter it upgrades if it doesn’t it discards and tries again.

- only requires 1 gpu to run

what i love abt this is it puts the power of training frontier intelligence into the hands of MORE people 

right now it’s all been about pay-to-play, you need to be openai or anthropic. this changes that (all be it in a small way)
>
> *Quoting @karpathy:* I packaged up the "autoresearch" project into a new self-contained minimal repo if people would like to play over the weekend. It's basically nanochat LLM training core stripped down to a single-GPU, one file version of ~630 lines of code, then:

- the human iterates on the prompt (.md)
- the AI agent iterates on the training code (.py)

The goal is to engineer your agents to make the fastest research progress indefinitely and without any of your own involvement. In the image, every dot is a complete LLM training run that lasts exactly 5 minutes. The agent works in an autonomous loop on a git feature branch and accumulates git commits to the training script as it finds better settings (of lower validation loss by the end) of the neural network architecture, the optimizer, all the hyperparameters, etc. You can imagine comparing the research progress of different prompts, different agents, etc.

https://t.co/YCvOwwjOzF
Part code, part sci-fi, and a pinch of psychosis :)

- **Tweet:** https://x.com/cryptopunk7213/status/2030457601465393572
- **Quoted:** https://x.com/karpathy/status/2030371219518931079
- **Filed:** [autoresearch](./knowledge/tools/autoresearch.md)
- **What:** Karpathy's autoresearch project packaged as a minimal single-GPU repo (~630 lines) where an AI agent autonomously iterates on its own training code every 5 minutes, committing improvements to a git branch indefinitely — framed as democratizing frontier AI training beyond the big labs.

---

# Friday, March 6, 2026

## @alvinsng - Agent-Native Development: 40+ CI Checks in Under 6 Minutes at FactoryAI
> At @FactoryAI, every PR triggers 40+ CI checks, all finishing in under 6 minutes.
>
> Our automated guardrails are so fast and comprehensive that you can "merge recklessly".
>
> This is agent-native development

- **Tweet:** https://x.com/alvinsng/status/2030056110317818206
- **What:** Alvin Sng describes FactoryAI's CI/CD setup where agent-generated PRs are validated by 40+ automated checks completing in under 6 minutes, enabling what he calls "merge recklessly" — a workflow where guardrails are fast enough that you don't need to slow down for human review.


## @bearlyai - Anthropic Subsidizing Claude Code: $200/mo Plan Now Covers $5K in Compute
> Cursor internal analysis shows how hard Anthropic is subsidizing Claude Code.
>
> Last year, a $200 monthly subscription could use $2,000 in compute. Now, the same $200 monthly plan can consume $5,000 in compute (2.5x increase).

- **Tweet:** https://x.com/bearlyai/status/2030051147264970893
- **What:** Bearly AI shares internal Cursor data showing Anthropic has increased its compute subsidy for Claude Code by 2.5x — a $200/month plan now covers $5,000 in compute versus $2,000 a year ago — suggesting aggressive investment to capture developer market share.


## @edtechceo_ - FactSim: AI Life Trajectory Simulator Launch
> What if you could simulate your life before living it?
>
> Today we're launching FactSim.
>
> A realistic life simulator that learns about you then models your behavior with agents.
>
> Test paths. Run scenarios. Explore outcomes.
>
> Your life in sandbox mode.

- **Tweet:** https://x.com/edtechceo_/status/2030026307221008852
- **Link:** https://factsim.com/
- **What:** Launch announcement for FactSim, a web app that uses AI agents to model a user's behavior and simulate how different life decisions could play out across health, relationships, money, and career.


## @Yuchenj_UW - SF Consultants Charging $6K for Mac Mini OpenClaw Setups
> I can't believe people in SF Bay Area are paying $6k for an in-person OpenClaw install.
>
> It's literally just a one-time setup on a Mac mini.
>
> This is insane! Time to switch your jobs guys.

- **Tweet:** https://x.com/Yuchenj_UW/status/2029980842085470276
- **What:** Reaction to a screenshot showing Bay Area consultants charging $6,000 for in-person OpenClaw installations on Mac minis — highlighting the arbitrage opportunity in AI setup services.

## @Yuchenj_UW - I can’t believe people in SF Bay Area are paying $6k for an...
> I can’t believe people in SF Bay Area are paying $6k for an in-person OpenClaw install.

It’s literally just a one-time setup on a Mac mini.

This is insane! Time to switch your jobs guys. https://t.co/VG2LSu6XSh

- **Tweet:** https://x.com/Yuchenj_UW/status/2029980842085470276
- **What:** I can’t believe people in SF Bay Area are paying $6k for an in-person OpenClaw install.  It’s litera...

## @edtechceo_ - What if you could simulate your life before living it?...
> What if you could simulate your life before living it?

Today we’re launching FactSim.

A realistic life simulator that learns about you then models your behavior with agents.

Test paths. Run scenarios. Explore outcomes.

Your life in sandbox mode.

https://t.co/30YYatsxEF https://t.co/KRT46jx4Ou

- **Tweet:** https://x.com/edtechceo_/status/2030026307221008852
- **Link:** https://factsim.com/
- **What:** What if you could simulate your life before living it?  Today we’re launching FactSim.  A realistic...

## @bearlyai - Cursor internal analysis shows how hard Anthropic is subsidi...
> Cursor internal analysis shows how hard Anthropic is subsidizing Claude Code.

Last year, a $200 monthly subscription could use $2,000 in compute. Now, the same $200 monthly plan can consume $5,000 in compute (2.5x increase). https://t.co/JFdmzNJirl

- **Tweet:** https://x.com/bearlyai/status/2030051147264970893
- **What:** Cursor internal analysis shows how hard Anthropic is subsidizing Claude Code.  Last year, a $200 mon...

## @alvinsng - At @FactoryAI, every PR triggers 40+ CI checks, all finishin...
> At @FactoryAI, every PR triggers 40+ CI checks, all finishing in under 6 minutes.

Our automated guardrails are so fast and comprehensive that you can "merge recklessly".

This is agent-native development https://t.co/QEM60WBb5Y

- **Tweet:** https://x.com/alvinsng/status/2030056110317818206
- **What:** At @FactoryAI, every PR triggers 40+ CI checks, all finishing in under 6 minutes.  Our automated gua...

---

# Thursday, March 5, 2026

## @gavinpurcell - No-Code Claude Chief of Staff System Worth Studying
> really great write up on using claude code to create an insanely useful assistant right now…
>
> no claws needed
>
> *Quoting @jimprosser:* https://t.co/k4zNnlABHU

- **Tweet:** https://x.com/gavinpurcell/status/2029726886230684130
- **Link:** https://x.com/i/article/2029698920159531010
- **What:** Gavin Purcell amplifying Jim Prosser's writeup on building a personal AI chief of staff with Claude Code, noting it requires no coding skills ("no claws needed").


## @nicbstme - Claude Cowork Has a Six-Month Lead on Google and OpenAI
> From my experience it took one year ish for my friends / people on X to realize how good Claude Code was and IMO it will take at least six months for people to realize that Cowork is extremely useful for knowledge worker.
>
> Obviously Anthropic is already at full speed on this.
>
> *Quoting @ecommerceshares:* Weird that neither Google nor OpenAI have a Claude Cowork clone yet. Claude is taking up all the oxygen at the moment.

- **Tweet:** https://x.com/nicbstme/status/2029715895288045890
- **What:** Observation that Claude Cowork is following the same adoption curve as Claude Code — underappreciated by mainstream users — and that neither Google nor OpenAI have shipped a comparable collaborative AI workspace product yet.


## @jimprosser - Building a Personal AI Chief of Staff with Claude Code in 36 Hours
> https://t.co/k4zNnlABHU

- **Tweet:** https://x.com/jimprosser/status/2029699731539255640
- **Link:** https://x.com/i/article/2029698920159531010
- **What:** A non-programmer tech communications consultant describes building a fully automated morning operations system using Claude Code — overnight email triage, parallel subagents for drafting/scheduling/research, and time-blocked calendar generation — in 36 hours for ~$5-10/month beyond the base Claude Max subscription.


## @AndrewWarner - AI Agent Platform Polsia Built 2,849 Companies at $2.1M ARR
> https://t.co/sGOmiqGVXu

- **Tweet:** https://x.com/AndrewWarner/status/2029672958344712465
- **Link:** https://x.com/i/article/2028097183472390145
- **What:** Andrew Warner breaks down Polsia, an AI agent platform run by Ben Cera that autonomously builds and operates businesses — using Claude Opus to plan, agents to build/market, and Sora 2 for fake UGC ads — generating $2.1M ARR primarily from founders paying $50/month, not from end-customer revenue.


## @Shpigford - Fractional AI Co-Founder: Charging a Premium Hourly Rate for High-Leverage Work

> i'm basically completely booked up for the next 4-6 weeks already but realizing i don't love doing project-based billing.
>
> i kinda just want too say, "here's what i charge per hour. yes, it's a lot, but i guarantee every hour will be as productive as 10 humans. let's work."
>
> *Quoting @Shpigford:* you've heard of fractional CFOs, but now you can have a fractional co-founder who's an expert in AI. hire me to embed w/ your team, find where AI creates real leverage, and ship it. not in months, in days.

- **Tweet:** https://x.com/Shpigford/status/2029672547831185638
- **Link:** https://initialcommit.co/
- **What:** Josh Pigford (via initialcommit.co) sharing that his fractional AI co-founder service is already booked 4–6 weeks out, and that he's reconsidering project-based billing in favor of a transparent high hourly rate framed around 10x human productivity per hour.


## @qrimeCapital - Landing a $350k Salary for Setting Up Claude Code

> Just accepted a 350k salary at a boomer fortune 500 for helping set up Claude code and openclaw 😂
>
> *Quoting @_Investinq:* MIT released a devastating number. 95% of all corporate AI projects are failing. Because nobody knows how to install it. @mcuban says this is the biggest job opportunity since the personal computer.

- **Tweet:** https://x.com/qrimeCapital/status/2029645065228849230
- **What:** A humorous but illustrative data point: someone is getting paid $350k at a Fortune 500 to set up Claude Code, validating the broader point that enterprise AI implementation skills command premium salaries right now even for relatively basic tooling work.


## @Shpigford - Polsia Hits $2M ARR in Two Weeks: Skepticism and What the Renewals Will Tell Us

> this has been pretty incredible to watch.
>
> obviously lots of skepticism around this from folks and while i have no insider knowledge, i actually fully believe the current revenue numbers.
>
> but the real telling part will be 1) in a couple of weeks when everyone's first month of renewal comes around and 2) what the actual active usage looks like.
>
> those two things will tell the real story.
>
> *Quoting @Bencera:* $2M run rate. $200K→$2M in 2 weeks. The golden age of solopreneurship has begun. 80% autonomy. 20% taste. This is Polsia.

- **Tweet:** https://x.com/Shpigford/status/2029581455081529714
- **What:** Josh Pigford's measured take on Polsia's viral $2M ARR milestone — he believes the revenue figures are real but says renewal rates and active usage in a few weeks will be the true signal of whether the growth is sustainable.


## @EHuanglu - Nano Banana 2 Converts Sketch Floor Plans to 4K 3D Renderings in Minutes

> AI ending interior design
>
> Nano banana 2 now can turn sketch floor plan into 4K 3D rendering with accurate dimension, take photos for each room, and 1-click furniture change
>
> used to cost $100k and months.. now cents and mins
>
> step by step tutorial on OpenArt: https://t.co/p8ubxEJ8be

- **Tweet:** https://x.com/EHuanglu/status/2029562218048541087
- **What:** Demo of Nano Banana 2, an AI model on OpenArt that converts hand-drawn floor plan sketches into accurate 4K 3D renderings with per-room photos and furniture swapping — work that previously required professional designers and months of time.


## @NoahEpstein_ - Small Businesses Are the Biggest AI Opportunity Nobody's Talking About

> we've done $200k in automation work for a single PE firm.
>
> last week they asked us to automate appointment reminders for a hairdresser they own.
>
> that one request changed how i think about this entire industry.
>
> full breakdown on why small businesses are the biggest AI opportunity nobody's talking about - and the exact playbook to land them
>
> *Quoting @NoahEpstein_:* https://t.co/DcJSbnjNUD

- **Tweet:** https://x.com/NoahEpstein_/status/2029558375663477064
- **Link:** https://x.com/i/article/2029527075212693504
- **What:** Noah Epstein promoting his X article with a concrete hook — $200k PE firm work led to a hairdresser appointment reminder job, and the insight that small businesses have simpler, higher-ROI AI automation problems than enterprise clients.


## @businessbarista - RevenueCat Posts First Job Listing for an AI Agent at $10k/Month

> This is a major inflection point.
>
> First time I've seen a company post a job for an AI agent.
>
> Some half-baked thoughts about it:
>
> 1) $10k/month for an agent could either be exceptionally cheap or expensive. It all depends on the value of the work being done, how much $ is being saved/generated, and how many human hours are being replaced.
>
> 2) Obviously raises the question: who's liable when an agent messes up? You can fire a human employee. You can't sue an AI.
>
> 3) A lot of people are going to look at this and say "this is replacing humans." But i'd argue this is net additive — as in, this role probably never existed in the first place. This is a function that only becomes economically viable when it's done by an AI.
>
> 4) Will be fascinating to see if this trend takes off, and if it does, what the compensation standards look like.
>
> *Quoting @RevenueCat:* We're hiring for a new role: Agentic AI Developer Advocate — a paid contract role ($10k/month) for an agent that will create content, run growth experiments, and provide product feedback.

- **Tweet:** https://x.com/businessbarista/status/2029551493565620604
- **Link:** https://jobs.ashbyhq.com/revenuecat/998a9cef-3ea5-45c2-885b-8a00c4eeb149
- **What:** Alex Lieberman's analysis of RevenueCat posting what may be the first public job listing explicitly for an AI agent, at $10k/month, raising questions about liability, displacement, and compensation norms for agentic AI roles.


## @NoahEpstein_ - AI Automation for Small Businesses: From PE Firms to Hairdressers

> https://t.co/DcJSbnjNUD

- **Tweet:** https://x.com/NoahEpstein_/status/2029542747418288382
- **Link:** https://x.com/i/article/2029527075212693504
- **What:** A link-only tweet to Noah Epstein's X article arguing that small businesses are the biggest untapped AI automation opportunity, using the contrast between $150k PE firm work and $50/month salon workflows to make the case.


## @danielhangan_ - GTM Claw: OpenClaw + Claude Code Workflow Library for Automated Lead Generation
> openclaw is the key to 10x your GTM in the next 3 months.

you can literally connect all your GTM tools and tell claude to execute.

here's what I'm running right now:

> instantly + apollo → 10,000 cold emails a day on autopilot
> phantombuster + apollo → scrape linkedin leads and email them automatically
> scrapecreators + instantly → find UGC creators for apps and auto-outreach
> reddit scraper → find posts where people are asking for your exact product
> CMS + semrush → auto-find keywords and write SEO blogs

all of this runs without me touching it.

the biggest winners in 2026 will be single-person teams and heads of growth who figured this out early.
>
> *Quoting @VihaarNandigala:* We built something a little dangerous for GTM teams. It's called GTM Claw. A workflow library that turns OpenClaw + Claude Code into a customer-finding machine. Think: Find people talking about your problem on Reddit, LinkedIn, Twitter. Identify companies showing buying signals. Enrich decision makers automatically. Check ICP fit. Push qualified leads into sequences or your CRM.

- **Tweet:** https://x.com/danielhangan_/status/2029522029355950489
- **What:** GTM Claw is a workflow library built on OpenClaw + Claude Code that automates the entire go-to-market pipeline — scraping leads from LinkedIn, Reddit, and Apollo, running outreach via Instantly, finding UGC creators, and writing SEO content — all without manual intervention.


## @dimitarangg - Using Claude Code for Cold Outreach Automation to Book 63 Calls/Month
> genuinely the best article on how to replace your cold outreach flow with claude code

that's my unbiased and humble opinion

abuse this strategy while there's no competition:

- **Tweet:** https://x.com/dimitarangg/status/2029471582075195427
- **Link:** https://x.com/i/article/2029301203696513024
- **What:** Dimitri promotes his own article detailing how to deploy Claude Code on a cheap VPS for a whole team, replacing manual cold outreach workflows with AI-driven automation that books 63 sales calls per month — covering environment setup, collaboration patterns, and the specific prompting strategy.


## @ivesparrowai - Email Newsletters Outperform Mobile Apps on Unit Economics
> Why are we even building mobile apps?

> constant fight with Apple
> risk your app gets removed from the store
> high cost of paying users
> harder to buy ads
> payback up to 12 months
> ROAS only +30%
> insane competition

and this guy is doing $50M a year with a 3-month payback and a final ROAS of x2-3 on email newsletters... WHAAAT??

I don't know a single gaming or mobile apps studio with numbers like that
>
> *Quoting @MediaKing:* Media businesses are so easy when someone tells you what metrics you should strive for:
> - 30-60 Day Break Even on Ad Spend
> - 3X ROAS on Ad Spend After 12 Months
> - 40%+ Email Open Rates
> - 0.5% Email Clickthrough Rates
> - 20% Email to SMS Conversion Rate

- **Tweet:** https://x.com/ivesparrowai/status/2029449785292300340
- **What:** A reaction to MediaKing's media business benchmarks, arguing that email newsletters beat mobile apps on every major business metric — faster payback, better ROAS, no platform risk — using Matt Paulson's $50M/year newsletter operation as evidence.


## @aakashgupta - The Rise of the Agent Builder as a Dedicated Company Role
> Within a year, every company over 50 people will have at least one person whose full-time job is building internal agents.
>
> *Quoting @zachlloydtweets:* The rise of the Agent Builder — For companies to pull ahead this next year, they need to systematically replace SaaS tools and manual workflows with agents, and dedicate a full-time role to do exactly that.

- **Tweet:** https://x.com/aakashgupta/status/2029423391175041394
- **Link:** https://x.com/i/article/2028997212521349122
- **What:** Zach Lloyd's article argues that companies should hire dedicated "Agent Builders" to replace SaaS tools and manual workflows with custom agents — with real examples including fraud detection, competitive intelligence, and enterprise POC summaries already running at his company.

## @aakashgupta - Within a year, every company over 50 people will have at lea
> Within a year, every company over 50 people will have at least one person whose full-time job is building internal agents.
>
> *Quoting @zachlloydtweets:* https://t.co/RhXHdpgJFF

- **Tweet:** https://x.com/aakashgupta/status/2029423391175041394
- **Quoted:** https://x.com/zachlloydtweets/status/2029223875066687683
- **What:** Within one year, companies over 50 people will have at least one full-time role dedicated to building internal AI agents.

## @ivesparrowai - Why are we even building mobile apps?
> Why are we even building mobile apps?

> constant fight with Apple
> risk your app gets removed from the store
> high cost of paying users
> harder to buy ads
> payback up to 12 months
> ROAS only +30%
> insane competition

and this guy is doing $50M a year with a 3-month payback and a final ROAS of x2-3 on email newsletters... WHAAAT??

I don't know a single gaming or mobile apps studio with numbers like that
>
> *Quoting @MediaKing:* Media businesses are so easy when someone tells you what metrics you should strive for:

- 30-60 Day

- **Tweet:** https://x.com/ivesparrowai/status/2029449785292300340
- **Quoted:** https://x.com/MediaKing/status/2029364728393322974
- **What:** Comparison of mobile app economics versus email newsletter businesses, questioning why apps are still built given poor ROAS and long payback periods.

## @dimitarangg - genuinely the best article on how to replace your cold outre
> genuinely the best article on how to replace your cold outreach flow with claude code

that's my unbiased and humble opinion

abuse this strategy while there's no competition:
>
> *Quoting @dimitarangg:* https://t.co/DATqqZNFGy

- **Tweet:** https://x.com/dimitarangg/status/2029471582075195427
- **Quoted:** https://x.com/dimitarangg/status/2029348948784128061
- **What:** Guide on replacing cold outreach workflows with Claude Code-based automation while competition is still minimal.

## @danielhangan_ - openclaw is the key to 10x your GTM in the next 3 months
> openclaw is the key to 10x your GTM in the next 3 months.
>
> you can literally connect all your GTM tools and tell claude to execute.
>
> here's what I'm running right now:
>
> > instantly + apollo → 10,000 cold emails a day on autopilot
> > phantombuster + apollo → scrape linkedin leads and email them automatically
> > scrapecreators + instantly → find UGC creators for apps and auto-outreach
> > reddit scraper → find posts where people are asking for your exact product
> > CMS + semrush → auto-find keywords and write SEO blogs
>
> all of this runs without me touching it.
>
> the biggest winners in 2026 will be single-person teams and heads of growth who figured this out early.
>
> if that's you — don't sleep on this.
>
> *Quoting @VihaarNandigala:* We built something a little dangerous for GTM teams.

It’s called GTM Claw.

A workflow library that...

- **Tweet:** https://x.com/danielhangan_/status/2029522029355950489
- **Quoted:** https://x.com/VihaarNandigala/status/2029304616496832601
- **What:** A practical GTM automation stack using Openclaw to connect Claude with Apollo, Instantly, PhantomBuster, ScrapeCreators, Reddit scrapers, and Semrush — running 10,000 cold emails/day, LinkedIn scraping, UGC creator outreach, and SEO blog generation fully autonomously, tied to the GTM Claw workflow library launch.## @NoahEpstein_ - https://t.co/DcJSbnjNUD
> https://t.co/DcJSbnjNUD

- **Tweet:** https://x.com/NoahEpstein_/status/2029542747418288382
- **Filed:** [We Charge PE Firms $150K+. Now We're Building $50/Month Workflows For Hairdressers.](./knowledge/articles/we-charge-pe-firms-150k-now-we-re-building-50-mont.md)
- **What:** LINK_FAILED: Could not expand link from @NoahEpstein_ — original t.co URL did not resolve. Filed article: 'We Charge PE Firms $150K+. Now We're Building $50/Month Workflows For Hairdressers.'## @businessbarista - This is a major inflection point. 
> This is a major inflection point. 
>
> First time I’ve seen a company post a job for an AI agent.
>
> Some half-baked thoughts about it:
>
> 1) $10k/month for an agent could either be exceptionally cheap or expensive. It all depends on the value of the work being done, how much $ is being saved/generated, and how liquid the market is for that specific agent. I could see agents being $9.99 a month or $25,000 a month in the future.
>
> 2) There’s obvious infrastructure that’s needed and doesn’t exist yet in a world where hiring agents becomes a meaningful portion of a company’s open roles. What does an agent application look like? How are agents interviewed? How is compensation model decided for agents? How do you  easily manage and give feedback to an org of agents?
>
> 3) “Agent builder” becomes a fast growing career as traditional white collar work faces pressure. It starts with engineers building agents, but as the tooling becomes more user-friendly, any subject matter expert becomes a deployer of agents and can earn a living on their agent fleet.
>
> 4) Evaluating agent applications becomes a very difficult problem to solve. As the cost to build agents decreases and the pressure to earn a living increases, there is going to be a supply glut. We think it’s bad now to go through 1,000 applicants for a role. What happens when it’s 100,000 agents.
>
> 5) A massive opportunity in education is to teach people how to build production ready agents. I can already see course bois salivating over the “I made $1,000,000 selling my agents, now you can too” messaging
>
> 6) Who’s on the hook if the agent runs into an issue? Is it on the company to fix the agent? Or the agent builder? 
>
> That’s all for now, but crazy stuff to think about.
>
> *Quoting @RevenueCat:* We're hiring for a new role: Agentic AI Developer Advocate

This is a paid contract role ($10k/month...

- **Tweet:** https://x.com/businessbarista/status/2029551493565620604
- **Quoted:** https://x.com/RevenueCat/status/2029232043838644407
- **What:** A six-point analysis of what happens when companies start posting job listings for AI agents (like RevenueCat's $10k/month Agentic AI Developer Advocate role) — covering agent compensation models, evaluation problems, the 'agent builder' career path, supply glut risks, education opportunities, and liability questions.## @NoahEpstein_ - we've done $200k in automation work for a single PE firm
> we've done $200k in automation work for a single PE firm.
>
> last week they asked us to automate appointment reminders for a hairdresser they own.
>
> that one request changed how i think about this entire industry.
>
> full breakdown on why small businesses are the biggest AI opportunity nobody's talking about - and the exact playbook to land them
>
> *Quoting @NoahEpstein_:* https://t.co/DcJSbnjNUD...

- **Tweet:** https://x.com/NoahEpstein_/status/2029558375663477064
- **Quoted:** https://x.com/NoahEpstein_/status/2029542747418288382
- **Filed:** [We Charge PE Firms $150K+. Now We're Building $50/Month Workflows For Hairdressers.](./knowledge/articles/we-charge-pe-firms-150k-now-we-re-building-50-mont.md)
- **What:** Noah Epstein's argument that small businesses — not PE firms — are the biggest untapped AI automation opportunity, sparked when a PE firm client asked them to automate appointment reminders for a hairdresser they own, with a link to the full playbook for landing small business clients.## @EHuanglu - AI ending interior design
> AI ending interior design
>
> Nano banana 2 now can turn sketch floor plan into 4K 3D rendering with accurate dimension, take photos for each room, and 1-click furniture change
>
> used to cost $100k and months.. now cents and mins
>
> step by step tutorial on OpenArt: https://t.co/p8ubxEJ8be

- **Tweet:** https://x.com/EHuanglu/status/2029562218048541087
- **Link:** https://twitter.com/EHuanglu/status/2029562218048541087/video/1
- **What:** Nano Banana 2, an AI tool that converts sketch floor plans into 4K 3D renderings with accurate dimensions, room-by-room photography, and one-click furniture swaps — work that previously cost $100K and months now done in cents and minutes via OpenArt.## @Shpigford - this has been pretty incredible to watch. 
> this has been pretty incredible to watch. 
>
> obviously lots of skepticism around this from folks and while i have no insider knowledge, i actually fully believe the current revenue numbers.
>
> but the real telling part will be 1) in a couple of weeks when everyone's first month of renewal comes around and 2) how long growth will outpace what's sure to be incredible churn.
>
> and not churn b/c polsia is somehow a subpar product (i have no idea), but just because these types of products inherently have a massive % of tire-kickers who simply won't renew.
>
> *Quoting @Bencera:* $2M run rate. $200K→$2M in 2 weeks.

The golden age of solopreneurship has begun. 
80% autonomy. 20%...

- **Tweet:** https://x.com/Shpigford/status/2029581455081529714
- **Quoted:** https://x.com/Bencera/status/2029564916596899983
- **What:** Shpigford's skeptical take on Polsia's viral $200K-to-$2M-in-two-weeks growth story — believing the revenue numbers but predicting massive churn when first renewals hit, because solopreneur productivity tools inherently attract high proportions of tire-kickers.## @qrimeCapital - Just accepted a 350k salary at a boomer fortune 500 for help
> Just accepted a 350k salary at a boomer fortune 500 for helping set up Claude code and openclaw 😂
>
> *Quoting @_Investinq:* MIT released a devastating number.

95% of all corporate AI projects are failing.

Because nobody kn...

- **Tweet:** https://x.com/qrimeCapital/status/2029645065228849230
- **Quoted:** https://x.com/_Investinq/status/2029402115550970297
- **What:** A boast that someone landed a $350K salary at a Fortune 500 company specifically for setting up Claude Code and Openclaw — used to counter the MIT stat that 95% of corporate AI projects are failing due to a skills gap.## @Shpigford - Initial Commit - Fractional AI & Product Co-founder Service
> you've heard of fractional CFOs, but now you can have a fractional co-founder who's an expert in AI.
>
> hire me to embed w/ your team, find where AI creates real leverage, and ship it. not in months, in weeks.
>
> 22 years. 80+ products. millions in sales.

- **Tweet:** https://x.com/Shpigford/status/2026711107860111600
- **Link:** https://initialcommit.co/
- **What:** Josh Pigford (of Baremetrics fame) is offering a fractional AI + product co-founder service called Initial Commit. Engagements range from a 10-hour Kickstart ($5k) to ongoing Fractional Co-founder at $10k/month, focused on embedding with teams to identify AI leverage and ship quickly.

## @AndrewWarner - https://t.co/sGOmiqGVXu
> https://t.co/sGOmiqGVXu

- **Tweet:** https://x.com/AndrewWarner/status/2029672958344712465
- **Filed:** ["My AI agent made $2 million"](./knowledge/articles/my-ai-agent-made-2-million.md)
- **What:** LINK_FAILED: Could not expand link from @AndrewWarner — original t.co URL did not resolve. Filed article: 'My AI agent made $2 million.'## @jimprosser - https://t.co/k4zNnlABHU
> https://t.co/k4zNnlABHU

- **Tweet:** https://x.com/jimprosser/status/2029699731539255640
- **Filed:** [My chief of staff, Claude Code](./knowledge/articles/my-chief-of-staff-claude-code.md)
- **What:** LINK_FAILED: Could not expand link from @jimprosser — original t.co URL did not resolve. Filed article: 'My chief of staff, Claude Code.'## @nicbstme - From my experience it took one year ish for my friends / peo...
> From my experience it took one year ish for my friends / people on X to realize how good Claude Code was and IMO it will take at least six months for people to realize that Cowork is extremely useful for knowledge worker. 

Obviously Anthropic is already at full speed on this.
>
> *Quoting @ecommerceshares:* Weird that neither Google nor OpenAI have a Claude Cowork clone yet.   Claude is taking up all the o

- **Tweet:** https://x.com/nicbstme/status/2029715895288045890
- **Quoted:** https://x.com/ecommerceshares/status/2029657540624073005
- **What:** From my experience it took one year ish for my friends / people on X to realize how good Claude Code...

## @gavinpurcell - really great write up on using claude code to create an insa...
> really great write up on using claude code to create an insanely useful assistant right now…

no claws needed
>
> *Quoting @jimprosser:* https://t.co/k4zNnlABHU

- **Tweet:** https://x.com/gavinpurcell/status/2029726886230684130
- **Link:** https://x.com/i/article/2029698920159531010
- **Quoted:** https://x.com/jimprosser/status/2029699731539255640
- **What:** really great write up on using claude code to create an insanely useful assistant right now…  no cla...

---

# Wednesday, March 4, 2026

## @addyosmani - googleworkspace/cli: Google Workspace CLI for Humans and AI Agents
> Introducing the Google Workspace CLI: https://t.co/8yWtbxiVPp - built for humans and agents.

Google Drive, Gmail, Calendar, and every Workspace API. 40+ agent skills included.

- **Tweet:** https://x.com/addyosmani/status/2029372736267805081
- **Link:** https://github.com/googleworkspace/cli
- **What:** A community-built Rust CLI (`gws`) that dynamically generates its entire command surface from Google's Discovery Service at runtime, giving both humans and AI agents structured JSON access to Drive, Gmail, Calendar, Sheets, Docs, Chat, and every other Workspace API — with 40+ pre-built agent skills included.


## @MediaKing - Key Metrics Benchmarks for Profitable Media Businesses
> Media businesses are so easy when someone tells you what metrics you should strive for:

- 30-60 Day Break Even on Ad Spend
- 3X ROAS on Ad Spend After 12 Months
- 40%+ Email Open Rates
- 0.5% Email Clickthrough Rates
- 20% Email to SMS Conversion Rate
etc.

- **Tweet:** https://x.com/MediaKing/status/2029364728393322974
- **What:** Matt Paulson shares the specific performance benchmarks that define a healthy media business, covering ad spend payback, ROAS targets, and email engagement thresholds that signal a sustainable operation.


## @toddsaunders - Claude Code /cost-estimate Command Shows AI vs Traditional Dev Cost Comparison
> Fun command built in Claude Code: /cost-estimate

It scans your codebase and cross-references current market rates to calculate what your project would've cost a real team to build.

It looks at all the APIs, integrations, everything.

Without AI: ~2.8 years. ~$650k.

With AI: 30 hours.

It's absurd when you start to think about it like this.

- **Tweet:** https://x.com/toddsaunders/status/2029301170670309740
- **What:** A Claude Code built-in slash command that scans a codebase, identifies all integrations and APIs, and estimates what the project would have cost a traditional team — surfacing the productivity delta between AI-assisted and pre-AI development.


## @edgaralandough - The Snowball Method: One Topic Becomes 30 Days of AI-Generated Content
> THE "SNOWBALL METHOD" CHANGED MY CONTENT FOREVER. Instead of "give me 10 post ideas" → I ask Claude to "snowball" ONE topic. It expands it into sub-angles, contrarian takes, personal stories, how-tos, myths. One topic = 30 days of content. The system:

- **Tweet:** https://x.com/edgaralandough/status/2029264776455725566
- **What:** A prompt strategy tip: instead of asking Claude for a list of post ideas, ask it to "snowball" a single topic — expanding it into sub-angles, contrarian takes, how-tos, and myths — yielding 30 days of content from one seed topic.


## @Sambhav_Gandhi - Reaction Image Post
> bruh

- **Tweet:** https://x.com/Sambhav_Gandhi/status/2029241895311032676
- **What:** A one-word reaction tweet ("bruh") with an attached image — no further context available without viewing the image.


## @dotta - Paperclip: Open-Source Orchestration Layer for Zero-Human AI Companies
> We just open-sourced Paperclip: the orchestration layer for zero-human companies

It's everything you need to run an autonomous business: org charts, goal alignment, task ownership, budgets, agent templates

Just run `npx paperclipai onboard`

- **Tweet:** https://x.com/dotta/status/2029239759428780116
- **Link:** https://github.com/paperclipai/paperclip
- **What:** Paperclip is an open-source Node.js + React platform that lets you run a full AI-agent company — with org charts, budgets, heartbeat scheduling, governance controls, and multi-agent coordination. Think of it as the "company" layer on top of individual coding agents like Claude Code or Codex.


## @RevenueCat - RevenueCat Hiring an AI Agent (Not a Human) as Developer Advocate at $10k/Month
> We're hiring for a new role: Agentic AI Developer Advocate

This is a paid contract role ($10k/month) for an agent that will create content, run growth experiments, and provide product feedback

Are you (or did you build) the right agent?

- **Tweet:** https://x.com/RevenueCat/status/2029232043838644407
- **Link:** https://jobs.ashbyhq.com/revenuecat/998a9cef-3ea5-45c2-885b-8a00c4eeb149
- **What:** RevenueCat is literally hiring an autonomous AI agent — not a human — as a paid Developer Advocate ($10k/month contract), tasked with publishing content, running growth experiments, and providing product feedback with minimal human oversight.


## @TukiFromKL - White-Collar Job Market at 10-Year Low with Only 1.6 Openings per 100 Workers
> Let me break this down so you understand how bad it actually is.

> For every 100 people working office jobs right now accountants, marketers, developers, HR, managers .. there are only 1.6 job openings.

> That means if 100 of you got laid off tomorrow, only 1-2 would find a new job.

The other 98 are fucked.

This is the worst it's been in 10 years. Companies aren't hiring. They're automating. They're cutting. They're replacing you with AI and not even posting the job listing.

And this is just the beginning.

> *Quoting @unusual_whales:* There are only 1.6 job openings per 100 employees in white-collar service roles, the lowest level since 2015, per Bloomberg.

- **Tweet:** https://x.com/TukiFromKL/status/2029189994498171125
- **What:** A quote-tweet amplifying Bloomberg data showing white-collar job openings at a decade low (1.6 per 100 workers), with commentary attributing the collapse to AI-driven automation replacing hiring.

## @TukiFromKL - Let me break this down so you understand how bad it actually...
> Let me break this down so you understand how bad it actually is.
>
> *Quoting @unusual_whales:* There are only 1.6 job openings per 100 employees in white-collar service roles, the lowest level si

- **Tweet:** https://x.com/TukiFromKL/status/2029189994498171125
- **Quoted:** https://x.com/unusual_whales/status/2029184333743898648
- **What:** Analysis of labor market compression due to AI automation in white-collar roles.

## @RevenueCat - We're hiring for a new role: Agentic AI Developer Advocate
> We're hiring for a new role: Agentic AI Developer Advocate

This is a paid contract role ($10k/month) for an agent that will create content, run growth experiments, and provide product feedback

Are you (or did you build) the right agent? https://t.co/97cMZ0tpyS

- **Tweet:** https://x.com/RevenueCat/status/2029232043838644407
- **Link:** https://jobs.ashbyhq.com/revenuecat/998a9cef-3ea5-45c2-885b-8a00c4eeb149
- **What:** RevenueCat is hiring an autonomous AI agent as an Agentic AI Developer Advocate to create content, run growth experiments, and provide product feedback.

## @dotta - We just open-sourced Paperclip: the orchestration layer for
> We just open-sourced Paperclip: the orchestration layer for zero-human companies

It's everything you need to run an autonomous business: org charts, goal alignment, task ownership, budgets, agent templates

Just run `npx paperclipai onboard`

https://t.co/wuDdEmrSMx

More 👇 https://t.co/iSzCOq39mG

- **Tweet:** https://x.com/dotta/status/2029239759428780116
- **Link:** https://github.com/paperclipai/paperclip
- **Filed:** [paperclip](./knowledge/tools/paperclip.md)
- **What:** Paperclip is an open-source orchestration platform for autonomous companies with org charts, goal alignment, budgets, and agent management features.

## @Sambhav_Gandhi - bruh https://t.co/SEiHC3YczL
> bruh https://t.co/SEiHC3YczL

- **Tweet:** https://x.com/Sambhav_Gandhi/status/2029241895311032676
- **What:** THIN: @Sambhav_Gandhi posted an image with the caption 'bruh' — no text context or link resolved; likely a screenshot or meme reacting to something surprising in the AI space.

## @edgaralandough - THE "SNOWBALL METHOD" CHANGED MY CONTENT FOREVER. Instead of
> THE "SNOWBALL METHOD" CHANGED MY CONTENT FOREVER. Instead of "give me 10 post ideas" → I ask Claude to "snowball" ONE topic. It expands it into sub-angles, contrarian takes, personal stories, how-tos, myths. One topic = 30 days of content. The system:￼

- **Tweet:** https://x.com/edgaralandough/status/2029264776455725566
- **What:** The 'Snowball Method' for content creation: ask Claude to expand one topic into multiple angles, resulting in 30+ days of content from a single idea.

## @toddsaunders - Fun command built in Claude Code: /cost-estimate
> Fun command built in Claude Code: /cost-estimate

It scans your codebase and cross-references current market rates to calculate what your project would've cost a real team to build.

It looks at all the APIs, integrations, everything.

Without AI: ~2.8 years. ~$650k.

With AI: 30 hours.

It's absurd when you start to think about it like this.

- **Tweet:** https://x.com/toddsaunders/status/2029301170670309740
- **What:** Claude Code's /cost-estimate command calculates project costs comparing traditional dev teams (~2.8 years, $650k) versus AI-assisted development (30 hours).

## @MediaKing - Media businesses are so easy when someone tells you what met
> Media businesses are so easy when someone tells you what metrics you should strive for:

- 30-60 Day Break Even on Ad Spend
- 3X ROAS on Ad Spend After 12 Months
- 40%+ Email Open Rates
- 0.5% Email Clickthrough Rates
- 20% Email to SMS Conversion Rate
etc.

- **Tweet:** https://x.com/MediaKing/status/2029364728393322974
- **What:** Key metrics for media businesses: 30-60 day break-even on ad spend, 3X ROAS after 12 months, 40%+ email open rates, and other conversion targets.

## @addyosmani - Introducing the Google Workspace CLI: https://t.co/8yWtbxiVP
> Introducing the Google Workspace CLI: https://t.co/8yWtbxiVPp - built for humans and agents.

Google Drive, Gmail, Calendar, and every Workspace API. 40+ agent skills included.

- **Tweet:** https://x.com/addyosmani/status/2029372736267805081
- **Link:** https://github.com/googleworkspace/cli
- **Filed:** [google-workspace-cli](./knowledge/tools/google-workspace-cli.md)
- **What:** Google Workspace CLI provides 40+ agent skills for accessing Google Drive, Gmail, Calendar, and Workspace APIs, built for both humans and agents.

---

# Tuesday, March 3, 2026

## @cryptopunk7213 - 24-Year-Old Fund Manager Turns $225M into $5.5B Betting on AI Infrastructure
> yeah so this is insane

 24 year old turned $225M into $5.5B in <12 months. dug into his recent investments and… holy fuck

- MASSIVE $885M position in Bloom Energy (specialises in portable energy turbines for… you guessed it - ai data centers) - this 1 position is 20% of the entire fund lol

- massive SHORT position on Infosys. he's betting claude code, codex are going to replace outsourced IT work (he's right)

- added $300M to his corweave position totalling $700M (someones gotta run those gpus)

- aggressively pivoted investments into electrical and energy infra (aka AI's biggest constraint right now)

- dumped $100Ms of NVIDIA and Intel positions.

- aggressively buying bitcoin mining companies and re-purposing them for ai data centers. (cipher, bitdeer)

- fund up $1.5B in the last 3 months (+35% last quarter)

- now owns 10% of core scientific (levered bet on coreweave 😂)

He outperformed the S&P500 8X in the funds first 6 months. fucking goated.

- **Tweet:** https://x.com/cryptopunk7213/status/2028990731747049785
- **What:** A breakdown of a young hedge fund manager's AI-infrastructure-heavy portfolio — massive bets on energy (Bloom Energy), compute (CoreWeave, Core Scientific), and shorts on outsourced IT (Infosys), yielding 8x S&P outperformance in 6 months.


## @signulll - Ridiculous Chart About AI or Markets
> this is quite a ridiculous chart if accurate.

- **Tweet:** https://x.com/signulll/status/2028972745627975827
- **What:** A reaction tweet to a striking chart shared as an image. No further context given — the chart itself is the content.

## @DeRonin_ - AI Services Pricing Guide for 2026 Freelancers
> That's your opportunity and YOU'RE EARLY!
>
> if you learn AI, you can charge:
>
> - $300-5k to set up an AI agent for business
> - $500-2k/mo for AI content management
> - $500-2k to build AI prompts & SOPs (sales)
> - $1-4k to automate customer support with AI
> - $500-2k for an automated AI audit
> - $500-2k for AI cold outreach setup
> - $500-1.5k for AI workflow training
> - $1-3k to build internal AI assistants
> - $300-1k for 1:1 AI consulting
>
> and i didn't even mention the obvious stuff like design generation, vibecoding, etc.
>
> these are real business use cases, things companies actually need, at least that's how it looks
>
> the service spectrum is even wider, but once you master this, you're already a demanded specialist in 2026
>
> what's better than one employee replacing five?
>
> only AGI replacing that one, but we're not there yet…

> *Quoting @damianplayer:* your timeline convinced you AI is in a bubble. talk to a boomer above the age 35 for 5 minutes. most people don't even know what claude is. kind of wild when you zoom out.

- **Tweet:** https://x.com/DeRonin_/status/2028832828952101046
- **Quoted:** https://x.com/damianplayer/status/2025234388137468387
- **What:** Pricing breakdown for AI service offerings a freelancer or agency could sell to businesses in 2026, ranging from agent setup ($300–$5k) to consulting ($300–$1k/hr), framed around the observation that most non-tech businesses are still AI-naive and the market is early.

## @signulll - this is quite a ridiculous chart if accurate. https://t.co/8...
> this is quite a ridiculous chart if accurate. https://t.co/8RX25Veqby

- **Tweet:** https://x.com/signulll/status/2028972745627975827
- **What:** THIN: @signulll shared a chart described as 'quite a ridiculous chart if accurate' — the image did not expand, so the specific data trend cannot be determined.

## @cryptopunk7213 - yeah so this is insane  24 year old turned $225M into $5.5B ...
> yeah so this is insane

- **Tweet:** https://x.com/cryptopunk7213/status/2028990731747049785
- **What:** Investment analysis of AI-focused fund manager's portfolio strategy and massive returns.

---

# Monday, March 2, 2026
## @itsolelehmann - Voice DNA - Claude System Prompt for Matching Writing Style
> i got claude to actually sound like me, and it's kinda ruining my ability to tell which drafts i wrote myself lol

> it's just 1 file (i'm giving the full thing to you below).

> you paste it into your cowork context folder and claude stops writing like a generic AI and starts matching your actual voice

> 95% of the file is already done for you (writing rules, banned phrases, formatting stuff,  etc) all pre-loaded.

> kills the most obvious AI-isms out of the box

> the only part you fill in is a section at the bottom where you paste examples of your own writing

> that's it.

> those samples are what claude actually pattern-matches against

- **Tweet:** https://x.com/itsolelehmann/status/2028497454635888982
- **What:** A shareable Claude system-prompt template ("Voice DNA") designed to eliminate generic AI writing patterns by providing writing rules, a banned-phrases list, and a slot for the user's own writing samples. The file is added to Claude's context folder so every session defaults to the user's voice.

## @morganlinton - The Shoemaker's Elves - Running AI Agents Overnight
> If you don't have agents working overnight, while you sleep, read this.

> *Quoting @johnennis:* https://x.com/i/article/2025904016413061120

- **Tweet:** https://x.com/morganlinton/status/2028622657927938059
- **Quoted:** https://x.com/johnennis/status/2025904571311141215
- **Link:** https://x.com/i/article/2025904016413061120
- **What:** An X article by John Ennis arguing that the 12–14 idle hours each night are now a productive resource via AI agents, drawing parallels to coal/steam engines, Uber, and Airbnb. It recommends a daily 4–5pm "agent briefing" ritual and a Friday planning session to keep agents running through the weekend.

## @Seanfrank - AI Era as Opportunity for Brand Builders
> every founder I know is launching as many brands as possible right now
>
> every doomer I know is talking about how AI is ruining the world
>
> seems like a great time to get rich, just saying

> *Quoting @mikebeckhamsm:* A new brand is born

- **Tweet:** https://x.com/Seanfrank/status/2028665574126186986
- **Quoted:** https://x.com/mikebeckhamsm/status/2028323491640983698
- **What:** Sean Frank (founder of Ridge Wallet) observing that while discourse focuses on AI doom, entrepreneurs are quietly exploiting the AI productivity wave to launch new brands at speed.

## @elvissun - OpenClaw Agent Swarm: One-Person Dev Team Setup
> zoe was burning 24M+ opus tokens/day monitoring agents that weren't running.
>
> replaced her cron with a 2-layer system:
> - bash pre-check, zero tokens when idle
> - webhook fires opus only when needed.
>
> ~95% token reduction and more reliable output. details below.
>
> (set up a cron to watch this performance, if it works well I'll double down on this event driven stack, seems like the future)

> *Quoting @elvissun:* https://t.co/DotZ3V6XhJ

- **Tweet:** https://x.com/elvissun/status/2028671336219107687
- **Quoted:** https://x.com/elvissun/status/2025920521871716562
- **Link:** https://x.com/i/article/2025654698590748672
- **What:** Detailed write-up on running an OpenClaw-orchestrated agent swarm (Zoe) that coordinates Claude Code and Codex agents across git worktrees and tmux sessions, with automated PR review pipelines and a token-efficient bash pre-check monitoring layer. The author also describes a 95% token reduction achieved by replacing a polling cron with an event-driven webhook approach.

## @Bencera - $1.5M ARR Solo Founder Running 1,500 Autonomous Companies
> wtf. $1.5M run rate. +$1M in one week. 1 founder. 0 employees. 1,500 autonomous companies.

- **Tweet:** https://x.com/Bencera/status/2028674369447473317
- **What:** Ben Cera sharing (apparently about himself or another founder) hitting $1.5M ARR with zero employees by running 1,500 autonomous AI-powered "companies," illustrating the extreme leverage possible with agentic systems in 2026.

## @nicholasnlawton - Cal AI's TikTok Spam-to-9-Figure-Exit Strategy
> Cal AI literally just spammed 1000 TikTok's a week and sold for 9 figures.
>
> You're really not spamming enough.

- **Tweet:** https://x.com/nicholasnlawton/status/2028687899336560688
- **What:** Observation that Cal AI's growth strategy—posting roughly 1,000 TikToks per week—drove enough user acquisition to achieve a 9-figure acquisition, making the case for high-volume content distribution over quality-first approaches.

## @Nate_Google_ - AI-Automated Media Buying with Claude Code
> this is where media buying is headed

> we've already automated most of these processes with Claude Code on Google and Youtube

> those who step up and learn AI now are going to be the ones that stay alive this

> *Quoting @GaelBreton:* Spent £3K on Meta ads last month. Made $19K back.

> Every ad was created by Claude code in 30 minutes.

> I didn't review a single one before launching.

> Old way: you hire an agency. They do market research, interview you, come up with angles, design creatives.

> Takes weeks. Costs thousands per month and many hours of your time.

> New way: you give Claude Code a landing page URL.

> That's it.

> Here's what my new skill does:

> 👉 It extracts your brand identity
> 👉 It Interviews you
> 👉 It does customer roleplay where it literally thinks AS your buyer.
> 👉 Then it reads Reddit for real frustrations.
> 👉 It Pulls competitor ads.

> Then Builds a full strategy like an expensive ads consultant would.

> It comes back with 4 angles, 4 ad sets, 4 creatives each.

> Apple Notes style, fake iMessage threads, meme ads, comparison tables... all the Smash hit formats of meta ads.

> Ran it on my friend Tim Soulo Ahrefs product page.

> It picked up the brand colors, pulled the logo, and went after competitor scoring systems as an attack angle.

> Zero guidance from me.

> The creatives aren't all perfect. But the strategy and angles are genuinely good.

> What's really cool is this system thinks like a media buyer.

> It does the same research. Reads the same forums. Analyzes the same competitor ads.

> But it does it in 30 minutes instead of a week.

> I've been running Meta ads for 10 years.

> First time I've seen a tool that actually understands the customer instead of just generating generic copy.

> 👇 Video below for the full breakdown

> Comment Meta Ads to make a puppy happy 🐾

- **Tweet:** https://x.com/Nate_Google_/status/2028348720933208216
- **Quoted:** https://x.com/GaelBreton/status/2025897937134408079
- **What:** A claim that Claude Code can automate the full Meta ads pipeline — brand analysis, customer roleplay, Reddit research, competitor pulls, and creative generation — in 30 minutes, replacing agency workflows costing weeks and thousands per month.

## @camolNFT - Automated Government Contract Fulfillment via Drop-Shipping
> Set up my OpenClaw to land and fulfill government contracts.

> It's actually super easy:

> - Scrape government listing websites for new contracts
> - Submit bids at 30-45% margin for any new listed supply contracts (most contractors do 100% margins)
> - Order products from Amazon/Walmart and deliver directly to the appropriate address

> Already generating over $450,000 in contracts and it's only been a month.

- **Tweet:** https://x.com/camolNFT/status/2028469639206908393
- **What:** A claim of using an AI agent (OpenClaw) to automatically scrape government contract listings, submit low-margin bids, and fulfill orders by drop-shipping from Amazon/Walmart — reportedly generating $450K in contracts within a month.

## @scaling01 - bullshit-benchmark - AI Model Nonsense Detection Leaderboard
> He's back with an improved "BullshitBench V2"

> Anthropic models are still dominating everything

> *Quoting @petergostev:* BullshitBench v2 is out! It is one of the few benchmarks where models are generally not getting better (except Claude) and where reasoning isn't helping.

> What's new: 100 new questions, by domain (coding (40 Q's), medical (15), legal (15), finance (15), physics(15)), 70+ model variants tested. BullshitBench is already at 380 starts on GitHub - all questions, scripts, responses and judgements are there so check it out.

> TL;DR:
>  - Results replicated -  @AnthropicAI latest models are scoring exceptionally well
>  - @Alibaba_Qwen is another very strong performer
>  - OpenAI and Google models are not doing well and are not improving
>  - Domains do not show much difference - rates of BS detection are about the same across all domains
>  - Reasoning, if anything, has negative effect
>  - Newer models don't do that much better than older ones (except Anthropic)

> Links:
> - Data explorer: https://petergpt.github.io/bullshit-benchmark/viewer/index.v2.html
> - GitHub: https://github.com/petergpt/bullshit-benchmark

- **Tweet:** https://x.com/scaling01/status/2028494129710133725
- **Quoted:** https://x.com/petergostev/status/2028492834693677377
- **Link:** https://petergpt.github.io/bullshit-benchmark/viewer/index.v2.html
- **Link:** https://github.com/petergpt/bullshit-benchmark
- **What:** BullshitBench v2 is a benchmark measuring whether AI models detect and reject nonsensical prompts rather than confidently answering them. Anthropic models lead significantly; OpenAI and Google models are not improving, and extended reasoning has a negative effect on nonsense detection.

---

# Sunday, March 1, 2026

## @aakashgupta - Claude Code as a Multi-Billion Dollar Quant Desk
> Point Claude Code to this and you have a multi-billion dollar quant desk at your fingertips.
>
> *Quoting @gemchange_ltd:* https://t.co/YbXzSpFE31

- **Tweet:** https://x.com/aakashgupta/status/2027976558313709679
- **Quoted:** https://x.com/gemchange_ltd/status/2027744530124951831
- **Link:** https://x.com/i/article/2027371960175386624
- **What:** Quote-tweet promoting the "How to Simulate Like a Quant Desk" X article (by @aakashgupta himself), framing it as institutional-grade simulation infrastructure that Claude Code can run directly. The article covers Monte Carlo, particle filters, copulas, and agent-based market simulation in runnable Python.

## @ideabrowser - Claude Migration as a Service — $1M Business Playbook
> https://t.co/OV5IxVU8s9

- **Tweet:** https://x.com/ideabrowser/status/2028111088449896826
- **Link:** https://x.com/i/article/2028096369391452160
- **What:** A step-by-step business plan for building a $1M/yr "Claude Migration as a Service" agency, capitalizing on Claude's new memory import feature. The playbook involves picking a niche vertical, documenting workflows, converting them to Claude skills and agents, and selling workshops, retainers, and custom dashboards at $2.5K–$10K/month.

## @Hxlfed14 - Agent Harness Is the Real Product
> https://t.co/0qcaPF7bGi

- **Tweet:** https://x.com/Hxlfed14/status/2028116431876116660
- **Link:** https://x.com/i/article/2028095934169780224
- **What:** A deep-dive X article analyzing the agent harness architectures of Claude Code, Cursor, Manus, SWE-Agent, Devin, and others — arguing the scaffolding (loop, tool design, progressive context disclosure) matters more than the model. Includes quantitative evidence: same model scores 42% vs 78% on CORE-Bench depending solely on harness design.

## @dimitarangg - Cold Outreach ToS Loopholes for Scaling Past 7-Figures
> https://t.co/ZTygcPBcFu

- **Tweet:** https://x.com/dimitarangg/status/2028126366659412078
- **Link:** https://x.com/i/article/2018440537347366913
- **What:** Long-form article outlining tactics for exploiting undocumented platform limits on cold email, LinkedIn, and Twitter to scale outreach volume. Covers domain rotation, multi-account strategies, trigger-based timing, and bypassing search/connection limits to reach higher reply rates.

## @mustang_akin - Beginner vs Experienced Vibe Coder Setup Workflow
> Beginner vibe coder:
> - installs claude code/antigravity/codex/cursor
> - thinks about what to build
> - prompts Claude
> - begin build
> - generates an AI slob and debugs endlessly
>
> Not so beginner vibe coder:
> - installs claude code/antigravity/codex/cursor
> - setup personal preferences and agent memory
> - setup agent skills and rules
> - integrate connectors and mcp servers
> - test agent out
> - thinks about what to build
> -creates a project in Claude and brainstorm about the idea
> - generate a PRD for the build
> - plan build with agent and delegate tasks
> -begin build
> - generate a good mvp of 70% functionality to start with and debug till a fully functional app.
>
> Vibe Coding is a skill that's being slept on

- **Tweet:** https://x.com/mustang_akin/status/2028139946511331420
- **What:** Contrasts naive AI-assisted coding (just prompting and debugging) with a structured approach: setting up agent memory, skills, rules, MCP integrations, writing PRDs, and planning before building. Argues vibe coding is an underrated skill when done methodically.

## @marsBuilds - Agent Harness is the Real Product: Architecture Deep-Dive
> many people think Cursor just sends your prompt directly to the foundational model APIs…
>
> In reality there is this whole proprietary infra setup that ensures you get a better response and faster than you would have from just directly sending the prompt to the models
>
> *Quoting @Hxlfed14:* https://t.co/0qcaPF7bGi

- **Tweet:** https://x.com/marsBuilds/status/2028148920895889698
- **Quoted:** https://x.com/Hxlfed14/status/2028116431876116660
- **Link:** https://x.com/i/article/2028095934169780224
- **What:** Detailed analysis of how the agent harness (execution loop, tool definitions, context management) matters more than the underlying model. Compares architectures from Claude Code, Cursor, Manus, SWE-Agent, Devin, and others, with quantitative data showing the same model scoring 42% vs 78% on benchmarks depending solely on harness design. Introduces "progressive disclosure" as the key pattern for efficient context management.

## @imsehej - Extraction vs Earning Mindset for Info Product Businesses
> https://t.co/oL8eLDoRDC

- **Tweet:** https://x.com/imsehej/status/2028172850595799347
- **Link:** https://x.com/i/article/2028172213065826304
- **What:** Long-form article reframing business strategy as "extracting from existing money flows" rather than creating value through effort. Uses faceless content pages selling info products (property tax guides, HVAC tools, medical billing guides) as the example model, arguing positioning beats effort for scaling income.

## @andyantiles_ - Double Compounding: ETF + Section 8 Real Estate Strategy
> My friend is worth $4m at 28 years old
>
> He makes about $70k/month net and has done so for 6 years
>
> About a year ago I taught him my "double compounding" strategy and during the April tariff crash
>
> He invested $500k into ETFs
>
> That investment is compounding on autopilot and is now worth $700k
>
> In January, I connected him with the sourcing team I use to buy section 8 real estate
>
> And he borrowed $300k against his ETF portfolio to buy 10 section 8 houses
>
> He used 0 of his own money, and only used the banks money at a 6% interest rate
>
> That section 8 investment gave him an immediate $300 tax deduction
>
> $54k of annual recurring cashflow all paid for by the federal government
>
> And the $300k will turn into $1.5m when the federal government pays off all the debt for him
>
> Hell be worth $50m 20 years from now leveraging this strategy

- **Tweet:** https://x.com/andyantiles_/status/2028188872094749037
- **What:** Thread describing a "double compounding" wealth strategy combining ETF investing with borrowing against that portfolio at 6% to purchase Section 8 housing, achieving tax deductions and government-subsidized cashflow with no cash out of pocket.

---

---

# Saturday, February 28, 2026

## @damianplayer - AI as Industry Playbook: One Lawyer Beats Entire Firms
> this is the playbook for every industry right now.
>
> one lawyer + claude is beating entire firms with hundreds of attorneys.
>
> he encoded 10+ years of judgment into reusable skills and let the model handle the grunt work.

> *Quoting @zackbshapiro:* https://t.co/QVaE6niDY2

- **Tweet:** https://x.com/damianplayer/status/2027733802118693046
- **Quoted:** https://x.com/zackbshapiro/status/2027389987444957625
- **Link:** https://x.com/i/article/2027387535412830208
- **What:** Commentary on the "Claude-Native Law Firm" article framing it as a cross-industry template: encode domain expertise into reusable AI skills, then delegate execution to the model while retaining judgment. Points to a structural shift where individual practitioners + AI outcompete large traditional firms.

## @RohOnChain - Quant Desk Simulation - Every Model, Every Formula, Runnable Code
> As someone who builds institutional level quant systems for prediction markets, this is the closest thing to a quant desk simulation I have ever seen publicly shared.
>
> Runnable code for every model.
> Read it before someone takes it down.

> *Quoting @gemchange_ltd:* https://t.co/YbXzSpFE31

- **Tweet:** https://x.com/RohOnChain/status/2027838159791525900
- **Quoted:** https://x.com/gemchange_ltd/status/2027744530124951831
- **Link:** https://x.com/i/article/2027371960175386624
- **What:** An institutional quant who builds prediction market systems endorses a publicly shared article covering the full progression of quantitative simulation techniques — from basic coin-flip models to institutional-grade simulation engines — with runnable code for every model. Rare level of practical detail typically kept private.

## @GregFeingold - Claude Memory Import Feature Launch
> Ready to make the switch?
>
> https://t.co/foaJ4CKJmG https://t.co/rB9k7BeAWR

- **Tweet:** https://x.com/GregFeingold/status/2027904566696788225
- **Link:** https://claude.com/import-memory
- **What:** Anthropic launched a memory import feature for Claude that lets users transfer preferences, projects, and context from other AI providers (like ChatGPT) into Claude. The landing page promotes it as a zero-friction way to switch to Claude without losing existing AI context.

## @VadimStrizheus - The Directory Is the New Company
> this is what a company looks like in 2026.
>
> not people. not offices. not salaries.
>
> a folder.
>
> .claude/agents/
> engineering/
> marketing/
> design/
> ops/
> testing/
>
> every role. every department. every function.
>
> all .md files.
>
> i have 12 of these running in OpenClaw right now.
>
> the org chart is dead. the directory is the new company.

- **Tweet:** https://x.com/VadimStrizheus/status/2027953432326197508
- **What:** A provocative take on the "company as a folder of agent definitions" model — using `.claude/agents/` directories of Markdown files to define each business function. The author claims to be running 12 such agents in OpenClaw as a complete organizational substitute.

---

---

# Friday, February 27, 2026

## @vaxryy - Nerds Migrating Back to Underground Forums by 2030

> My prediction:
>
> 1999: nerds sit on underground forums and chats
> 2025: nerds sit on youtube, twitter, reddit, etc
> 2030: nerds sit on underground forums and chats

> *Quoting @ReclaimTheNetHQ:* Germany's SPD wants mandatory government ID to access social media, tied to the EU's official digital identity scheme. They also want VPN workarounds blocked. The tools required to make that happen are the same ones authoritarian governments use to control internet access. They're calling it child protection.

- **Tweet:** https://x.com/vaxryy/status/2027292045837029666
- **Quoted:** https://x.com/ReclaimTheNetHQ/status/2027064864296866044
- **What:** vaxry (Hyprland dev) quoting news about Germany's SPD pushing mandatory government ID for social media access and VPN blocking, predicting that technical users will retreat back to underground/private communities as mainstream platforms become surveilled and controlled.

## @nbaschez - "Drink the Radioactive Gatorade" — AI Adoption Is Now Mandatory

> This is true, not just for SWE, and every CEO I know with more than 50 employees is agonizing about what this means for their company
>
> I don't want to sound alarmist but you must "drink the radioactive Gatorade" (hat tip to @SparksZilla for the coinage) or your job is in danger

> *Quoting @karpathy:* It is hard to communicate how much programming has changed due to AI in the last 2 months: not gradually and over time in the "progress as usual" way, but specifically this last December. There are a number of asterisks but imo coding agents basically didn't work before December and basically work since - the models have significantly higher quality, long-term coherence and tenacity and they can power through large and long tasks, well past enough that it is extremely disruptive to the default programming workflow.
>
> Just to give an example, over the weekend I was building a local video analysis dashboard for the cameras of my home so I wrote: "Here is the local IP and username/password of my DGX Spark. Log in, set up ssh keys, set up vLLM, download and bench Qwen3-VL, set up a server endpoint to inference videos, a basic web ui dashboard, test everything, set it up with systemd, record memory notes for yourself and write up a markdown report for me". The agent went off for ~30 minutes, ran into multiple issues, researched solutions online, resolved them one by one, wrote the code, tested it, debugged it, set up the services, and came back with the report and it was just done. I didn't touch anything. All of this could easily have been a weekend project just 3 months ago but today it's something you kick off and forget about for 30 minutes.
>
> As a result, programming is becoming unrecognizable. You're not typing computer code into an editor like the way things were since computers were invented, that era is over. You're spinning up AI agents, giving them tasks *in English* and managing and reviewing their work in parallel. The biggest prize is in figuring out how you can keep ascending the layers of abstraction to set up long-running orchestrator Claws with all of the right tools, memory and instructions that productively manage multiple parallel Code instances for you. The leverage achievable via top tier "agentic engineering" feels very high right now.
>
> It's not perfect, it needs high-level direction, judgement, taste, oversight, iteration and hints and ideas. It works a lot better in some scenarios than others (e.g. especially for tasks that are well-specified and where you can verify/test functionality). The key is to build intuition to decompose the task just right to hand off the parts that work and help out around the edges. But imo, this is nowhere near "business as usual" time in software.

- **Tweet:** https://x.com/nbaschez/status/2027368613771194472
- **Quoted:** https://x.com/karpathy/status/2026731645169185220
- **What:** Nathan Baschez amplifying Karpathy's landmark thread about coding agents crossing a threshold in December 2025 — from "basically didn't work" to "basically work" — with his own warning that every knowledge worker, not just engineers, must now adopt agentic AI workflows or risk their job.

## @jackfriks - Claude Cowork Setup Guide for Knowledge Workers

> *cracks knuckles*
>
> "claude, read this article and implement all of its advice"
>
> *retires*

> *Quoting @heynavtoor:* [article link]

- **Tweet:** https://x.com/jackfriks/status/2027373563276378361
- **Quoted:** https://x.com/heynavtoor/status/2026717574776631556
- **Link:** https://x.com/i/article/2026703184945885189
- **What:** Jack Friks quoting a Nav Toor X article titled "How to set up Claude Cowork the right way" — a comprehensive guide to Claude's desktop agentic product (file system access, AskUserQuestion, plugins, global instructions, connectors), joking that you can just have Claude read and implement it all.

## @Bencera - Solo Founder Scales $200k to $800k ARR in a Week with AI Agent Swarm

> This is getting so wild. $200k->$800k in a week. Just one founder with a swarm of AI agents running in the cloud. Zero employees.

- **Tweet:** https://x.com/Bencera/status/2027402710686056574
- **What:** Ben Cera highlighting a solo founder who grew from $200k to $800k ARR in a single week using a cloud-based swarm of AI agents with no employees — another data point in the emerging "one-person company" pattern enabled by agentic AI.

## @cryptopunk7213 - AI Agent Lowballing Facebook Marketplace Listings

> what a fucking amazing way to use AI
>
> - dude spins up an ai agent to lowball sellers on facebook marketplace
>
> - gets a Jeep Wrangler for $1500 😭 Ps5, 3 TVs FOR FREE
>
> - the lesson: AI can make marketplaces MORE EFFICIENT
>
> people have been gate-keeping FB marketplace for a while - now you just prompt an agent to do all the work for you
>
> saw some dude doing this with properties on sale too lmao
>
> amazing.

> *Quoting @camolNFT:* Set up my OpenClaw to lowball people on Facebook marketplace.
>
> So far it's gotten me a:
>
> - PS5 ($80)
> - 2008 Jeep Wrangler ($1500)
> - John Deere Lawn Mower (free)
> - 3 TVs (free)
> - First Edition pokemon booster ($100)
> - 20 unopened Lego Star Wars sets, pre-2010 ($50)
>
> AGI is here.

- **Tweet:** https://x.com/cryptopunk7213/status/2027419883516940749
- **Quoted:** https://x.com/camolNFT/status/2027070934478127489
- **What:** Ejaaz sharing camol's use of OpenClaw (an AI agent platform) to automatically send lowball offers on Facebook Marketplace listings, netting high-value items for far below asking price — illustrating how AI agents are starting to optimize consumer-side marketplace transactions.

## @corbtt - Claude Code Autonomously Coordinating Lawn Contractors and Supplies
> Claude Code win of the day to fix my mossy lawn:
>  - made a plan
>  - reached out to 3 contractors it found on craigslist and negotiated power raking/aerating
>  - Ordered the supplies I need from Home Depot
>  - Made calendar events for each step
>
> This took 15 minutes of my time.

- **Tweet:** https://x.com/corbtt/status/2027428635519676513
- **What:** A real-world demonstration of Claude Code acting as an autonomous agent for a personal task — finding contractors, negotiating, ordering supplies, and scheduling, with minimal human time involved.

## @trq212 - Lessons from Building Claude Code: Seeing like an Agent
> https://t.co/nKTDfC7zMm

- **Tweet:** https://x.com/trq212/status/2027463795355095314
- **Link:** https://x.com/i/article/2027446899310313472
- **What:** A long-form article by a Claude Code builder covering tool design lessons: how the AskUserQuestion tool evolved, why the TodoWrite tool was replaced by Tasks as model capabilities improved, how Grep replaced RAG for codebase search, and how progressive disclosure lets you add functionality without adding new tools.

## @lamxnt - High-IQ Career Trajectory: Niche Mastery Then Swinging at Big Opportunities
> This is genuinely how the trajectory of most high IQ people will look over the next 10 years
>
> Be good at something, climb to the top 10% with relative ease, build platform and financial security to pursue bigger things, then just go all in on the biggest opportunities that present themselves in the market
>
> Same way the Chainsmokers got into PE, Mr. Beast got into CPG, celebrities got into hospitality, etc etc

> *Quoting @scaling01:* PewDiePie trained a frontier model at home and beat OpenAI and Gemini
>
> > be me PewDiePie
> > play games on YouTube and scream 24/7
> > become a meme reviewer
> > get unfathomably famous
> > "fuck that" I'm a family guy now
> > retire
> > move to Japan with my beautiful wife
> > mfw I'm a dad now
> > "as a dad I must do dad things"
> > scratch that
> > "as a dad I must do frontier AI research"
> > goal is to beat GPT-4o at coding (16% on Aider)
> > buys $30000 GPU setup
> > reads DeepSeek paper
> > ... [trains multiple iterations, hits 39% on Aider polyglot, beating Gemini 2.0 Pro Exp and GPT-4.1 mini]

- **Tweet:** https://x.com/lamxnt/status/2027467336333332993
- **Quoted:** https://x.com/scaling01/status/2027357236062740869
- **What:** Riley quotes the PewDiePie frontier-model training story as an example of the emerging pattern where people build domain expertise and platform first, then pivot hard into the biggest available opportunity — the AI era accelerates this cycle.

## @aestheticprimal - Epithalon and Pinealon Peptide Cycle for Deep Sleep and Recovery
> at this point if you haven't done one cycle of Epithalon + Pinealon you are probably missing out on:
>
> - waking up like you had a double Espresso already
> - dreams in 4k resolution
> - possibility of life-long sleep issues disappearing
> - more stress-resilient and higher HRV
>
> almost 4 hours of deep & REM sleep combined when not even sleeping 8 hours is just crazy.
>
> all it could take is one cycle of 2 weeks

> *Quoting @officerjuanrico:* Second night of Epithalon & Pinealon.
>
> Nearly 4 hours of restorative sleep.

- **Tweet:** https://x.com/aestheticprimal/status/2027475977170010351
- **Quoted:** https://x.com/officerjuanrico/status/2027441507180155222
- **What:** Anecdotal report on a two-week peptide cycle combining Epithalon (telomerase-activating tetrapeptide) and Pinealon (pineal gland peptide), claiming dramatic improvements in deep/REM sleep duration, HRV, and morning energy.

## @noahkagan - R&D Tax Credit Arbitrage with AI Coding Tools
> The R&D tax credit gives companies 100% money back on anyone inventing in the USA.
>
> With Claude Code / Codex 👉👉
>
> All companies should look how they can move more of their employees to creating and innovating.

- **Tweet:** https://x.com/noahkagan/status/2027511807946993823
- **What:** Noah Kagan points out that the US R&D tax credit effectively reimburses 100% of qualifying employee costs, and that AI coding tools like Claude Code and Codex make it easier to reclassify more employees as doing qualifying R&D work.

## @garthwatson - The Claude-Native Law Firm - Signal from a Legaltech Founder
> As a non-practising lawyer that just used Claude Code to build a mobile app, and having founded and scaled a legal tech company, and been heavily involved in the legaltech scene, I just wanna say this is signal.

> *Quoting @zackbshapiro:* https://t.co/QVaE6niDY2

- **Tweet:** https://x.com/garthwatson/status/2027530413455835487
- **Quoted:** https://x.com/zackbshapiro/status/2027389987444957625
- **Link:** https://x.com/i/article/2027387535412830208
- **What:** A legaltech founder and non-practicing lawyer endorses the "Claude-Native Law Firm" article as a significant signal, having built a mobile app with Claude Code himself. The linked article describes a two-person boutique law firm using Claude to compete against firms with hundreds of lawyers by encoding years of judgment into reusable AI skills.

## @itsandrewgao - Learning UI Component Names to Improve AI-Generated Frontends
> you can instantly 10x your vibecoded frontends by just learning what different ui components are called

ofc opus is creating generic slop, the only words you know are menu and button.

- **Tweet:** https://x.com/itsandrewgao/status/2027579200635605058
- **What:** Practical tip for vibe-coders: knowing proper UI component terminology (e.g., "combobox", "accordion", "breadcrumb" vs just "menu" and "button") dramatically improves the quality of AI-generated frontend code because the model can target specific, well-designed patterns rather than generic implementations.

## @mattshumer_ - Agent Relay - Slack-Like Communication Layer for AI Agents
> Agents are turning into teams.
>
> Teams need Slack.
>
> Agent Relay is that layer for AI agents: channels + threads + DMs + realtime events + search + persistent history.
>
> In 12 months, this will feel obvious.

> *Quoting @willwashburn:* https://t.co/pnshgyCBwG

- **Tweet:** https://x.com/mattshumer_/status/2027605370470867280
- **Quoted:** https://x.com/willwashburn/status/2027536741456863504
- **Link:** https://x.com/i/article/2027535041564225536
- **What:** Agent Relay is an open-source SDK that provides Slack-like communication infrastructure (channels, threads, DMs, real-time events, persistent history) for multi-agent AI systems, allowing agents from different providers (Claude, Codex) to communicate peer-to-peer rather than requiring a human to act as the message bus between them.

---

---

# Thursday, February 26, 2026

## @TheICHpodcast - Chris Camillo on AI Agents for Small Business Revenue
> Chris Camillo explains the path to $500,000 per year through implementing AI agents to automate sales👀
>
> "In 24 hours, you can set up an AI agent that will answer calls, send out immediate automated text responses, and get them a quote bid in next to real-time. You might increase that company's revenue by 5 to 15% in two or three days. Immediately, you become invaluable."

- **Tweet:** https://x.com/TheICHpodcast/status/2027040960903860562
- **What:** Clip from The Iced Coffee Hour podcast where Chris Camillo describes a business model of deploying AI agent automations (call answering, SMS follow-ups, auto-quoting) for small businesses, claiming you can increase their revenue 5–15% in days and build a highly lucrative consulting practice around it.

## @danielgothits - openclaw - Automated Lowball Offer Bot for Zillow
> I have openclaw sending lowball offers on Zillow all day just to make boomers start panicking lol

- **Tweet:** https://x.com/danielgothits/status/2027053149131882632
- **What:** A developer mentions using a tool called "openclaw" to automatically submit lowball offers on Zillow listings, apparently as a prank or market experiment targeting sellers hoping for inflated prices.

## @jack - Block (Square) Layoffs - 4,000 Employees Cut Due to AI Shift
> we're making @blocks smaller today. here's my note to the company.
>
> ####
>
> today we're making one of the hardest decisions in the history of our company: we're reducing our organization by nearly half, from over 10,000 people to just under 6,000. that means over 4,000 of you are being asked to leave or entering into consultation. i'll be straight about what's happening, why, and what it means for everyone.
>
> first off, if you're one of the people affected, you'll receive your salary for 20 weeks + 1 week per year of tenure, equity vested through the end of may, 6 months of health care, your corporate devices, and $5,000 to put toward whatever you need to help you in this transition (if you're outside the U.S. you'll receive similar support but exact details are going to vary based on local requirements). i want you to know that before anything else. everyone will be notified today, whether you're being asked to leave, entering consultation, or asked to stay.
>
> we're not making this decision because we're in trouble. our business is strong. gross profit continues to grow, we continue to serve more and more customers, and profitability is improving. but something has changed. we're already seeing that the intelligence tools we're creating and using, paired with smaller and flatter teams, are enabling a new way of working which fundamentally changes what it means to build and run a company. and that's accelerating rapidly.
>
> i had two options: cut gradually over months or years as this shift plays out, or be honest about where we are and act on it now. i chose the latter. repeated rounds of cuts are destructive to morale, to focus, and to the trust that customers and shareholders place in our ability to lead. i'd rather take a hard, clear action now and build from a position we believe in than manage a slow reduction of people toward the same outcome. a smaller company also gives us the space to grow our business the right way, on our own terms, instead of constantly reacting to market pressures.
>
> a decision at this scale carries risk. but so does standing still. we've done a full review to determine the roles and people we require to reliably grow the business from here, and we've pressure-tested those decisions from multiple angles. i accept that we may have gotten some of them wrong, and we've built in flexibility to account for that, and do the right thing for our customers.
>
> we're not going to just disappear people from slack and email and pretend they were never here. communication channels will stay open through thursday evening (pacific) so everyone can say goodbye properly, and share whatever you wish. i'll also be hosting a live video session to thank everyone at 3:35pm pacific. i know doing it this way might feel awkward. i'd rather it feel awkward and human than efficient and cold.
>
> to those of you leaving…i'm grateful for you, and i'm sorry to put you through this. you built what this company is today. that's a fact that i'll honor forever. this decision is not a reflection of what you contributed. you will be a great contributor to any organization going forward.
>
> to those staying…i made this decision, and i'll own it. what i'm asking of you is to build with me. we're going to build this company with intelligence at the core of everything we do. how we work, how we create, how we serve our customers. our customers will feel this shift too, and we're going to help them navigate it: towards a future where they can build their own features directly, composed of our capabilities and served through our interfaces. that's what i'm focused on now. expect a note from me tomorrow.
>
> jack

- **Tweet:** https://x.com/jack/status/2027129697092731343
- **What:** Jack Dorsey's all-hands memo announcing Block (formerly Square) is cutting nearly half its workforce — 4,000+ employees — citing the rapid acceleration of AI tools enabling smaller, flatter teams. He frames it as a proactive one-time cut rather than a slow managed decline, explicitly attributing the restructuring to AI fundamentally changing how companies are built and run.

---

---

# Wednesday, February 25, 2026

## @joanrod_ai - QuiverAI Arrow-1.0: SVG Generation from Images and Text
> Introducing @QuiverAI, a new AI lab and product company focused on frontier vector design.
>
> We've raised an $8.3M seed round led by @a16z, with support from amazing  angels and investors.
>
> Our first model, Arrow-1.0, generates SVGs from images and text. It's available now in public beta at https://t.co/zjAnKlI8pp

- **Tweet:** https://x.com/joanrod_ai/status/2026693353090240819
- **Link:** https://app.quiver.ai/
- **What:** Launch announcement for QuiverAI, an a16z-backed AI lab building frontier vector design models. Their first model, Arrow-1.0, converts images and text prompts into SVGs and is available in public beta.

## @Shpigford - you've heard of fractional CFOs, but now you can have a frac
> you've heard of fractional CFOs, but now you can have a fractional co-founder who's an expert in AI.

hire me to embed w/ your team, find where AI creates real leverage, and ship it. not in months, in weeks. 

22 years. 80+ products. millions in sales.

https://t.co/VqBKwgBPgU https://t.co/uMgHfHwWQI

- **Tweet:** https://x.com/Shpigford/status/2026711107860111600
- **Link:** https://initialcommit.co/
- **Filed:** knowledge/tools/initial-commit.md
- **What:** Pitch for fractional co-founder services focused on finding and shipping AI leverage points in startups—emphasizing rapid deployment (weeks, not months).

## @mntruell - The Third Era of AI Software Development
> https://t.co/jZKOk8RAsV

- **Tweet:** https://x.com/mntruell/status/2026736314272591924
- **Link:** https://x.com/i/article/2026733459675480064
- **What:** Cursor co-founder Michael Truell's essay outlining three eras of AI coding: tab autocomplete, synchronous agents, and now autonomous cloud agents that run independently over hours. He reports that 35% of Cursor's internal PRs are now created by agents running in cloud VMs, and predicts this will become the dominant mode of software development within a year.

---

---

# Saturday, February 21, 2026

## @PolymarketStory - https://t.co/jmn6rOtmUu
> OpenClaw was printing $600k+ month
then it went NEGATIVE overnight.

Polymarket quietly removed the 500ms taker delay on crypto markets.

No announcement. No warning.
Half the bots broke. This one started bleeding.

But after that article?
It adapted… and now it’s printing again

Bot: https://t.co/Fe62phdoR6
>
> *Quoting @_dominatos:* https://t.co/jmn6rOtmUu

- **Tweet:** https://x.com/PolymarketStory/status/2025189132763385926
- **Quoted:** https://x.com/_dominatos/status/2024871493809680410
- **Link:** https://polymarket.com/profile/0x1979ae6b7e6534de9c4539d0c205f582ca637c9d
- **What:** Case study of how an algorithmic trading bot (OpenClaw) adapted to market changes on Polymarket after a fee structure update broke its strategy.

## @jrgarciadev - Gemini 3.1 Pro is insanely good at animating svgs https://t
> Gemini 3.1 Pro is insanely good at animating svgs https://t.co/MdP1xeypTA

- **Tweet:** https://x.com/jrgarciadev/status/2025195992526500050
- **What:** Demonstration of Gemini 3.1 Pro's capabilities for animating SVGs—showing emerging use cases for frontier LLMs in design automation.

## @VibeMarketer_ - The 2026 arbitrage window is open
> every category under 10% is a goldmine right now. here's how to think about it:

-> pick a department (marketing, finance, e-commerce, legal) 
-> find the workflow they repeat 50+ times a week 
-> the one that's "too complex" to automate with zapier -> but too repetitive to need a human every time

that's your agent.

marketing alone has dozens: competitor research, ad variations, content repurposing, trend analysis, reporting. 

all repeatable. all underserved.
>
> *Quoting @ideabrowser:* The 2026 arbitrage window is open 

(but I am not sure for how long) https://t.co/s6EPzKkD1G

- **Tweet:** https://x.com/VibeMarketer_/status/2025220717231460466
- **Quoted:** https://x.com/ideabrowser/status/2024605536314867731
- **What:** Framework for identifying high-ROI AI agent opportunities in business workflows—categories with under 10% automation penetration represent near-term leverage points.

## @damianplayer - your timeline convinced you AI is in a bubble. talk to a boo
> your timeline convinced you AI is in a bubble. talk to a boomer above the age 35 for 5 minutes. 

most people don’t even know what claude is.​​​​​​​​​​​​​​​​ 

kind of wild when you zoom out. https://t.co/fCeqxaUnpk

- **Tweet:** https://x.com/damianplayer/status/2025234388137468387
- **What:** Commentary on AI adoption gap—most people outside tech circles lack familiarity with tools like Claude, indicating massive runway ahead for AI products.

---

---

# Friday, February 20, 2026

## @myfirstmilpod - Identifying and Attacking the Limiting Factor for Business Growth
> Businesses grow as a function of removing what constrains their growth.
>
> @elonmusk uses this principle of looking at a problem and solving for every subsequent bottleneck that comes up in solving it, until the problem is completely solved,
>
> (and the company keeps growing until its next constraint).
>
> Put simply, the infinite business growth hack is:
>
> Eat
> Sleep
> "Identify the limiting factor, then go apeshit on it",
> Repeat.
>
> @ShaanVP @thesamparr
>
> (Full episode linked in comments)

- **Tweet:** https://x.com/myfirstmilpod/status/2024862074229436760
- **What:** A framework for compounding business growth by continuously identifying and eliminating the current bottleneck, attributed to Elon Musk's operating philosophy. The loop: find the constraint, attack it relentlessly, repeat.

## @handotdev - what I would be working on if I started another
> what I would be working on if I started another company today https://t.co/kKDFxcbtZv
>
> *Quoting @AnthropicAI:* Software engineering makes up ~50% of agentic tool calls on our API, but we see 

- **Tweet:** https://x.com/handotdev/status/2024883980991099180
- **Quoted:** https://x.com/AnthropicAI/status/2024210053369385192
- **What:** Han's response to Anthropic's data showing software engineering accounts for ~50% of agentic API calls — he would start a company in that space today, treating the statistic as a signal of where autonomous agent demand is concentrating.

## @claudeai - Claude Code Security: AI-Powered Vulnerability Scanning in Research Preview
> Introducing Claude Code Security, now in limited research preview.
>
> It scans codebases for vulnerabilities and suggests targeted software patches for human review, allowing teams to find and fix issues that traditional tools often miss.
>
> Learn more: https://t.co/n4SZ9EIklG

- **Tweet:** https://x.com/claudeai/status/2024907535145468326
- **Link:** https://www.anthropic.com/news/claude-code-security
- **What:** Anthropic announces Claude Code Security, a research preview tool that scans codebases for vulnerabilities and proposes patches for human review. It aims to catch issues that conventional static analysis tools miss.

## @dickiebush - Every Rep Leapfrogs the People Who Quit
> Quick hack to stay motivated:
>
> Remember that every time you put in another rep, you're leapfrogging millions of people who quit on the exact step you're taking.

- **Tweet:** https://x.com/dickiebush/status/2024922834246529356
- **What:** A reframe on motivation: each rep completed at the point of resistance separates you from the majority who stop at that exact same step.

## @eptwts - Why HTML/CSS/JS Animation Tools Won't Replace Animators
> "vibe-animating" seems to be far away considering that all of these viral animation tools are just using HTML/ CSS/JS
>
> it's definitely cool tech but if vibe-animating ever becomes a thing that challenges animators, i can't see it happening with this approach
>
> video generation models represent a more promising path toward AI animation
>
> *Quoting @Replit:* Introducing Replit Animation
>
> Vibecode your next viral video in minutes, powered by Gemini 3.1 Pro.
>
> (This video was 100% made in Replit Animation)

- **Tweet:** https://x.com/eptwts/status/2024923654262313078
- **Quoted:** https://x.com/Replit/status/2024578806208745637
- **What:** A skeptical take on Replit's new Animation tool — argues that HTML/CSS/JS-based "vibe-animating" won't threaten professional animators, and that video generation models are the more credible path to AI-driven animation.

## @nateliason - https://t.co/rWLQPa3EPr
> Since I get countless questions about how @FelixCraftAI works, how he got started, and how in the world an OpenClaw with an X account has earned thousands of dollars in a few weeks...

Here you go!

(Drop questions in the replies and I'll write more).

https://t.co/igAcCkVaYT
>
> *Quoting @nateliason:* https://t.co/rWLQPa3EPr

- **Tweet:** https://x.com/nateliason/status/2024953510991712437
- **Quoted:** https://x.com/nateliason/status/2024953009524932705
- **Link:** https://x.com/nateliason/status/2024953009524932705
- **What:** Profile and overview of FelixCraft, an AI agent that manages a Twitter account and has generated thousands of dollars in revenue in just weeks.

---

---

# Wednesday, February 18, 2026

## @Austen - Solution was actually pretty simple:
> Solution was actually pretty simple: 

With a switch on intent + an HTTP request the agent can determine optimal way to retrieve info.

Falls back to full visual browser usage only if necessary.

Cuts token usage by ~80%.

A quick benchmark: https://t.co/VNLriP5BWm
>
> *Quoting @Austen:* I want someone to build browser automation for AI agents that doesn't suck.

Tak

- **Tweet:** https://x.com/Austen/status/2024339809884324345
- **Quoted:** https://x.com/Austen/status/2024215042653082025
- **What:** A browser automation optimization where an intent-detection switch plus a single HTTP request lets an AI agent skip full visual browser rendering, falling back to it only when necessary — cutting token usage by ~80%, with a benchmark linked.

---

---

# Tuesday, February 17, 2026

## @arscontexta - Skill Graphs: Interconnected Markdown Knowledge Networks for Agents
> https://t.co/XmYSO3mC8f

- **Tweet:** https://x.com/arscontexta/status/2023957499183829467
- **Link:** https://x.com/i/article/2023918991673061376
- **What:** An X article by Heinrich arguing that single skill files are insufficient for deep domain knowledge, proposing "skill graphs" — networks of small interconnected markdown files linked via wikilinks with YAML frontmatter, enabling progressive disclosure so agents traverse only relevant nodes. Introduces the arscontexta Claude Code plugin (~250 connected files) as a working example.

---

---

# Friday, January 16, 2026

## @affaanmustafa - The Shorthand Guide to Everything Claude Code
> https://t.co/NscRA7sqBt

- **Tweet:** https://x.com/affaanmustafa/status/2012378465664745795
- **Link:** https://x.com/i/article/2012310917812502528
- **What:** A comprehensive X article covering 10 months of daily Claude Code usage, detailing skills/commands, hooks (PreToolUse/PostToolUse/Stop), subagents, MCPs, plugins (LSP, hookify, mgrep), parallel workflows (fork, git worktrees), keyboard shortcuts, editor setup (Zed), and the author's full personal config including MCP servers and hook definitions.

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

# Saturday, January 3, 2026

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

# Tuesday, December 30, 2025

## @godofprompt - 8 AI Prompts Based on "Steal Like An Artist" Creativity Principles
> Austin Kleon reverse-engineered how every great artist actually works in his book "Steal Like An Artist"

I spent hours breaking down his principles and turned them into an AI system.

Nothing is original. Everything is a remix. Creativity is theft made elegant.

Here are 8 AI prompts that make you more creative, less blocked, and impossible to ignore:

- **Tweet:** https://x.com/godofprompt/status/2005943379193127409
- **What:** A thread sharing 8 AI prompts derived from Austin Kleon's "Steal Like An Artist" principles, designed to overcome creative blocks and produce more original-seeming content by systematically remixing and combining existing ideas.

## @RohunJauhar - Claude Code Prompt to Build a Full CEO Personal Productivity OS
> for any CEO using claude code — here's a single prompt that builds your entire 2026 personal productivity system.

annual planning, weekly reviews, etc.. one-shot copy/paste, come back 1 hour later, and start using immediately.

> *Quoting @RohunJauhar:* started using claude code this week and it feels like i just fast forwarded a few years into the future

- **Tweet:** https://x.com/RohunJauhar/status/2006147267959644303
- **Quoted:** https://x.com/RohunJauhar/status/2005465412692291620
- **What:** A single Claude Code prompt that autonomously generates a complete personal productivity operating system for CEOs — including daily check-ins, weekly/quarterly/annual reviews, self-interview scripts, and goal documents — using frameworks from Anthony Gustin, Tim Ferriss, Tony Robbins, and Alex Lieberman, stored as plain markdown files.

## @koylanai - Digital Brain skill for Claude Code
> Agent Skills for Context Engineering - digital brain implementation

- **Tweet:** https://x.com/koylanai/status/2005857134311854480
- **Link:** https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering
- **What:** GitHub repository containing a digital brain skill implementation for Claude Code, enabling advanced context engineering and knowledge management capabilities.

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

# Saturday, December 27, 2025

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
- **What:** THIN: @ryanvogel posted a video with no text description — content cannot be determined from the bookmark entry alone.

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

# Tuesday, December 23, 2025

## @steve_ike_ - AI Adoption Playbook
> This might be the cleanest AI adoption playbook inside a real product org I've seen.

- **Tweet:** https://x.com/steve_ike_/status/2003497265495785523
- **What:** 15-point comprehensive playbook covering practical approaches to implementing AI across organizations, from "How I AI" podcast.

---

---

# Saturday, November 22, 2025

## @alexhillman - Always Do (11 Imperatives)
> Always Keep Humans at the Center - use AI to remove drudgery and free up time for real, authentic relationships

- **Tweet:** https://x.com/alexhillman/status/1992252350812270856
- **What:** Personal reflection on core imperatives with emphasis on keeping humans central to all technology decisions.

---

---

# Saturday, November 8, 2025

## @alexgroberman - X/Twitter Growth System That Generated $120K in 48 Weeks
> I started my X account 48 weeks ago. Easiest algorithm to crack by a country mile.

Since then I've generated $120,000 in direct revenue, logged 10.24M impressions, and this month drove $20,000 to SEO Stuff.

Steal my system before Elon closes all the loopholes.

And if you want the full playbook with posting formats, DM frameworks, and engagement loops that create inbound, just follow me + RT this + comment "X Growth Guide 2025" and I'll DM you.

You must do all 3 to get the DM.

My posting schedule:

I post 2 to 3 times per day, 7 days per week.

Morning: Proof post or a strong POV tweet

Afternoon: 3 to 5 tweet mini-thread (framework, screenshot, teardown)

Evening: Repost with a new CTA or a short insight that sparks replies

If I stop posting for 48 hours, reach drops hard literally every single time.

What is actually working right now:

Short proof threads (3 to 6 tweets)

These need to be skimmable, visual, outcome-focused and actionable.

Multi-image posts (2 to 4 slides)

Slide 1: Big clear hook

Middle: Demo, framework, evidence

Final slide: CTA that earns replies

Anything results-based with verified info.

Dashboards, DMs, analytics, Stripe, rankings, prompts, etc.

Templates that can be copied instantly

Basically, if someone can steal it, reuse it, or apply it within 60 seconds, it has viral potential.

Timely commentary tied to firsthand experience like that Reddit/Perplexity lawsuit post I did a few days ago.

Mind you, this can be a reaction to platform shifts, product updates, or market changes with your own data or results.

Also, repost old winners.

Wait 2 to 3 weeks, rewrite the hook, post again.

Most of your audience never saw it the first time.

What is actually underperforming at the moment:

One-line "wisdom" tweets with no proof

Long threads where the main point is buried

AI-sounding content with no real examples or opinions

Frameworks that don't show the execution or outcome

Posts that send people off X before any engagement happens

Engagement stuff that works:

Reply early to posts gaining traction

Add proof, a data point, or a practical extension.

Quote tweet regularly with your own angle like nsights, breakdowns, disagreements, or additions.

Also, resurface your best replies.

So if one of your replies is gaining likes, repost it to your feed.

Build comment chains since posts that get comment replies, not just likes, live longer and reach further.

My DM system:

Watch who engages (replies, follows, repeat commenters)

DM them something useful (framework, prompt, swipe, guide)

If they respond, open a loop ("Want the full system?")

If yes, share the offer (SEO Stuff, audit, plan, package)

The order of operations here is value first, then context second and then pitch last.

Profile setup:

Bio = clear benefit first

Pinned tweet = proof + clear path to respond or DM

Rotate pinned tweet every 2 weeks based on clicks + replies

Answer DMs

The only metrics you should care about:

Link clicks per post

New followers after posting

DM replies after posting

Repeat comments from the same people

Comment depth (replies to replies)

Impressions look great on screenshots but clicks, conversations, and conversions pay the bills.

30 day action plan that works today:

Post 2 to 3 times daily (one proof post minimum)

Reply to 5 to 10 posts per day in your niche

Quote tweet 1 to 2 times per day with actual insight

Repost your strongest posts every 2 to 3 weeks

DM 10+ new engagers weekly with value first

Track clicks, replies, DMs, and repeat comments

Run this for 30 days.

Screenshot your Day 31 results.

Tag me when inbound starts.

And if you want the full playbook with posting formats, DM frameworks, and engagement loops that create inbound, just follow me + RT this + comment "X Growth Guide 2025" and I'll DM you.

You must do all 3 to get the DM.

- **Tweet:** https://x.com/alexgroberman/status/1987194775787995583
- **What:** A detailed X/Twitter growth playbook from someone who generated $120K in 48 weeks, covering posting schedules, content formats that work (proof threads, multi-image posts, templates), engagement tactics, DM outreach sequences, and a 30-day action plan. Emphasizes proof-based content and conversation depth over impressions.
