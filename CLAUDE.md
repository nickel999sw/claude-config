# Global instructions

## Project locations
- Golfrounds app repo: /Users/niklaslindefelt/Code/golfrounds. The Firestore spec lives at /Users/niklaslindefelt/Code/golfrounds/docs/spec-sammanvagd-runda.md.
- Training modules site repo: /Users/niklaslindefelt/Code/golftraining. It deploys to Firebase Hosting (site golftraining-nl in golfrounds-ac8bd, https://golftraining-nl.web.app) with `npm run deploy`; ask before deploying. GitHub Pages only serves a link page from the gh-pages branch, so a push to main publishes nothing.
- If the session starts outside these directories, cd into the correct repo before doing anything else.

## Machine context
- I use three Macs. Before doing any filesystem work, run `scutil --get ComputerName` to confirm which machine this session is on.
  - Mac mini M5 Pro, "MacMiniF". Bought in Ferragudo, Portugal, now in Sweden. My main machine.
  - MacBook Pro M4, "MacBookProM4".
  - Mac mini M4, in Sweden. Used less now that MacMiniF is here.
- This file is shared across the Macs via the repo ~/Code/claude-config (~/.claude/CLAUDE.md is a symlink to it). If it has not been pulled for more than a day, run `git -C ~/Code/claude-config pull` at the start of the session. After changing it, commit and ask me before pushing.
- Each Mac needs its own tool setup (Homebrew, Node, Java 21, firebase-tools, uv). Pull repos with `git pull` before working.
- Never touch work OneDrive folders unless I ask. Personal files go into iCloud Drive.
- When moving or reorganizing files: first write a move plan (source → destination, size) to `~/Library/Mobile Documents/com~apple~CloudDocs/move-log.md`, excluding OneDrive and work folders. Wait for my OK, then move and mark each row done, so another Mac can continue from the log.

## Working style
- If I give a rule or spec, implement my version first. If you think another approach is better, propose it separately and wait for my OK before switching.
- For UI behavior or sync/delete logic: before coding, write a short behavior spec (rules, edge cases such as after save, after delete, offline and the first item, and the tests you will add). If my rule and your proposal differ, show both. Wait for my OK before coding.
- Keep changes minimal: no abstractions, options or error handling I did not ask for.
- Touch only what the task needs and match the existing style. Mention unrelated dead code or refactoring ideas, but do not change them.
- Stay on the current task. Do not switch to other projects unless I ask.
