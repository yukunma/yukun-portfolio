# 📋 Standard Operating Procedure (SOP)
## How to Update Your Portfolio Website

**Target Audience**: Non-technical users who need to update the website content

---

## 🚨 IMPORTANT: Read This First!

This guide assumes you have:
- ✅ The portfolio folder on your computer
- ✅ Terminal/Command Prompt access
- ✅ Basic familiarity with opening folders and files

**⚠️ Always follow these steps IN ORDER. Do not skip steps!**

---

## 📝 Step-by-Step Instructions

### Step 1: Open Project in VSCode
1. **Open VSCode** (Visual Studio Code)
2. **Open your portfolio folder**:
   - Click `File` → `Open Folder...`
   - Navigate to and select your `yukun-portfolio` folder
   - Click `Open`
3. **Open the integrated terminal**:
   - **Keyboard shortcut**: Press `Ctrl` + `` ` `` (the backtick key, upper-left of keyboard)
   - **OR menu**: Click `View` → `Terminal`
   - The terminal will automatically be in your project folder

### Step 2: Pull Latest Changes (ALWAYS DO THIS FIRST!)
**Why**: This ensures you have the most recent version before making changes

**Instructions**: Copy the command below and paste it into the terminal, then press Enter
```bash
git pull origin master
```
**Expected result**: You should see "Already up to date" or a list of updated files

### Step 3: Make Your Content Changes
1. **Open the files you need to edit** in VSCode
2. **Common files to edit**:
   - `_pages/about.md` - Your about page
   - `_data/cv.yml` - Your CV information
   - `_projects/` folder - Your projects
   - `_config.yml` - Site settings

#### � **Detailed Content Update Guides:**
Click on the links below for step-by-step instructions:

- 📄 **[How to Update Your CV PDF](SOP/update-cv-pdf.md)** - Upload new CV files and update links
- 👤 **[How to Update Your About Page](SOP/update-about-page.md)** - Personal info, bio, and profile picture
- 🔬 **[How to Update Your Research Page](SOP/update-research-page.md)** - Add new papers or update existing ones
- 🎓 **[How to Update Your Teaching Page](SOP/update-teaching-page.md)** - Add courses and update ratings

3. **Make your changes and SAVE the files**

### Step 4: Test Changes Locally (See Your Changes Before Publishing)
1. **Start the local server**:
   
   **Instructions**: Copy the command below and paste it into the terminal, then press Enter
   ```bash
   bundle exec jekyll serve --lsi
   ```
2. **Open your browser** and go to: `http://127.0.0.1:4000`
3. **Check your changes** - does everything look correct?
4. **When done checking**, press `Ctrl+C` in Terminal to stop the server

### Step 5: Stage All Changes
**What this does**: Tells Git which files you want to save

**Instructions**: Copy the command below and paste it into the terminal, then press Enter
```bash
git add .
```
**Note**: The period (.) means "add all changed files"

### Step 6: Commit Changes with a Message
**What this does**: Saves your changes with a description

**Instructions**: Choose ONE of the options below:

**Option A - Quick commit (uses today's date):**
Copy and paste this command into the terminal, then press Enter
```bash
git commit -m "Portfolio updates - $(date '+%Y-%m-%d')"
```

**Option B - Custom message:**
Copy the command below, **replace the message with your own description**, paste into terminal, then press Enter
```bash
git commit -m "Your description of what you changed"
```

**Examples of good custom messages**:
- `git commit -m "Updated about page with new research interests"`
- `git commit -m "Added new project: Machine Learning Research"`
- `git commit -m "Updated CV with latest publications"`

### Step 7: Push Changes to Website
**What this does**: Uploads your changes to make them live on the internet

**Instructions**: Copy the command below and paste it into the terminal, then press Enter
```bash
git push origin master
```
**Expected result**: You should see "Everything up-to-date" or a progress bar

---

## ✅ Success Checklist

After completing all steps, you should have:
- [ ] Pulled the latest changes
- [ ] Made your content edits
- [ ] Tested changes locally
- [ ] Added all changes to git
- [ ] Committed with a descriptive message
- [ ] Pushed changes to the live website

---

## 🚨 What If Something Goes Wrong?

### Problem: "Git command not found"
**Solution**: Git is not installed. Contact your technical support.

### Problem: "Permission denied" or "Access denied"
**Solution**: You may not have the right permissions. Contact your technical support.

### Problem: Local server won't start
**Solution**: 
1. Make sure you're in the right folder
2. Try running: `bundle install` first
3. Then try: `bundle exec jekyll serve --lsi` again

### Problem: Changes don't appear on the website
**Solution**: 
1. Wait 5-10 minutes (sometimes changes take time to appear)
2. Clear your browser cache and refresh
3. Check if you followed all steps correctly

---

## 📞 Need Help?

If you get stuck or see error messages:
1. **Take a screenshot** of the error
2. **Note which step** you were on
3. **Contact your technical support** with this information

---

## ⏰ Typical Timeline

- **Pulling latest changes**: 5-30 seconds
- **Making content edits**: 5-30 minutes (depends on changes)
- **Testing locally**: 1-2 minutes to start + review time
- **Git operations**: 30 seconds - 2 minutes total
- **Changes going live**: 5-10 minutes after pushing

**Total time**: Usually 15-45 minutes depending on the scope of your changes.
