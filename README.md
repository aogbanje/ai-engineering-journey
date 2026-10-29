# AI Engineering Journey

Working through the [AI Engineering from Scratch](https://github.com/rohitg00/ai-engineering-from-scratch) curriculum with the AI tutor.

## Where things are
- `LEARNING.md`: source of truth for my progress, path, and review queue
- `phases/`: my own implementations of each lesson
- `projects/`: things I built using what I learned (or links to their repos)

## Projects
_PSB_

## Setup (to rebuild on a new machine)
```bash
# 1. Install Node (nvm) and check it
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
# open a new terminal
nvm install --lts
node -v
npx -v

# 2. Get the repo
git clone https://github.com/aogbanje/ai-engineering-journey.git
cd ~/ai-engineering-journey

# 3. Set your Git identity
git config --global user.name "your-name"
git config --global user.email "your-github-email"
git config --global init.defaultBranch main

# 4. Install the course skills
npx skills add rohitg00/ai-engineering-from-scratch
# You chose all skills, the agents Claude Code, Codex, Grok Build and OpenCode, scope Project, method Symlink, and yes to find-skills.

# 5. Commit and push the skills
git add .
git commit -m "chore: add ai engineering course skills"
git push

# 6. Check the skill's instructions (optional)
grep -n -i "LEARNING.md\|ROADMAP" .agents/skills/start-learning/SKILL.md | head -20

# 7. Install and open Codex
npm install -g @openai/codex
which codex
cd ~/ai-engineering-journey
codex
# type start-learning inside Codex.

# After every reset
# The repo and skills live on GitHub, so you only redo the tools:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
# open a new terminal
nvm install --lts
npm install -g @openai/codex
git config --global user.name "your-name"
git config --global user.email "your-github-email"
cd ~/ai-engineering-journey   # or: git clone ... first if the folder is gone
codex

start-learning
```
