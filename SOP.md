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
   - Press `Ctrl+ ~(backtick)` or `View` → `Terminal`
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

#### 📄 **How to Update Your CV PDF:**
**If you want to upload a new CV PDF file:**

1. **Add your new PDF file**:
   - Place your new CV PDF in the `assets/pdf/` folder
   - **Recommended naming**: `Yukun-Ma-CV-v5.pdf` (increment the version number)

2. **Update the CV page link**:
   - Open the file: `_pages/cv.md`
   - Find the line: `cv_pdf: Yukun-Ma-CV-v4.pdf`
   - Change it to: `cv_pdf: Yukun-Ma-CV-v5.pdf` (or your new filename)
   - **Save the file**

3. **Optional - Clean up old files**:
   - You can delete old CV versions from `assets/pdf/` folder if desired
   - Keep at least the current version referenced in `cv.md`

**Example**: If your new CV is named `Yukun-Ma-CV-v5.pdf`, your `_pages/cv.md` should look like:
```
cv_pdf: Yukun-Ma-CV-v5.pdf
```

#### 👤 **How to Update Your About Page:**
**To update your personal information, bio, or profile:**

**File to edit**: `_pages/about.md`

**Common updates**:
1. **Personal info** (top section):
   - Phone number: `<p>+1 (615) 710-7851</p>`
   - Email: `<p><a href="mailto:...">your.email@domain.com</a></p>`
   - Address: `<p>225 Harkness Hall</p>`
   - Google Scholar: `<p> <a href="...">Google Scholar</a></p>`

2. **Bio text** (main content):
   - Update the paragraphs below the `---` section
   - Describe your current position, research interests, achievements

3. **Profile picture**:
   - Add new photo to `assets/img/` folder
   - Update: `image: your-new-photo.jpg`

**Example**: To change your bio, edit the text after the `---` line

#### 🔬 **How to Update Your Research Page:**
**To add new papers or update existing ones:**

**File to edit**: `_pages/research.md`

**To add a new paper**:
1. **Copy the format** of an existing paper section
2. **Update all details**:
   - Title in colored header: `#### <font color ="#263755">Your Paper Title</font>`
   - Co-authors with their website links
   - Journal/conference information
   - Abstract
   - Links to PDF, arXiv, Google Scholar

3. **Add PDF files**:
   - Put paper PDFs in `assets/pdf/` folder
   - Link them: `[PDF](/assets/pdf/Your-Paper.pdf)`

**To update existing papers**:
- Edit the relevant section with new information
- Update PDF links if you have new versions

#### 🎓 **How to Update Your Teaching Page:**
**To add new courses or update ratings:**

**File to edit**: `_pages/teaching.md`

**To add new courses**:
1. **Follow the existing format**:
   ```
   **University Name, Department**
   
   COURSE CODE: Course Name Semester Year (Rating/5)
   ```

2. **Example**:
   ```
   ECON 101: Introduction to Economics Spring 2025 (4.8/5)
   ```

**To update course ratings**:
- Find the course line and update the rating in parentheses

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
