# Quick Start Guide

## Two Ways to Work

### Option A: Web-Only Workflow (Quick Edits)

1. **Create your copy:**
   - Click green **"Use this template"** button at top
   - Name it: `your-project-name`
   - Make it **Public**
   - Click "Create repository from template"

2. **Edit HTML directly on GitHub:**
   - Click `index.html` in your new repository
   - Click the ✏️ (pencil icon) at top right
   - Find `Your Name` and replace with your actual name
   - Find `Your Project Title` and replace with your title
   - Scroll to `<!-- TODO: ... -->` comments and add your content
   - Scroll down and click **"Commit changes"**

3. **Upload visualizations:**
   - Click into `images/` folder
   - Click "Add file" → "Upload files"
   - Drag PNG files from your computer
   - Click "Commit changes"

4. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Source: Deploy from branch `main`
   - Click Save
   - Your site will be live at: `YOUR-USERNAME.github.io/your-project-name`

### Option B: GitHub Desktop Workflow (Recommended for Groups)

**Best for:** Group projects, frequent edits, working offline

1. **Create your copy first:**
   - Click green **"Use this template"** button at top
   - Name it: `your-project-name`
   - Make it **Public**
   - Click "Create repository from template"

2. **Clone with GitHub Desktop:**
   - Click green "Code" button → "Open with GitHub Desktop"
   - Choose where to save on your computer
   - Click "Clone"

3. **Edit in text editor:**
   - Right-click repository in GitHub Desktop → "Open in Visual Studio Code" (or your preferred editor)
   - Open `index.html` and use Find & Replace (Ctrl+F / Cmd+F):
     - Replace `Your Name` → Your actual name
     - Replace `Your Project Title` → Your project title
     - Replace `yourusername` → Your GitHub username

4. **Fill in content:**
   - Look for `<!-- TODO: ... -->` comments
   - Replace with your research content

5. **Add images:**
   - Export visualizations from Google Colab as PNG
   - Save to `images/` folder in your local repository

6. **Commit and push changes:**
   - Go to GitHub Desktop
   - Add commit message (e.g., "Added my content and visualizations")
   - Click "Commit to main"
   - Click "Push origin" to sync to GitHub

7. **Enable GitHub Pages:**
   - Go to Settings → Pages on GitHub
   - Source: Deploy from branch `main`
   - Click Save
   - Your site will be live at: `YOUR-USERNAME.github.io/your-project-name`

## Key Sections to Fill In

| Section | What to Add |
|---------|-------------|
| **Research Question** | Your question + background context |
| **Data & Methods** | Dataset details, collection method, tools used |
| **Analysis** | Visualizations + code examples + explanations |
| **Findings** | Key discoveries + data tables |
| **Reflection** | Framework connections + limitations + future work |

## Common Edits

### Change Colors
Edit `css/styles.css` at the top:
```css
:root {
    --primary-color: #4d1979;      /* Change this */
    --secondary-color: #7c3aed;    /* And this */
}
```

### Add More Sections
Copy an existing section and change the ID:
```html
<section id="newsection">
    <h2>New Section Title</h2>
    <p>Content here...</p>
</section>
```

Don't forget to add it to navigation!

### Add More Visualizations
Copy the figure block:
```html
<figure class="viz-container">
    <img src="images/your-chart.png" alt="Description of chart">
    <figcaption>Figure X: Your caption here</figcaption>
</figure>
```

## Checklist

- [ ] Personalized title and name
- [ ] Filled in all TODO sections
- [ ] Added visualizations to `images/`
- [ ] Updated image paths in HTML
- [ ] Added GitHub repo link
- [ ] Tested in browser
- [ ] Ready to deploy!

## Need Help?

- **Full documentation:** See `README.md`
- **CSS reference:** See workshop Session 2
- **HTML structure:** See workshop Session 1
- **Examples:** See workshop Session 3

---

**Remember:** The CSS is complete—you only need to edit `index.html` content!
