# How to Push to GitHub

This guide will help you push the Cover Letter Generator to a **separate GitHub repository** (keeping it distinct from your NOC Generation tool).

## Step 1: Create a New GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the **"+"** icon in top right → **New repository**
3. Fill in the details:
   - **Repository name**: `company-cover-letter-generator`
   - **Description**: `Professional cover letter generator with multiple design templates`
   - **Public/Private**: Choose based on preference
   - **Add .gitignore**: No (we already have one)
   - **Add license**: MIT (recommended)

4. Click **Create repository**

You'll see a page with commands to initialize your repository.

---

## Step 2: Initialize and Push (Command Line)

### If this is a NEW repository (first time):

Open terminal/command prompt and navigate to the project folder:

```bash
cd cover-letter-generator
```

Initialize Git:

```bash
git init
```

Add the remote repository:

```bash
git remote add origin https://github.com/YOUR-USERNAME/company-cover-letter-generator.git
```

(Replace `YOUR-USERNAME` with your actual GitHub username)

Stage all files:

```bash
git add .
```

Create first commit:

```bash
git commit -m "Initial commit: Cover Letter Generator with 5 design templates"
```

Push to GitHub:

```bash
git branch -M main
git push -u origin main
```

---

## Step 3: For Future Updates

After making changes, use these commands to push updates:

```bash
git add .
git commit -m "Description of changes"
git push
```

---

## Step 4: Set Up GitHub Pages (Optional - for Live Demo)

If you want a live demo link:

1. Go to your GitHub repository
2. Click **Settings** tab
3. Scroll to **Pages** section (left sidebar)
4. Under "Source", select **main** branch
5. Click **Save**
6. Your site will be live at: `https://YOUR-USERNAME.github.io/company-cover-letter-generator`

---

## Step 5: Use with Claude Code

To use this with Claude Code (like your NOC tool):

### Option A: Clone the Repository
```bash
git clone https://github.com/YOUR-USERNAME/company-cover-letter-generator.git
cd company-cover-letter-generator
```

### Option B: Open in Claude Code
1. Open Claude Code
2. Start a new chat for this project
3. Paste: `https://github.com/YOUR-USERNAME/company-cover-letter-generator`
4. Claude Code will handle cloning and setup

---

## Important: Keeping Projects Separate

✅ **Your NOC Tool** → Original repository
✅ **Cover Letter Generator** → This NEW repository (separate)

They have:
- Different GitHub repos
- Different project folders
- Different Git histories
- Different Claude Code chats (if using Claude Code)

**They will NOT merge** as long as you:
1. Create a separate GitHub repository
2. Keep them in separate local folders
3. Use separate Claude Code chats

---

## Troubleshooting

### "Remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/YOUR-USERNAME/cover-letter-generator.git
```

### "Permission denied (publickey)"
You need to set up SSH keys. Instead, use HTTPS:
```bash
git remote set-url origin https://github.com/YOUR-USERNAME/cover-letter-generator.git
```

### "fatal: not a git repository"
Make sure you're in the correct folder:
```bash
cd cover-letter-generator
```

### Need to update from GitHub locally
```bash
git pull origin main
```

---

## Project Organization

Suggested folder structure on your computer:

```
Projects/
├── noc-generator/                 (Your existing NOC tool)
│   └── .git
├── company-cover-letter-generator/ (This new tool)
│   └── .git
```

Each has its own `.git` folder and GitHub repository.

---

## Next Steps

After pushing to GitHub:

1. ✅ Repository is now backed up
2. ✅ Can be cloned anywhere
3. ✅ Can share link with others
4. ✅ Ready to use with Claude Code
5. ✅ Can set up GitHub Pages for live demo

---

**Questions?** The tool works completely offline - all data stays in your browser. No authentication or external services needed!
