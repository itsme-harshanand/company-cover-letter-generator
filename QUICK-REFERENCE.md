# Quick Reference: Push to GitHub

## 1️⃣ Create Repo on GitHub.com

Go to: https://github.com/new
- Repository name: `company-cover-letter-generator`
- Description: `Professional cover letter generator with multiple design templates`
- License: MIT
- Click: **Create repository**

Copy the HTTPS URL you get (looks like: `https://github.com/YOUR-USERNAME/company-cover-letter-generator.git`)

---

## 2️⃣ Push from Command Line

Open terminal, navigate to project folder:

```bash
cd /path/to/company-cover-letter-generator
```

Initialize and push:

```bash
git init
git add .
git commit -m "Initial commit: Professional Cover Letter Generator"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/company-cover-letter-generator.git
git push -u origin main
```

**Done!** ✅ Your code is now on GitHub.

---

## 3️⃣ Use in Claude Code

**Option 1: Clone & Work**
- Terminal: `git clone https://github.com/YOUR-USERNAME/company-cover-letter-generator.git`
- Open with Claude Code

**Option 2: Direct Open**
- New Claude Code chat
- Paste the GitHub URL
- Claude Code handles it

---

## 4️⃣ Keep Separate from NOC Tool

✅ Different GitHub repos
✅ Different local folders  
✅ Different Claude Code chats
✅ No merging/conflicts

---

## 5️⃣ Future Updates

After making changes:

```bash
git add .
git commit -m "Your changes description"
git push
```

---

## Files in This Project

```
company-cover-letter-generator/
├── index.html       (Main application - works standalone)
├── README.md        (Project description)
├── SETUP.md         (Detailed setup guide)
└── .gitignore       (Git ignore rules)
```

---

## 📱 Optional: GitHub Pages (Live Demo)

After pushing to GitHub:

1. Go to repo → **Settings** → **Pages**
2. Select **main** branch as source
3. Your site goes live at: `https://YOUR-USERNAME.github.io/company-cover-letter-generator`

Share that link for anyone to use the tool! 🌐

---

## ⚡ That's It!

Once you run the `git push` command, your project is on GitHub and separate from your NOC tool. You can work on both independently without any issues.

**The tool is production-ready** - no npm, no build steps, no dependencies. Just open `index.html` in any browser!
