# Yukun's Portfolio

A Jekyll-based academic portfolio website built on the al-folio theme.

## 🚀 Quick Commands for Local Development

Once you have the environment set up (see below), use these commands to work on your portfolio:

### Start Development Server
```bash
bundle exec jekyll serve --lsi
```
Your site will be available at `http://127.0.0.1:4000`

### View Local Changes
- The server automatically rebuilds when you make changes
- Refresh your browser to see updates
- Press `Ctrl+C` to stop the server



### Git Operations
```bash
# Check status and see changes
git status

# Add all changes
git add .

# Commit changes
git commit -m "Your commit message"

# Push to remote repository
git push origin master

# Pull latest changes
git pull origin master

# View commit history
git log --oneline
```

### Install New Dependencies
```bash
bundle install
```
---

## 🛠️ Initial Environment Setup

### Prerequisites
- macOS with Homebrew installed
- Terminal access

### Step 1: Install Ruby Version Manager
```bash
# Install rbenv and ruby-build
brew install rbenv ruby-build

# Add rbenv to your shell profile
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc

# Reload your shell
source ~/.zshrc
```

### Step 2: Install Ruby
```bash
# Install Ruby 3.1.6 (stable version compatible with Jekyll)
rbenv install 3.1.6

# Set as global default
rbenv global 3.1.6

# Verify installation
ruby --version  # Should show ruby 3.1.6
```

### Step 3: Install Dependencies
```bash
# Install Bundler
gem install bundler

# Install all Jekyll dependencies
bundle install
```

### Step 4: Start Development Server
```bash
bundle exec jekyll serve --lsi
```

Your portfolio will be running at `http://127.0.0.1:4000` 🎉

---

## 📁 Project Structure

- `_pages/` - Main site pages (about, CV, projects, etc.)
- `_posts/` - Blog posts
- `_projects/` - Project showcase items
- `_data/` - Data files (CV info, repositories, etc.)
- `_sass/` - Styling files
- `assets/` - Images, PDFs, and other assets
- `_config.yml` - Site configuration

---

## ✨ Customization Tips

1. **Personal Info**: Update `_config.yml` with your details
2. **About Page**: Edit `_pages/about.md`
3. **CV**: Update `_data/cv.yml`
4. **Projects**: Add/edit files in `_projects/`
5. **Publications**: Update `_bibliography/papers.bib`

---

## 📝 License

The theme is available as open source under the terms of the [MIT License](https://github.com/alshedivat/al-folio/blob/master/LICENSE).

Originally based on the [\*folio theme](https://github.com/bogoli/-folio) by [Lia Bogoev](https://liabogoev.com).
