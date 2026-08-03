# Deploying to GitHub Pages

No terminal, no git, no build step. Everything below happens in a browser and takes about ten minutes.

Your GitHub username is **`kanishkajain621ak`**, so every URL below is already filled in.
Your portfolio will live at **https://kanishkajain621ak.github.io**

---

## Step 1 — Create the repository

1. Click the **+** in the top-right of github.com → **New repository**
2. **Repository name:** type exactly your username followed by `.github.io`

       kanishkajain621ak.github.io

   This exact naming is what gives you a clean root URL. Any other name puts the site at
   `username.github.io/reponame/` instead, which looks worse on a résumé.
3. Set it to **Public**. Private repos can't serve GitHub Pages on a free account, and you want this
   public anyway — it's the code sample that fills your empty profile.
4. Leave "Add a README file" **unticked**. You already have one.
5. Click **Create repository**.

---

## Step 2 — Upload the files

On the empty repository page you'll see a link reading **"uploading an existing file"**. Click it.

1. Open the unzipped `portfolio` folder on your computer.
2. Select **everything inside it** — `index.html`, `README.md`, `DEPLOY.md`, `SCREENSHOTS.md`,
   `.nojekyll`, the résumé PDF, and the `images` folder — and drag the whole selection onto the upload area.

   Drag the **contents** of the folder, not the folder itself. If you drag `portfolio` as a folder, every
   file lands one level too deep and the site won't load.

3. Dragging the `images` folder is fine and keeps its subfolders intact — GitHub preserves the structure.
4. Scroll down, leave the commit message as-is, click **Commit changes**.

Uploading 27 images takes a minute or two. Wait for it to finish before moving on.

---

## Step 3 — Turn on Pages

1. In your repository, click **Settings** (top row, far right)
2. In the left sidebar, click **Pages**
3. Under "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** `main`, folder `/ (root)`
4. Click **Save**

---

## Step 4 — Visit your site

Wait 60–90 seconds, then open:

    https://kanishkajain621ak.github.io

If you get a 404, wait another minute and hard-refresh with `Ctrl+Shift+R`. First deploys are sometimes slow.

**That URL now goes on your résumé, your LinkedIn profile, and every application you send.**

---

## Updating it later

**To replace a screenshot:** navigate to the file in the repo (`images` → project folder), click
**Add file → Upload files**, drag the new PNG in with the same filename, commit. Live within a minute.
Hard-refresh to see it — browsers cache images aggressively.

**To edit text:** click `index.html`, click the pencil icon, edit, scroll down, commit.

---

## Troubleshooting

| Symptom | Cause |
|---|---|
| Site 404s after several minutes | Repository is private, or Pages source wasn't saved. Re-check Settings → Pages. |
| Page loads but is unstyled | `index.html` ended up inside a subfolder. It must be at the repository root. |
| Images broken | Folder structure was flattened on upload. `images/divine-hindu/01-home.png` must be that exact path. |
| Changes not showing | Browser cache — hard-refresh `Ctrl+Shift+R`. |

---

## Once it's live

- [ ] Add the URL to your résumé contact line (it currently says `[portfolio URL]`)
- [ ] Add it to your LinkedIn profile — Contact info → Website
- [ ] Create a second repo named exactly your username (`kanishkajain621ak`) with a `README.md` in it —
      GitHub displays that file at the top of your profile page. Point it at the portfolio.
- [ ] Replace the placeholder screenshots as you capture them (see `SCREENSHOTS.md`)
