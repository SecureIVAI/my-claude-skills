<h1 align="center">My Claude Skills</h1>

<div align="center">
<strong>Plug-and-play skills that make Claude Code unreasonably good at real work.</strong>
</div>div>

<br>

<div align="center">

  [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/SecureIVAI/my-claude-skills/blob/main/LICENSE)
  [![Stars](https://img.shields.io/github/stars/SecureIVAI/my-claude-skills?style=social)](https://github.com/SecureIVAI/my-claude-skills/stargazers)
  [![Forks](https://img.shields.io/github/forks/SecureIVAI/my-claude-skills?style=social)](https://github.com/SecureIVAI/my-claude-skills/network/members)
  ![8 Skills](https://img.shields.io/badge/skills-8-purple)
  ![Zero Dependencies](https://img.shields.io/badge/dependencies-zero-brightgreen)
  ![60 Second Setup](https://img.shields.io/badge/setup-60%20seconds-orange)

  </div>

  <div align="center">
    <sub>Customer success analytics &bull; DISC profiling &bull; Leadership coaching &bull; SDLC metrics<br>Project scheduling &bull; Prompt engineering &bull; Workflow automation &bull; and more</sub>sub>
  </div>div>
  
  ---
  
  ## Try It in 60 Seconds
  
  ```bash
# 1. Clone it
git clone https://github.com/SecureIVAI/my-claude-skills.git

# 2. Copy any skill into your project
cp my-claude-skills/leadership-skill.zip ~/my-project/
cd ~/my-project && unzip leadership-skill.zip

# 3. Start Claude Code. That's it. Claude picks up the skill automatically.
```

> **No API keys. No config files. No dependencies.** Just unzip and go.
>
> ---
>
> ## What's Inside
>
> | | Skill | What It Does | Try It |
> |---|-------|-------------|--------|
> | :dart: | **Customer Success Manager** | Health scoring, churn prediction, expansion opportunities -- 3 Python CLI tools that analyze your entire SaaS portfolio | [Explore](customer-success-manager/) |
> | :performing_arts: | **DISC Profiling** | Personality assessment and communication coaching based on the DISC behavioral model | [Download](DISC.zip) |
> | :bug: | **Defect KPIs & SDLC Metrics** | Defect density, escape rates, MTTR, test coverage, release quality gates -- everything you need to measure software quality | [Download](Defect_KPIs_SDLC_Metrics.zip) |
> | :crown: | **Leadership Skill** | Delegation frameworks, difficult conversations, strategic thinking, team motivation, and executive communication | [Download](leadership-skill.zip) |
> | :pencil2: | **Precise Verbs** | Replaces weak, vague verbs with powerful, specific alternatives -- instantly sharpens any professional writing | [Download](precise-verbs-skill.zip) |
> | :calendar: | **Project Scheduler Agent** | Breaks work into tasks, estimates durations, maps dependencies, flags critical path -- generates visual timelines | [Download](project-scheduler-agent.zip) |
> | :bulb: | **Prompt Design Bundle** | Chain-of-thought patterns, few-shot templates, system prompt frameworks, and evaluation rubrics | [Download](prompt-design-bundle.zip) |
> | :gear: | **Workflow Automation** | Maps existing processes, identifies bottlenecks, designs optimized workflows, creates automation specs | [Download](workflow.zip) |
>
> ---
>
> ## What Are Claude Skills?
>
> Think of them as **superpowers you install into Claude Code**. Each skill is a self-contained package of prompts, scripts, templates, and context that transforms Claude from a general-purpose assistant into a domain expert.
>
> Drop a skill into your project folder and Claude instantly knows how to do things like score customer health across a SaaS portfolio, coach you through difficult leadership conversations, or break a complex project into a dependency-mapped timeline.
>
> ---
>
> ## What People Build With These
>
> :briefcase: **SaaS Founders** run the Customer Success Manager tools before board meetings to identify at-risk accounts and expansion opportunities.
>
> :memo: **Technical Writers** use Precise Verbs to transform first drafts into sharp, professional documentation in a single Claude session.
>
> :bar_chart: **QA Leads** plug in the Defect KPIs skill to generate metrics dashboards that track quality across the entire SDLC.
>
> :people_holding_hands: **Managers** use the DISC and Leadership skills together to prepare for 1-on-1s, tailor their communication style, and navigate tough conversations.
>
> :rocket: **Project Managers** feed the Project Scheduler a scope doc and get back a structured timeline with critical path analysis.
>
> ---
>
> ## Deep Dive: Customer Success Manager
>
> The most fully-featured skill in the collection. Three production-grade Python CLI tools with zero external dependencies:
>
> ### Health Score Calculator
> Multi-dimensional scoring across four weighted dimensions:
>
> | Dimension | Weight | What It Measures |
> |-----------|--------|-----------------|
> | Usage | 30% | Login frequency, feature adoption, DAU/MAU ratio |
> | Engagement | 25% | Support tickets, meeting attendance, NPS/CSAT |
> | Support | 20% | Open tickets, escalation rate, resolution time |
> | Relationship | 25% | Executive sponsor engagement, multi-threading, renewal sentiment |
>
> Accounts are classified as **Green** (75-100), **Yellow** (50-74), or **Red** (0-49) with trend analysis comparing to previous periods.
>
> ### Churn Risk Analyzer
> Detects behavioral signals across five risk categories and classifies accounts into tiers: **Critical** (immediate escalation), **High** (urgent intervention), **Medium** (proactive outreach), or **Low** (standard monitoring).
>
> ### Expansion Opportunity Scorer
> Identifies upsell, cross-sell, and seat expansion opportunities with revenue estimates and priority rankings.
>
> ```bash
> # Run the full pipeline
> python customer-success-manager/scripts/health_score_calculator.py data.json --format json > health.json
> python customer-success-manager/scripts/churn_risk_analyzer.py data.json --format json > risk.json
> python customer-success-manager/scripts/expansion_opportunity_scorer.py data.json --format json > expansion.json
> ```
>
> Also includes QBR templates, success plan templates, onboarding checklists, and CS playbooks. See the full docs in [`customer-success-manager/SKILL.md`](customer-success-manager/SKILL.md).
>
> ---
>
> ## Also Included: GSD Agent for Claude Code
>
> This repo comes pre-configured with the **GSD (Get Shit Done) v1.27.0** agent in the `.claude/` directory -- a productivity layer for Claude Code with:
>
> - **Session hooks** that keep Claude focused across long tasks
> - - **Context monitoring** that tracks what Claude has touched
>   - - **Prompt guards** that catch drift before Claude goes off-track
>     - - **Status line** that shows real-time session health
>       -
>       - ---
>       -
>       - ## Repository Structure
>       -
>       - ```
>         my-claude-skills/
>         |-- .claude/                          # GSD agent (hooks, commands, settings)
>         |-- customer-success-manager/         # Full directory skill with Python tools
>         |   |-- assets/                       # Sample data + templates (QBR, success plan, onboarding)
>         |   |-- references/                   # Health scoring framework, CS playbooks, benchmarks
>         |   |-- scripts/                      # 3 Python CLI tools
>         |   +-- SKILL.md                      # Complete documentation
>         |-- DISC.zip                          # DISC personality profiling
>         |-- Defect_KPIs_SDLC_Metrics.zip      # Software quality metrics
>         |-- leadership-skill.zip              # Leadership coaching
>         |-- precise-verbs-skill.zip           # Precision writing
>         |-- project-scheduler-agent.zip       # Project scheduling
>         |-- prompt-design-bundle.zip          # Prompt engineering
>         |-- workflow.zip                      # Workflow automation
>         |-- CONTRIBUTING.md                   # Contribution guide
>         |-- LICENSE                           # MIT License
>         +-- README.md                         # You are here
>         ```
>
>         ---
>
>         ## Requirements
>
>         | Requirement | What For | Notes |
>         |------------|----------|-------|
>         | Claude Code | Everything | Desktop app or CLI |
>         | Python 3.7+ | Customer Success Manager scripts | Standard library only |
>         | Node.js | GSD agent hooks | Included in `.claude/` |
>
>         That's it. Every other skill is self-contained with zero dependencies.
>
>         ---
>
>         ## Contributing
>
>         We welcome new skills, improvements, and documentation fixes. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.
>
>         The short version: fork, create a branch, add your skill (with a `SKILL.md`), update this README, and open a PR.
>
>         ---
>
>         ## License
>
>         [MIT](LICENSE) -- use these skills however you want.
>
>         ---
>
>         <div align="center">
  <strong>Built by <a href="https://secureIVAI.com">Secure IVAI</a></strong><br>
  <sub>Safely integrating and securing AI solutions for SMBs.</sub><br><br>
  <a href="https://github.com/SecureIVAI/my-claude-skills/stargazers">Star this repo</a> if you find it useful -- it helps others discover these skills too.
  </div>
  
</sub>
</strong>
