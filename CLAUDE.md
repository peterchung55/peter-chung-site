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

## Adding a Weekly Briefing issue (blog)

The brief for writing an issue is in `.claude/weekly-briefing.md`. Issues are dated Wednesdays.

1. Copy the latest `blog/weekNN/index.html` to `blog/week(NN+1)/index.html` and replace the content:
   `<title>`, meta description, canonical/og URLs, `article:published_time`, h1, issue no. and date,
   the take, the side facts, the Korean paragraph, and the item list with source links.
2. Add a new `.row` at the top of the list in `blog/index.html` (newest first).
3. On the previous issue page, point the pager's left slot at the new issue if useful.
4. Pages under `blog/` use root-absolute paths (`/assets/...`, `/blog/`), so preview them through the
   `site` server in `.claude/launch.json`, not by opening the file directly.

`CLAUDE.md` and `.claude/` are listed in `.vercelignore` so they are not published on the site.

Pushes must go through the `peterchung55` GitHub account (this PC's default GitHub login).
If a push fails with 403 / permission denied, stop and tell the owner rather than retrying.
