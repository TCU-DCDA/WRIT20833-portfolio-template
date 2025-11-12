# Visual Guide: GitHub Collaboration for Portfolio Projects
## No Command Line Required!

This guide provides step-by-step instructions for using GitHub's web interface to create and collaborate on your portfolio.

---

## What You'll Learn

✅ How to create your portfolio from the template
✅ How to edit HTML directly on GitHub
✅ How to upload images
✅ How to collaborate with your group
✅ How to publish with GitHub Pages

**What you need:**
- A GitHub account (free)
- PNG files from your Google Colab notebooks
- Your research content ready to add

---

## 🚨 GROUPS: Start Here First!

**If you're working in a group, read this section BEFORE creating your repository!**

### Step 0: Designate Repository Owner (Group Work)

**⚠️ IMPORTANT: Only ONE person creates the repository**

**Group decision time:**

```
Your group needs to choose ONE person to:
✅ Create the repository from the template
✅ Own the repository on their GitHub account
✅ Add everyone else as collaborators
```

**Who should be the repository owner?**

Good choices:
- The person most comfortable with GitHub
- Your designated "web developer" for the project
- Someone who will stay organized and responsive
- Anyone willing to be the main point of contact

**What happens:**

```
Step 1: Repository Owner creates repo from template
   ↓
Step 2: Repository Owner adds teammates as collaborators
   ↓
Step 3: Everyone else receives invitation email
   ↓
Step 4: Everyone accepts invitation
   ↓
Step 5: Everyone clones the repository
   ↓
Step 6: Team works together!
```

**Repository will live at:**
- `https://github.com/OWNER-USERNAME/project-name`
- Example: `https://github.com/alexchen/twitter-sentiment-analysis`

**Note:** Even though it's on one person's account, **everyone has full edit access** once added as collaborators!

**✅ Once you've chosen your repository owner, that person continues to Step 1 below.**

---

## Step 1: Use the Template

### Creating Your Portfolio Repository

**Where to start:** https://github.com/TCU-DCDA/WRIT20833-portfolio-template

**What you'll see:**
```
┌─────────────────────────────────────────────────┐
│  TCU-DCDA / WRIT20833-portfolio-template        │
│  [Use this template ▼]  [Code ▼]  [Fork]       │
└─────────────────────────────────────────────────┘
```

**What to do:**

1. Click the green **"Use this template"** button
2. Select **"Create a new repository"**

**Visual cue:** Look for the green button at the top right of the page!

---

## Step 2: Name Your Repository

### Fill in Repository Details

**What you'll see:**

```
Create a new repository from WRIT20833-portfolio-template

Owner: [your-username] ▼
Repository name: [_________________]
Description (optional): [_________________]

○ Public    ○ Private

[✓] Include all branches

        [Create repository from template]
```

**What to enter:**

- **Repository name:** `twitter-sentiment-analysis` (use your project name)
- **Description:** "Analysis of sentiment patterns in climate change discourse"
- **Public/Private:** Select **Public** ⚠️ (Required for GitHub Pages!)

**Then:** Click **"Create repository from template"**

---

## Step 3: Your New Repository

### What You Just Created

**You now have your own copy!**

```
┌─────────────────────────────────────────────────┐
│  your-username / twitter-sentiment-analysis     │
│  Public                                         │
├─────────────────────────────────────────────────┤
│  📁 css/                                        │
│  📁 images/                                     │
│  📄 .gitignore                                  │
│  📄 index.html           ← This is what you edit│
│  📄 README.md                                   │
│  📄 QUICK_START.md                              │
└─────────────────────────────────────────────────┘
```

**Next step:** Edit `index.html` to add your content

---

## Step 4: Edit HTML on GitHub

### How to Edit Files Directly on GitHub

**Method 1: Click the pencil icon**

1. Click on `index.html` in the file list
2. Look for the ✏️ (pencil) icon at the top right
3. Click it to enter edit mode

**Method 2: Press the `.` (period) key**
- Opens web-based VS Code editor (advanced)

**Visual guide:**
```
┌─────────────────────────────────────────────────┐
│  index.html                      [✏️ Edit] [...]│
│  207 lines (8 KB)                               │
├─────────────────────────────────────────────────┤
│  1  <!DOCTYPE html>                             │
│  2  <html lang="en">                            │
│  3  <head>                                      │
```

**Click the ✏️ pencil icon!**

---

## Step 5: Make Your Edits

### What to Change in index.html

**Look for these placeholder texts:**

```html
<title>Your Project Title | WRIT 20833</title>
       ↓ Change to ↓
<title>Twitter Climate Sentiment | WRIT 20833</title>
```

```html
<h1>Your Project Title</h1>
<p>Your Name | WRIT 20833 | Fall 2025</p>
       ↓ Change to ↓
<h1>Climate Change Discourse Analysis</h1>
<p>Jane Smith | WRIT 20833 | Fall 2025</p>
```

**Pro tip:** Use browser's Find & Replace
- Press `Ctrl+F` (Windows) or `Cmd+F` (Mac)
- Type `Your Name` → Replace with your actual name
- Type `Your Project Title` → Replace with your title

---

## Step 6: Add Your Content

### Finding the TODO Markers

**Scroll through index.html and look for:**

```html
<!-- TODO: Add your research question here -->
<p>What patterns emerge when we analyze
   [your cultural phenomenon]?</p>
```

**Replace the example with YOUR content:**

```html
<!-- TODO: Add your research question here -->
<p>What patterns of sentiment emerge in climate
   change discourse on Twitter between 2020-2024?</p>
```

**Keep the HTML tags!** Only change the text between `>` and `<`

---

## Step 7: Commit Your Changes

### Saving Your Edits to GitHub

**Scroll to bottom of edit page:**

```
┌─────────────────────────────────────────────────┐
│  Commit changes                                 │
├─────────────────────────────────────────────────┤
│  Commit message:                                │
│  [Add research question and project title____]  │
│                                                 │
│  Extended description (optional):               │
│  [_________________________________________]    │
│                                                 │
│  ○ Commit directly to the main branch          │
│  ○ Create a new branch for this commit         │
│                                                 │
│         [Cancel]  [Commit changes]              │
└─────────────────────────────────────────────────┘
```

**What to do:**
1. Write a clear commit message: "Add research question and background"
2. Select "Commit directly to the main branch"
3. Click **"Commit changes"**

---

## Step 8: Upload Visualizations

### Adding PNG Files from Google Colab

**First: Export from Google Colab**

```python
import matplotlib.pyplot as plt

# After creating your chart:
plt.savefig('sentiment-distribution.png',
            dpi=300, bbox_inches='tight')

# In Colab: Files tab → Right-click → Download
```

**Then: Upload to GitHub**

1. Click into **`images/`** folder in your repository
2. Click **"Add file"** → **"Upload files"**
3. Drag PNG files into the upload box
4. Write commit message: "Add sentiment visualizations"
5. Click **"Commit changes"**

---

## Step 9: Upload Process Visual

### What the Upload Screen Looks Like

```
┌─────────────────────────────────────────────────┐
│  Add files to images/                           │
├─────────────────────────────────────────────────┤
│                                                 │
│      ┌─────────────────────────────────┐       │
│      │  Drag files here to add them    │       │
│      │  to your repository             │       │
│      │                                 │       │
│      │  or choose your files           │       │
│      └─────────────────────────────────┘       │
│                                                 │
├─────────────────────────────────────────────────┤
│  Commit changes                                 │
│  [Add sentiment visualizations_______________]  │
│                                                 │
│         [Cancel]  [Commit changes]              │
└─────────────────────────────────────────────────┘
```

**Tip:** You can drag multiple PNG files at once!

---

## Step 10: Add Collaborators (Group Work)

### Setting Up Team Access

**⚠️ This step is done by the REPOSITORY OWNER only**

**Go to:** Settings tab → Collaborators (left sidebar)

```
┌─────────────────────────────────────────────────┐
│  Collaborators                                  │
├─────────────────────────────────────────────────┤
│  Manage access                                  │
│                                                 │
│  [Add people_______________________________] 🔍 │
│                                                 │
│  Collaborators have read and write access      │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Steps:**
1. Click **"Add people"**
2. Enter teammate's **GitHub username** (not email!)
3. Click **"Add [username] to this repository"**
4. They'll receive an email invitation
5. Repeat for all group members

**After adding collaborators:**
- Tell your teammates to check their email
- They must **accept the invitation** to get access
- Then everyone can proceed to clone the repository

---

## Step 11: Clone to GitHub Desktop (Group Work)

### Getting the Repository on Your Computer

**⚠️ IMPORTANT: ALL team members do this step (including the owner)**

**After accepting the collaborator invitation:**

**In GitHub Desktop:**

1. Open GitHub Desktop
2. File → Clone Repository
3. Find the repository: `owner-username/project-name`
   - **Note:** Look for the OWNER's username, not yours!
   - Example: `alexchen/twitter-sentiment-analysis`
4. Choose where to save it on your computer
5. Click **"Clone"**

**What this does:**
- Downloads the entire repository to your computer
- Keeps it connected to GitHub
- Allows you to pull updates and push changes

**Visual:**
```
┌─────────────────────────────────────────────────┐
│  Clone a Repository                             │
├─────────────────────────────────────────────────┤
│  GitHub.com                                     │
│  ┌───────────────────────────────────────────┐ │
│  │ 🔍 Filter your repositories                │ │
│  │                                            │ │
│  │ your-username/twitter-sentiment-analysis  │ │
│  │ your-username/other-project               │ │
│  └───────────────────────────────────────────┘ │
│                                                 │
│  Local Path:                                    │
│  [/Users/you/Documents/GitHub]  [Choose...]    │
│                                                 │
│                    [Cancel]  [Clone]            │
└─────────────────────────────────────────────────┘
```

---

## Step 13: Coordination Strategy (Group Work)

### The Golden Rule: **PULL → EDIT → COMMIT → PUSH**

**⚠️ CRITICAL: Always pull before editing!**

### The Pull-Before-Edit Workflow

**Every time before you start working:**

```
Step 1: PULL (Get latest changes)
   ↓
Step 2: EDIT (Make your changes)
   ↓
Step 3: COMMIT (Save with message)
   ↓
Step 4: PUSH (Send to GitHub)
```

**In GitHub Desktop:**

```
┌─────────────────────────────────────────────────┐
│  Current Repository: twitter-sentiment-analysis │
├─────────────────────────────────────────────────┤
│  Current Branch: main                           │
│                                                 │
│  [Fetch origin]  ← Click this FIRST            │
│                                                 │
│  ↓ If there are changes:                       │
│                                                 │
│  [Pull origin]   ← Then click this             │
└─────────────────────────────────────────────────┘
```

### File Locking Strategy: "Claim Your Section"

**⚠️ Problem:** Two people editing `index.html` at the same time = merge conflict!

**✅ Solution: Section-Based Workflow**

**Before editing, announce in your group chat:**

```
👤 Alex: "Claiming Research Question section - editing now"
👤 Blake: "OK! I'll do Methods section next"
👤 Casey: "Great! I'll wait and then do Results"
```

**While someone is editing:**

```
👤 Alex: [Currently editing]
👤 Blake: [Waiting - maybe working on visualization code]
👤 Casey: [Waiting - maybe preparing content in Google Doc]
```

**After editing:**

```
👤 Alex: "Done with Research Question! Committed & pushed."
👤 Blake: "Thanks! Pulling now... Starting Methods section"
```

### Communication Templates

**Starting work:**
```
"Pulling latest changes now"
"Editing [section name] - will take ~15 minutes"
"Working on index.html - don't edit until I push"
```

**Finishing work:**
```
"Committed and pushed [section name]"
"Done! Safe to pull and edit now"
"Pushed my changes - please pull before you start"
```

**Coordination:**
```
"Can you wait 10 min? Almost done with my section"
"I'll edit after you push"
"Let's both work on visualizations - different files, no conflict!"
```

**Tools for coordination:**
- Slack / Discord / GroupMe
- Text message group chat
- Zoom/Google Meet call while working

---

## Step 14: Division of Labor (Group Work)

### Suggested Section Assignments

**For a 3-person group:**

```
📝 Person A:
   • Research Question (index.html lines 45-60)
   • Background Context (lines 65-80)
   • Pull → Edit → Commit → Push (Session 1)

📊 Person B:
   • Data & Methods (index.html lines 85-120)
   • Results & Analysis (lines 125-160)
   • Pull → Edit → Commit → Push (Session 2)

💭 Person C:
   • Key Findings (index.html lines 165-180)
   • Critical Reflection (lines 185-220)
   • Pull → Edit → Commit → Push (Session 3)
```

**Upload images strategy:**
- Person with best visualization should upload all images at once
- Coordinate: "I'm uploading all 5 images now"
- Others: Pull after images are pushed

**For a 2-person group:**
```
📝 Person A: 
   • Research Question, Background, Reflection
   • Session 1: Pull → Edit top sections → Push
   
📊 Person B: 
   • Data & Methods, Results, Findings
   • Session 2: Pull → Edit middle sections → Push
   • Upload all images in Session 3
```

**Everyone:** Review final portfolio together before submitting!

---

## Step 15: Handling Merge Conflicts (Group Work)

### Prevention is Best!

**✅ Best practices to AVOID conflicts:**

1. **Always pull before editing** (most important!)
2. **Communicate in real-time** (Slack/Discord/text)
3. **Work on different sections** (claim your section)
4. **Push immediately after finishing** (don't wait days)
5. **Don't edit on GitHub.com AND Desktop simultaneously**

### What If a Conflict Happens?

**You'll see this in GitHub Desktop:**

```
┌─────────────────────────────────────────────────┐
│  ⚠️ Resolve Conflicts                           │
├─────────────────────────────────────────────────┤
│  1 conflicted file                              │
│                                                 │
│  index.html                                     │
│  [Open in Visual Studio Code]                   │
│                                                 │
│  After resolving, commit the merge.            │
└─────────────────────────────────────────────────┘
```

**Step-by-step resolution:**

**1. Don't panic!** Your work isn't lost.

**2. Open the conflicted file** (click "Open in Visual Studio Code" or your text editor)

**3. Look for conflict markers:**
```html
<<<<<<< HEAD
<p>Alex's version of this paragraph</p>
=======
<p>Blake's version of this paragraph</p>
>>>>>>> main
```

**4. Decide what to keep:**

Option A: Keep Alex's version (delete Blake's)
```html
<p>Alex's version of this paragraph</p>
```

Option B: Keep Blake's version (delete Alex's)
```html
<p>Blake's version of this paragraph</p>
```

Option C: Combine both (best option!)
```html
<p>Alex's version with Blake's additions</p>
```

**5. Remove conflict markers** (`<<<<<<<`, `=======`, `>>>>>>>`)

**6. Save the file**

**7. In GitHub Desktop:**
   - File should now show as "Resolved"
   - Add commit message: "Resolved merge conflict in index.html"
   - Click "Commit to main"
   - Click "Push origin"

**8. Tell your group:** "Conflict resolved! Everyone pull now."

### Real-World Scenario

**What went wrong:**

```
👤 Alex: Pulled at 2:00 PM, started editing
👤 Blake: Pulled at 2:05 PM, started editing same file
👤 Alex: Pushed changes at 2:20 PM ✅
👤 Blake: Tries to push at 2:25 PM ❌ CONFLICT!
```

**How to fix:**

```
👤 Blake: "I got a conflict - one sec"
         [Opens index.html in editor]
         [Sees both versions]
         [Keeps both, removes markers]
         [Commits: "Resolved conflict - kept both sections"]
         [Pushes]
👤 Blake: "Fixed! Everyone pull latest version"
👤 Alex: "Got it!" [Pulls]
👤 Casey: "Pulled!" [Pulls]
```

### When to Ask for Help

**❌ DON'T try to resolve if:**
- You're not sure which version is correct
- Multiple files have conflicts
- The conflict involves code you didn't write

**✅ DO ask instructor/TA if:**
- You get conflicts on multiple files
- You're confused about what to keep
- The conflict involves HTML structure (not just content)

**In office hours, bring:**
- Screenshot of GitHub Desktop conflict view
- The conflicted file open in text editor
- Timeline of who edited when

---

## Step 16: Preview Your Work

### Checking Your Portfolio Before Publishing

**Option 1: View on GitHub (limited preview)**
- Just see the HTML code, not the styled page

**Option 2: Open locally from GitHub Desktop**

1. In GitHub Desktop, right-click your repository
2. Select "Open in Visual Studio Code" (or your preferred editor)
3. Open `index.html`
4. Right-click the file and "Open with Live Server" (if you have the extension)
5. Or just double-click `index.html` in Finder/Explorer

**Option 3: Enable GitHub Pages (see next step)**

---

## Step 17: Enable GitHub Pages

### Publishing Your Portfolio to the Web

**Go to:** Settings tab → Pages (left sidebar)

```
┌─────────────────────────────────────────────────┐
│  GitHub Pages                                   │
├─────────────────────────────────────────────────┤
│  Source                                         │
│  [Deploy from a branch ▼]                       │
│                                                 │
│  Branch                                         │
│  [main ▼]  [/ (root) ▼]      [Save]           │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Steps:**
1. Source: Select **"Deploy from a branch"**
2. Branch: Select **"main"**
3. Folder: Select **"/ (root)"**
4. Click **"Save"**

---

## Step 18: Get Your URL

### Your Portfolio Is Live!

**After 1-2 minutes, refresh the Settings → Pages page:**

```
┌─────────────────────────────────────────────────┐
│  ✅ Your site is live at                        │
│                                                 │
│  https://your-username.github.io/               │
│         twitter-sentiment-analysis/             │
│                                                 │
│         [Visit site]                            │
└─────────────────────────────────────────────────┘
```

**This is your portfolio URL!**

✅ Submit this link for your assignment
✅ Share with your group to review
✅ Include in your resume/CV
✅ Show to future employers

---

## Troubleshooting

### Images Not Showing

**What you see on your portfolio:**
```
┌─────────────────┐
│  🖼️ [broken]    │
│  Figure 1: ...  │
└─────────────────┘
```

**Causes & Solutions:**

❌ **Wrong filename:** `sentiment-chart.png` ≠ `Sentiment-Chart.PNG`
✅ **Solution:** Check exact filename in `images/` folder

❌ **Wrong path:** `/images/chart.png` or `Images/chart.png`
✅ **Solution:** Use `images/chart.png` (lowercase, relative path)

❌ **File not uploaded**
✅ **Solution:** Check `images/` folder - is your PNG there?

❌ **Browser cache**
✅ **Solution:** Hard refresh: `Ctrl+Shift+R` or `Cmd+Shift+R`

---

### GitHub Pages Not Working

**What you see when visiting your URL:**
```
┌─────────────────────────────────────────────────┐
│              404                                │
│  There isn't a GitHub Pages site here.         │
└─────────────────────────────────────────────────┘
```

**Checklist:**

- [ ] Repository is **Public** (not Private)
- [ ] Waited 2-3 minutes after enabling Pages
- [ ] Hard refreshed browser (`Ctrl+Shift+R`)
- [ ] Pages is enabled: Settings → Pages → Source = "main"
- [ ] `index.html` is in root folder (not in subfolder)
- [ ] Visiting correct URL (includes repository name)

**If still not working:** Ask in office hours with screenshot!

---

## Best Practices

### Tips for Success

**✅ DO:**
- ✅ Write clear commit messages ("Add methods section" not "update")
- ✅ Communicate with group before editing
- ✅ Refresh page before editing to see latest changes
- ✅ Test in browser before final submission
- ✅ Use descriptive filenames (`sentiment-chart.png` not `chart1.png`)

**❌ DON'T:**
- ❌ Edit at same time as teammate
- ❌ Use vague commit messages ("asdf" or "changes")
- ❌ Upload images to wrong folder
- ❌ Make repository Private (GitHub Pages won't work)
- ❌ Delete files you're not sure about

---

## Workflow Summary

### Complete Process at a Glance

**Individual Projects:**

```
1. Use Template → Create Repository
         ↓
2. Edit index.html (click ✏️ pencil)
         ↓
3. Commit changes (with clear message)
         ↓
4. Upload images to images/ folder
         ↓
5. Enable GitHub Pages (Settings → Pages)
         ↓
6. Wait 2 minutes → Visit your URL
         ↓
7. Test and review
         ↓
8. Submit GitHub Pages URL
```

---

### Group Projects Workflow

**Complete Process for Teams:**

```
1. ONE PERSON: Use template, create repository
         ↓
2. ADD COLLABORATORS (Settings → Collaborators)
         ↓
3. DIVIDE SECTIONS (coordinate on chat)
         ↓
4. PERSON A: Edit section, commit
         ↓
5. PERSON B: Edit section, commit (wait for A)
         ↓
6. PERSON C: Edit section, commit (wait for B)
         ↓
7. ONE PERSON: Upload all images
         ↓
8. REVIEW TOGETHER before enabling Pages
         ↓
9. Enable Pages, test, submit
```

**Communication is key!** 📱

---

## Resources

### Where to Get Help

**📖 Documentation in Template:**
- `README.md` - Complete guide
- `QUICK_START.md` - Fast reference
- `WEB_WORKFLOW.md` - Detailed walkthrough

**🆘 When You Need Help:**
- Check Troubleshooting sections in README
- Post screenshot in Canvas discussion
- Attend office hours
- Ask your group members
- Test in different browser

**🔗 External Resources:**
- GitHub Pages docs: https://docs.github.com/pages
- HTML reference: https://developer.mozilla.org/docs/Web/HTML

---

## Quick Start Checklist

### Getting Started Today

**What you learned:**
✅ Create portfolio from template (no code!)
✅ Edit HTML on GitHub (just click ✏️)
✅ Upload visualizations (drag & drop)
✅ Collaborate with group (take turns!)
✅ Publish with GitHub Pages (Settings → Pages)

**What you DON'T need:**
❌ Command line / Terminal
❌ Git software
❌ VS Code (optional but not required)
❌ Advanced technical skills

**Your browser can do everything!** 🌐

---

## Quick Reference Card

### One-Page Cheat Sheet

**Create Repository:**
- Use this template → Name it → Make Public → Create

**Edit File:**
- Click file → Click ✏️ → Edit → Commit with message

**Upload Images:**
- Click `images/` → Add file → Upload → Drag PNGs → Commit

**Add Collaborators (Groups):**
- Settings → Collaborators → Add people → Enter username

**Coordinate (Groups):**
- Message: "Editing [section] now"
- Wait for teammate to commit
- Refresh before you start editing

**Enable GitHub Pages:**
- Settings → Pages → Deploy from `main` → Save

**Troubleshoot:**
- Images: Check filename matches exactly
- 404: Make sure repo is Public, wait 2 min
- Conflict: Copy your text, refresh, try again

---

**Template:** https://github.com/TCU-DCDA/WRIT20833-portfolio-template

**Questions?** See README.md or attend office hours!
