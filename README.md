# IELTS Sprint — 10 Days to 7.5

A single-file, self-contained tracker for a 10-day IELTS prep sprint: daily checklist, mock-score chart toward a 7.5 goal, and original practice drills for Listening Section 4 and Reading Passage 3. No build step, no dependencies — it's one `index.html` file. All progress is saved in the browser's `localStorage`, so nothing leaves the device.

## Run it locally

Just open `index.html` in any browser, or serve the folder:

```bash
npx serve .
```

## Push this to GitHub

This folder is already a local git repo with one commit. To publish it:

1. Create a new **empty** repository on GitHub (no README/license/gitignore) — e.g. named `ielts-sprint`.
2. Copy the remote URL it gives you (HTTPS or SSH), then from this folder run:

   ```bash
   git remote add origin <the-url-you-copied>
   git branch -M main
   git push -u origin main
   ```

   You'll be prompted to authenticate with GitHub the way you normally do (browser sign-in, a personal access token, or SSH key).

## Enable GitHub Pages (to get a live link)

1. On GitHub, go to the repo's **Settings → Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
4. GitHub will give you a URL like:

   ```
   https://<your-username>.github.io/ielts-sprint/
   ```

   It can take a minute or two to go live after the first save, and again after every future push.

## Updating the plan later

Everything — the 10-day schedule, the practice drills, the chart logic — lives in `index.html`. Edit it, then:

```bash
git add index.html
git commit -m "Update plan"
git push
```

Pages will redeploy automatically within a minute or so of the push.
