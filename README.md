# Academic Website

A clean, minimalist academic webpage built with plain HTML & CSS.  
Font: Cormorant Garamond · Palette: Black & White

---

## File Structure

```
academic-site/
├── index.html        ← redirects to about.html
├── about.html        ← About: bio, features, news
├── research.html     ← Research: interests, publications, service
├── teaching.html     ← Teaching: courses, supervision, notes & blogs
├── others.html       ← Others: photo gallery
├── style.css         ← shared styles (edit for global changes)
└── images/           ← create this folder and put your photos here
```

---

## How to publish on GitHub Pages

### 1. Create a GitHub repository

- Go to [github.com](https://github.com) and click **New repository**
- Name it: `yourusername.github.io`  
  *(replace `yourusername` with your actual GitHub username)*
- Set it to **Public**
- Click **Create repository**

### 2. Upload the files

**Option A — via the GitHub website (easiest):**
1. Open your new repository
2. Click **Add file → Upload files**
3. Drag all files from this folder into the upload area
4. Click **Commit changes**

**Option B — via Git (recommended for ongoing edits):**
```bash
git init
git add .
git commit -m "Initial site"
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. In your repository, go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose **main** branch and **/ (root)** folder
4. Click **Save**

Your site will be live at:  
**`https://yourusername.github.io`**  
*(it may take 1–2 minutes to appear)*

---

## How to customise

### Personal info
Search for `[Your Name]`, `[Your Title]`, `[University]` etc. across all `.html` files and replace with your real details.

### Photo (about.html)
1. Create an `images/` folder
2. Add your photo as `images/photo.jpg`
3. In `about.html`, replace the `<div class="photo-placeholder">` block with:
   ```html
   <img src="images/photo.jpg" alt="[Your Name]"/>
   ```

### Gallery photos (others.html)
1. Put images in `images/`
2. Inside each `.gallery-item`, replace the `<div class="gallery-placeholder">` with:
   ```html
   <img src="images/your-photo.jpg" alt="Description"/>
   ```

### Adding publications (research.html)
Copy any `.pub-item` block and fill in the details. Publications expand on click to show a summary.

### Adding news items (about.html)
Copy any `.news-item` block and update the date, text, and link.

### Global styles
Edit `style.css` to change fonts, colours, spacing, or layout across all pages.

---

## Custom domain (optional)

To use your own domain (e.g. `yourname.com`):
1. In your repo, create a file called `CNAME` with just your domain:
   ```
   yourname.com
   ```
2. Point your domain's DNS to GitHub Pages (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))
