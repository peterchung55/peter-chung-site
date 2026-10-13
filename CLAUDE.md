# peter-chung-site

Static personal website for Hyung-Eun (Peter) Chung, served at https://peterchung.kr.
Plain HTML/CSS/JS, no build step: `index.html`, `record/`, `assets/site.css`, `assets/site.js`, `images/`.

## Deployment

- GitHub repo: `peterchung55/peter-chung-site`, branch `main`.
- Vercel is connected to that repo and redeploys automatically on every push to `main`.

## Workflow (standing instruction from the owner)

After making any requested change to the site, without asking first:

1. `git pull --rebase origin main` before editing, so the local copy is current.
2. Make the change and check it (open the page in the browser pane if it's visual).
3. Commit with a short, descriptive message.
4. `git push origin main` — this publishes the change to the live site via Vercel.
5. Tell the owner what changed and that it was pushed.

Pushes must go through the `peterchung55` GitHub account (the remote URL pins it).
If a push fails with 403 / permission denied, stop and tell the owner rather than retrying.
