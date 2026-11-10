# Pagecraft

A bullet journal with a new hand-designed look every day. Each date gets its own palette, fonts, paper, box styles and doodles, and you can shuffle for a new look anytime.

It includes a daily log (tasks, events and notes), a habit tracker, a mood, water and sleep check-in, gratitude, notes with a daily prompt, a month view, and boxes you design yourself (checklists, writing space, tap trackers and number logs).

---

## Put Pagecraft online with GitHub Pages

You only need a free GitHub account and a web browser. No coding or command line is needed.

### 1. Create a repository

1. Sign in at [github.com](https://github.com).
2. Click **+** (top right) → **New repository**.
3. **Repository name:** `pagecraft` (this becomes part of your web address).
4. Choose **Public**. Free GitHub Pages needs a public repo. Only the app's code is public; nobody's journal entries are ever uploaded.
5. Leave the other options alone and click **Create repository**.

### 2. Upload the files

1. On the new, empty repository page, click the link **uploading an existing file**.
2. Open the `pagecraft` folder on your computer, select **everything inside it** (`index.html`, `manifest.webmanifest`, `sw.js`, `README.md` and the `icons` folder), and drag it all onto the upload area.
   - Upload the *contents* of the folder, not the `pagecraft` folder itself. `index.html` must sit at the top level of the repository.
   - Dragging the `icons` folder keeps it as a folder on GitHub. This works in Chrome, Edge and Firefox. If `icons/` is missing after you commit, see **The icon is missing** under Troubleshooting.
3. Scroll down and click **Commit changes**.

When it's done, the repository should list `icons/`, `index.html`, `manifest.webmanifest`, `README.md` and `sw.js`.

### 3. Turn on GitHub Pages

1. In the repository, click **Settings** (top bar).
2. In the left sidebar, click **Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Under **Branch**, choose **main** and **/ (root)**, then click **Save**.
5. Wait one to two minutes, then refresh the page. A box at the top shows your live address:

   `https://YOUR-USERNAME.github.io/pagecraft/`

Open that link and Pagecraft is live.

---

## Install it on your phone

**iPhone or iPad (use Safari):**
1. Open your Pagecraft link in Safari.
2. Tap the **Share** button (square with an arrow).
3. Scroll down and tap **Add to Home Screen**, then **Add**.

**Android (use Chrome):**
1. Open your Pagecraft link in Chrome.
2. Tap **⋮** (top right), then **Install app** or **Add to Home screen**.

Pagecraft then opens full-screen from its own icon, and works offline after the first visit.

**On a computer**, Chrome and Edge show an install icon in the address bar. You can also just bookmark the link.

---

## Good to know

- **Your entries stay on your device.** Everything is saved in the browser on that phone or computer. Nothing is sent anywhere, and each device keeps its own journal.
- **Make backups.** Use **⋯ → Export backup** now and then. On a phone this opens the share sheet so you can save the file to Files or Drive, or email it to yourself. **⋯ → Import backup** restores it, including on a different device.
- **iPhone tip:** use the home-screen app rather than a Safari tab. Safari can clear saved data for websites you haven't visited in a while; home-screen apps are much less affected. Backups are still a good idea.
- **Fonts:** the handwritten fonts load from Google Fonts. Pagecraft keeps a copy of each font once you've seen it, so offline you may get a plain fallback font for a look you haven't seen before.
- **Sharing:** anyone can open your link and start their own journal. They never see your entries.

---

## Updating Pagecraft later

1. In the repository, click **Add file → Upload files** and upload the changed files. Files with the same name are replaced.
2. Open `sw.js`, click the pencil icon to edit, and change `pagecraft-v1` to `pagecraft-v2` (then `v3`, and so on, each time you update). Click **Commit changes**.
3. Installed copies pick up the new version the next time they're opened with an internet connection, sometimes on the second launch. Journal entries are not affected.

---

## Troubleshooting

- **The link shows a 404 page.** Wait a few minutes after turning on Pages, and check that `index.html` is at the top level of the repository, not inside a folder.
- **The icon is missing.** The repository needs an `icons` folder with all six image files inside it. If dragging the folder didn't work (some versions of Safari don't support it), upload it again from Chrome, Edge or Firefox. Or create it by hand: click **Add file → Create new file**, type `icons/placeholder.txt` as the name, commit, open the new `icons` folder, use **Add file → Upload files** to add the six images, then delete `placeholder.txt`.
- **Changes don't show up.** Make sure you bumped the version in `sw.js`, then close and reopen the app.

---

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, icon and colors for installing to a home screen |
| `sw.js` | Lets the app open offline and keeps copies of fonts |
| `icons/` | App icons (`icon-1024.png` is a full-size master copy) |
