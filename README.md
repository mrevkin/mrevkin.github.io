# Mara Revkin — GitHub Pages Website

This folder contains a complete static website ready to upload to GitHub Pages at your existing repo:
**https://github.com/mrevkin/mrevkin.github.io**

---

## How to Upload to GitHub Pages

### Option A — Upload via GitHub.com (no coding needed)

1. Go to **https://github.com/mrevkin/mrevkin.github.io** in your browser
2. If the repo already has files, you'll want to clear them first (or just overwrite)
3. Click **Add file → Upload files**
4. Drag the entire contents of this folder (all .html, style.css, and the `images/` folder) into the upload window
5. At the bottom, click **Commit changes**
6. Your site will be live at **https://mrevkin.github.io** within a minute or two

> **Note:** GitHub Pages serves `index.html` as the homepage automatically.

---

### Option B — Upload via GitHub Desktop (easier for large folders)

1. Download [GitHub Desktop](https://desktop.github.com/) if you don't have it
2. Clone your repo: File → Clone Repository → mrevkin/mrevkin.github.io
3. Copy all files from this folder into the cloned repo folder on your computer
4. In GitHub Desktop, you'll see all the new files listed
5. Add a commit message (e.g., "New website") and click **Commit to main**
6. Click **Push origin**
7. Live at **https://mrevkin.github.io** within a minute

---

## Connecting Your Custom Domain (mararevkin.com)

To use `mararevkin.com` instead of `mrevkin.github.io`:

1. In your GitHub repo, go to **Settings → Pages**
2. Under "Custom domain", type `mararevkin.com` and click Save
3. GitHub will create a file called `CNAME` in your repo automatically
4. Log in to wherever you bought your domain (likely GoDaddy, Namecheap, etc.)
5. Find the DNS settings and add these records:

   | Type | Name | Value |
   |------|------|-------|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | mrevkin.github.io |

6. DNS changes take up to 24 hours to propagate
7. Once it works, check "Enforce HTTPS" in GitHub Pages settings for the padlock icon

---

## File Structure

```
mararevkin-github-site/
├── index.html              ← Home page
├── research.html           ← Research areas
├── teaching.html           ← Courses
├── cv.html                 ← C.V. with PDF link
├── data.html               ← Datasets
├── policy-ngo-reports.html ← Policy reports gallery
├── media.html              ← Media coverage
├── contact.html            ← Contact info
├── style.css               ← All styles (shared)
├── images/
│   ├── header-ninewa.jpeg          ← Home banner
│   ├── writing-ninewa.jpeg         ← Home sidebar photo
│   ├── research-police.jpeg
│   ├── research-rebel-governance.jpg
│   ├── research-transitional-justice.jpeg
│   ├── research-comparative-law.jpg
│   ├── research-law-armed-conflict.jpg
│   ├── research-human-rights.jpeg
│   ├── cv-flying-iraq.jpeg
│   └── contact-istanbul.jpeg
└── README.md               ← This file
```

---

## Placeholders to Fill In

Before going live, you'll want to:

- **Add your headshot** — Save it as `images/headshot.jpeg`, then in `index.html` and `contact.html` replace the gray placeholder div with:
  ```html
  <img src="images/headshot.jpeg" alt="Mara Revkin" />
  ```
- **Add your CV PDF** — Save it as `revkin_cv.pdf` in the main folder, then in `cv.html` uncomment the `<iframe>` block
- **Add your teaching photo** — Save it as `images/teaching-lecture.jpeg` and replace the placeholder in `teaching.html`
- **Add Policy report covers** — Download the cover images from your current Weebly site and swap out the gray placeholder boxes in `policy-ngo-reports.html`
- **Update email** — The site currently uses `mara.revkin@duke.edu`. Update if different.

---

## Editing Content Later

All content is plain HTML. Open any `.html` file in a text editor (TextEdit, Notepad, VS Code, etc.) to make changes. The text is readable — you don't need to know HTML deeply to update names, dates, or links.
