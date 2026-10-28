# claude-config

My global Claude Code instructions, shared across my Macs.
`~/.claude/CLAUDE.md` is a symlink to `CLAUDE.md` in this repo.

Set up on a new Mac:

```sh
git clone https://github.com/nickel999sw/claude-config.git ~/Code/claude-config
mv ~/.claude/CLAUDE.md ~/.claude/CLAUDE.md.bak 2>/dev/null; ln -s ~/Code/claude-config/CLAUDE.md ~/.claude/CLAUDE.md
```
