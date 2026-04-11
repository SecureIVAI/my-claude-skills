# Contributing to My Claude Skills

Thank you for your interest in contributing! This guide explains how to add new skills, improve existing ones, or help with documentation.

---

## Ways to Contribute

- **Submit a new skill** — Share a Claude Code skill you have built
- - **Improve an existing skill** — Better prompts, more templates, bug fixes
  - - **Improve documentation** — Clearer instructions, more examples, typo fixes
    - - **Report issues** — Found a bug or have a suggestion? Open an issue
     
      - ---

      ## Submitting a New Skill

      ### Skill Structure

      Every skill should include at minimum:

      1. **A `SKILL.md` file** at the root of your skill directory with frontmatter metadata:
     
      2. ```yaml
         ---
         name: your-skill-name
         description: One-line description of what the skill does
         license: MIT
         metadata:
           version: "1.0.0"
           author: Your Name
           category: your-category
           domain: your-domain
         ---
         ```

         2. **Clear documentation** explaining what the skill does, how to use it, and any requirements
        
         3. 3. **Sample data or examples** so users can test the skill immediately
           
            4. ### Naming Conventions
           
            5. - Use lowercase kebab-case for skill directories and ZIP files (e.g., `my-new-skill/` or `my-new-skill.zip`)
               - - Name scripts descriptively (e.g., `health_score_calculator.py` not `script1.py`)
                
                 - ### Testing Your Skill
                
                 - Before submitting, verify that:
                
                 - - The skill works in a fresh Claude Code session
                   - - All scripts run without errors using only the documented dependencies
                     - - Sample data or examples produce the expected output
                       - - Documentation is clear enough for someone unfamiliar with the skill to use it
                        
                         - ---

                         ## How to Submit

                         1. **Fork** this repository
                         2. 2. **Create a branch** for your contribution (`git checkout -b add-my-new-skill`)
                            3. 3. **Add your skill** as either a directory or a ZIP file in the repo root
                               4. 4. **Update the README** to include your skill in the Skills Included table and Skill Details section
                                  5. 5. **Commit** with a descriptive message (e.g., `feat: add data-analysis skill for CSV exploration`)
                                     6. 6. **Open a Pull Request** with a clear description of what your skill does
                                       
                                        7. ---
                                       
                                        8. ## Code of Conduct
                                       
                                        9. - Be respectful and constructive in all interactions
                                           - - Focus feedback on the work, not the person
                                             - - Help others learn and improve
                                              
                                               - ---

                                               ## Questions?

                                               Open an issue or reach out at [info@secureIVAI.com](mailto:info@secureIVAI.com).

                                               Thank you for helping make Claude skills better for everyone!
                                               
