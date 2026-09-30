# Agent notes

- This repo is a content-only "awesome list" (README.md + etc/logo.png); there is no application code.
- The Base44 preview serves README.md with nginx + docsify (loaded from CDN). The docsify index.html is generated inside the container, not in the repo.
- The repo is mounted read-only at `/repo/`; README edits show after a browser refresh (no build step).
- Verify: `curl -s localhost:3000/repo/README.md | head`.
