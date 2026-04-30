# Claude Code Automation Guide

## Automatic Deployment on Every Push

This project is set up with **GitHub Actions** that automatically deploy changes to the live site whenever you push code.

---

## 🚀 How Automatic Updates Work

1. **You make changes** in Claude Code
2. **You push to GitHub** (`git push`)
3. **GitHub Actions** automatically runs
4. **Site updates** within 30 seconds at: `https://itsme-harshanand.github.io/company-cover-letter-generator`

**No manual deployment needed!**

---

## 📝 Claude Code Workflow

### Step 1: Clone the Repository

```bash
git clone https://github.com/itsme-harshanand/company-cover-letter-generator.git
cd company-cover-letter-generator
```

### Step 2: Make Changes in Claude Code

For example, to modify `index.html`:

```
Claude, please:
1. Open index.html
2. Find the section with "export-buttons"
3. Change the button text or styling as needed
4. Save the file
```

Or simply edit files directly:
- Edit `index.html` for layout/functionality changes
- Edit `README.md` for documentation updates
- Edit styles or add new features

### Step 3: Commit and Push

After making changes, push to GitHub:

```bash
git add .
git commit -m "Describe your changes: Add feature X or Fix bug Y"
git push origin main
```

### Step 4: Automatic Deployment (Magic ✨)

GitHub Actions will automatically:
- ✅ Detect your push
- ✅ Run deployment checks
- ✅ Update the live site
- ✅ Complete within 30 seconds

**Your changes are now LIVE!** Visit: `https://itsme-harshanand.github.io/company-cover-letter-generator`

---

## 🔧 Common Claude Code Prompts

### Add a New Feature

```
I want to add [feature] to the Cover Letter Generator.

Currently it [does X].

I need it to also [do Y].

Please modify the code in index.html to:
1. [Change/add specific functionality]
2. [Update styling if needed]
3. [Test the changes]

Then commit with message: "Add [feature]"
And push to GitHub.
```

### Fix a Bug

```
There's a bug where [description].

Please:
1. Find the problematic code in index.html
2. Fix the issue
3. Test it
4. Commit with: "Fix: [bug description]"
5. Push to GitHub
```

### Change Design/Colors

```
Please update the design templates in index.html:
1. Change the colors from [old colors] to [new colors]
2. Update the styling for [specific elements]
3. Test all 5 templates with Shuffle button
4. Commit: "Update: [changes made]"
5. Push
```

### Add New Template

```
I want to add a 6th design template called "[name]".

Please:
1. Create new CSS class in styles
2. Add styling with:
   - [specific colors/fonts/layout details]
3. Add to templates array in JavaScript
4. Test the shuffle button
5. Commit: "Add template: [name]"
6. Push
```

### Performance Optimization

```
Please optimize the index.html for performance:
1. Minimize CSS
2. Optimize JavaScript
3. Improve load times
4. Commit: "Perf: Optimize code"
5. Push
```

---

## 📊 Monitor Deployment Status

Check if your changes deployed successfully:

1. Go to: `https://github.com/itsme-harshanand/company-cover-letter-generator/actions`
2. You'll see recent deployments with ✅ or ❌ status
3. Click on any deployment to see logs

---

## 🔄 Continuous Workflow

### Typical Development Cycle

1. **Open Claude Code**
   ```bash
   git clone https://github.com/itsme-harshanand/company-cover-letter-generator.git
   cd company-cover-letter-generator
   ```

2. **Tell Claude what to change**
   ```
   Please modify [file] to [do something]
   Then git commit and push
   ```

3. **Claude Code handles it all:**
   - ✅ Makes the changes
   - ✅ Commits with message
   - ✅ Pushes to GitHub
   - ✅ GitHub Actions deploys automatically

4. **Live site updates instantly**

---

## 🎯 Multi-Level Automation

### Level 1: Manual Control
```bash
git add .
git commit -m "Your message"
git push
# GitHub Actions automatically deploys
```

### Level 2: Claude Code Automation
```
Tell Claude: "Make [change] and push to GitHub"
# Claude handles everything including git commands
```

### Level 3: GitHub Actions
```
When you push, GitHub automatically:
- Runs tests (if configured)
- Deploys to live site
- Updates documentation
```

---

## 🚨 Troubleshooting

### Changes not showing on live site?

1. **Hard refresh browser** (Ctrl+Shift+R or Cmd+Shift+R)
2. **Check deployment status** at `/actions` page
3. **Wait 30 seconds** - GitHub Actions needs time
4. **Check browser console** for errors (F12)

### Deployment failed?

1. Go to: `https://github.com/itsme-harshanand/company-cover-letter-generator/actions`
2. Click the failed deployment
3. Read the error message
4. Ask Claude to fix the issue based on the error

### Git conflicts?

```bash
git pull origin main
# Resolve conflicts
git add .
git commit -m "Resolve conflicts"
git push
```

---

## 💡 Best Practices

1. **Write clear commit messages**
   ```bash
   ❌ git commit -m "changes"
   ✅ git commit -m "Add PDF export functionality"
   ```

2. **Test locally first**
   - Open index.html in browser
   - Test features before pushing
   - Use console (F12) to check for errors

3. **One change per commit**
   ```bash
   ❌ git commit -m "Fix colors, add feature, update text"
   ✅ git commit -m "Update theme colors"
   # Then separate commit for feature
   ```

4. **Push frequently**
   - Small, frequent pushes are safer
   - Easier to debug if something breaks

---

## 📚 Quick Reference

| Task | Command |
|------|---------|
| Clone repo | `git clone https://github.com/itsme-harshanand/company-cover-letter-generator.git` |
| Check status | `git status` |
| Stage changes | `git add .` |
| Commit | `git commit -m "Description"` |
| Push | `git push origin main` |
| Pull latest | `git pull origin main` |
| View log | `git log --oneline` |
| Undo last commit | `git reset HEAD~1` |

---

## 🎉 Summary

**You now have a fully automated deployment system:**

✅ Edit code locally in Claude Code  
✅ Commit and push when ready  
✅ GitHub Actions automatically deploys  
✅ Live site updates within 30 seconds  
✅ No manual steps needed  

**That's it!** Your workflow is completely automated. 🚀

---

## 🔗 Important Links

- **Live Site**: https://itsme-harshanand.github.io/company-cover-letter-generator
- **GitHub Repo**: https://github.com/itsme-harshanand/company-cover-letter-generator
- **Deployment Status**: https://github.com/itsme-harshanand/company-cover-letter-generator/actions
- **GitHub Actions Docs**: https://docs.github.com/en/actions

---

Need help? Ask Claude Code to make changes and push them automatically!
