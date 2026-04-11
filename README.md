# My Claude Skills

Ready-to-use skills and agents for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — covering customer success analytics, DISC personality profiling, leadership coaching, defect and SDLC metrics, project scheduling, prompt engineering, and workflow automation.

**Download a ZIP, drop it into your Claude project folder, and start using it immediately.** No external dependencies, no API keys, no setup headaches.

---

## Table of Contents

- [What Are Claude Skills?](#what-are-claude-skills)
- - [Skills Included](#skills-included)
  - - [Quick Start](#quick-start)
    - - [Skill Details](#skill-details)
      - - [Repository Structure](#repository-structure)
        - - [Requirements](#requirements)
          - - [Contributing](#contributing)
            - - [License](#license)
             
              - ---

              ## What Are Claude Skills?

              Claude Skills are reusable configurations, prompts, scripts, and templates that extend what Claude Code can do. Think of them as plug-and-play modules — each skill focuses on a specific domain (customer analytics, leadership, project management, etc.) and gives Claude the context and tools it needs to deliver expert-level output in that area.

              ---

              ## Skills Included

              | Skill | Description | Format |
              |-------|-------------|--------|
              | **Customer Success Manager** | Health scoring, churn risk analysis, and expansion opportunity identification for SaaS portfolios | Directory (Python CLI tools) |
              | **DISC Profiling** | DISC personality assessment and communication coaching | ZIP |
              | **Defect KPIs & SDLC Metrics** | Software quality metrics, defect tracking KPIs, and SDLC measurement frameworks | ZIP |
              | **Leadership Skill** | Leadership coaching, team management strategies, and executive communication | ZIP |
              | **Precise Verbs** | Writing skill focused on replacing weak verbs with strong, specific alternatives | ZIP |
              | **Project Scheduler Agent** | Project planning, timeline estimation, and task dependency management | ZIP |
              | **Prompt Design Bundle** | Prompt engineering patterns, templates, and best practices for Claude | ZIP |
              | **Workflow Automation** | Task automation, process optimization, and workflow design | ZIP |

              ---

              ## Quick Start

              ### Option 1: Use a ZIP Skill

              1. Download the `.zip` file for the skill you want (e.g., `leadership-skill.zip`)
              2. 2. Unzip it into your Claude Code project directory
                 3. 3. Start a Claude Code session — Claude will automatically detect and use the skill
                   
                    4. ### Option 2: Use the Customer Success Manager (Directory Skill)
                   
                    5. The `customer-success-manager/` directory is ready to use as-is:
                   
                    6. ```bash
                       # Clone the repo
                       git clone https://github.com/SecureIVAI/my-claude-skills.git
                       cd my-claude-skills

                       # Run health scoring on your customer data
                       python customer-success-manager/scripts/health_score_calculator.py your_data.json

                       # Run churn risk analysis
                       python customer-success-manager/scripts/churn_risk_analyzer.py your_data.json

                       # Find expansion opportunities
                       python customer-success-manager/scripts/expansion_opportunity_scorer.py your_data.json
                       ```

                       All three scripts support `--format json` for machine-readable output that can be piped into other tools.

                       ### Option 3: Use the GSD (Get Shit Done) Agent

                       This repo includes a pre-configured `.claude/` directory with the GSD v1.27.0 agent for Claude Code, complete with hooks for session monitoring, context tracking, and prompt guarding.

                       ---

                       ## Skill Details

                       ### Customer Success Manager

                       Production-grade customer success analytics with three Python CLI tools:

                       - **Health Score Calculator** — Multi-dimensional scoring across usage (30%), engagement (25%), support (20%), and relationship (25%) dimensions. Classifies accounts as Green/Yellow/Red with trend analysis.
                       - - **Churn Risk Analyzer** — Behavioral signal detection covering usage decline, engagement drops, support issues, relationship signals, and commercial factors. Outputs risk tiers: Critical, High, Medium, Low.
                         - - **Expansion Opportunity Scorer** — Identifies upsell, cross-sell, and seat expansion opportunities with revenue estimates and priority rankings.
                          
                           - Includes QBR templates, success plan templates, onboarding checklists, health scoring framework documentation, and CS playbooks. See [`customer-success-manager/SKILL.md`](customer-success-manager/SKILL.md) for full documentation.
                          
                           - **Requirements:** Python 3.7+ (standard library only — zero external dependencies)
                          
                           - ### DISC Profiling
                          
                           - Personality assessment skill based on the DISC behavioral model (Dominance, Influence, Steadiness, Conscientiousness). Helps Claude coach users on communication styles, team dynamics, and interpersonal effectiveness.
                          
                           - ### Defect KPIs & SDLC Metrics
                          
                           - Frameworks for measuring software quality throughout the development lifecycle — defect density, escape rates, mean time to resolution, test coverage analysis, and release quality gates.
                          
                           - ### Leadership Skill
                          
                           - Executive coaching and leadership development — covers delegation frameworks, difficult conversations, strategic thinking, team motivation, and leadership communication patterns.
                          
                           - ### Precise Verbs
                          
                           - A writing-focused skill that trains Claude to replace vague, weak verbs with specific, powerful alternatives. Useful for professional writing, documentation, and business communication.
                          
                           - ### Project Scheduler Agent
                          
                           - An agentic skill for project planning — breaks down work into tasks, estimates durations, identifies dependencies, flags critical path items, and generates timeline visualizations.
                          
                           - ### Prompt Design Bundle
                          
                           - A collection of prompt engineering patterns and templates, including chain-of-thought structures, few-shot examples, system prompt frameworks, and evaluation rubrics for prompt quality.
                          
                           - ### Workflow Automation
                          
                           - Process design and automation skill — helps map existing workflows, identify bottlenecks, design optimized processes, and create automation specifications.
                          
                           - ---

                           ## Repository Structure

                           ```
                           my-claude-skills/
                           ├── .claude/                          # Claude Code configuration (GSD agent)
                           │   ├── agents/                       # Agent definitions
                           │   ├── commands/gsd/                 # GSD slash commands
                           │   ├── get-shit-done/                # GSD core modules
                           │   ├── hooks/                        # Session, context, and prompt hooks
                           │   ├── settings.json                 # Claude Code settings with hook config
                           │   └── package.json                  # GSD package metadata
                           ├── customer-success-manager/         # Full directory skill (not zipped)
                           │   ├── assets/                       # Sample data, templates (QBR, success plan, onboarding)
                           │   ├── references/                   # Health scoring framework, CS playbooks, benchmarks
                           │   ├── scripts/                      # Python CLI tools (health, churn, expansion)
                           │   └── SKILL.md                      # Detailed skill documentation
                           ├── DISC.zip                          # DISC personality profiling skill
                           ├── Defect_KPIs_SDLC_Metrics.zip      # Software quality metrics skill
                           ├── leadership-skill.zip              # Leadership coaching skill
                           ├── precise-verbs-skill.zip           # Precise writing skill
                           ├── project-scheduler-agent.zip       # Project scheduling agent
                           ├── prompt-design-bundle.zip          # Prompt engineering skill
                           ├── workflow.zip                      # Workflow automation skill
                           ├── CONTRIBUTING.md                   # How to contribute
                           ├── LICENSE                           # MIT License
                           └── README.md                         # This file
                           ```

                           ---

                           ## Requirements

                           - **Claude Code** (Claude desktop app or CLI with Claude Code enabled)
                           - - **Python 3.7+** for the Customer Success Manager scripts (standard library only)
                             - - **Node.js** for the GSD agent hooks (included in `.claude/`)
                              
                               - No other external dependencies are required for any skill.
                              
                               - ---

                               ## Contributing

                               Contributions are welcome! Whether it is a new skill, an improvement to an existing one, or better documentation — all contributions help.

                               See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to submit skills, report issues, or suggest improvements.

                               ---

                               ## License

                               This project is licensed under the [MIT License](LICENSE) — you are free to use, modify, and distribute these skills in your own projects.

                               ---

                               **Built by [Secure IVAI](https://secureIVAI.com)** — Safely integrating and securing AI solutions for SMBs.
                               
