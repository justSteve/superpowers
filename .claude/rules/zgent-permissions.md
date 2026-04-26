# Rule: Zgent Permissions — superpowers (Infrastructure Fork)

## Filesystem
- READ any file under the enterprise root directory tree
- WRITE only within this repository's directory (`/root/projects/superpowers/`)
- NEVER read or write outside the enterprise root

## GitHub
- READ any repository under `justSteve/`
- READ upstream at `obra/superpowers` (issues, PRs, commits, discussions)
- WRITE (push, branch, PR, issues) only to `justSteve/superpowers`
- NEVER push to `obra/superpowers` (upstream) — enterprise artifacts do not belong upstream
- Cross-repo writes require explicit delegation via beads

## Upstream Sync
- Fetch and merge from `upstream` (obra/superpowers) freely
- Push only to `origin` (justSteve/superpowers)

## Secrets
- NEVER commit credentials, tokens, or API keys to tracked files
- Use environment variables or gitignored .env files
