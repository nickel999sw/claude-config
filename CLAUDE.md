# Global instructions

## Project locations
- Golfrounds app repo: /Users/niklaslindefelt/Code/golfrounds. The Firestore spec lives at /Users/niklaslindefelt/Code/golfrounds/docs/spec-sammanvagd-runda.md.
- Training modules site repo: /Users/niklaslindefelt/Code/golftraining. It deploys via GitHub Pages on push to main.
- If the session starts outside these directories, cd into the correct repo before doing anything else.

## Machine context
- I use three Macs. Before doing any filesystem work, run `scutil --get ComputerName` to confirm which machine this session is on.
  - Mac mini M5 Pro, "MacMiniF". Bought in Ferragudo, Portugal, now in Sweden. My main machine.
  - MacBook Pro M4, "MacBookProM4".
  - Mac mini M4, in Sweden. Used less now that MacMiniF is here.
- This file is shared across the Macs via the repo ~/Code/claude-config (~/.claude/CLAUDE.md is a symlink to it). If it has not been pulled for more than a day, run `git -C ~/Code/claude-config pull` at the start of the session. After changing it, commit and ask me before pushing.
- Each Mac needs its own tool setup (Homebrew, Node, Java 21, firebase-tools, uv). Pull repos with `git pull` before working.
- Never touch work OneDrive folders unless I ask. Personal files go into iCloud Drive.

## Working style
- If I give a rule or spec, implement my version first. If you think another approach is better, propose it separately and wait for my OK before switching.
- Stay on the current task. Do not switch to other projects unless I ask.
