# GitHub Pages Setup Guide - Removing Custom Domain

## Step 1: Commit and Push Your Changes Locally

Open your terminal/PowerShell in the project directory and run:

```bash
# Check what files have changed
git status

# Add all changed files
git add _config.yml index.md _data/authors.yml

# Commit the changes
git commit -m "Switch from custom domain to GitHub Pages URL"

# Push to GitHub
git push origin main
```
*(If your default branch is `master` instead of `main`, use `git push origin master`)*

---

## Step 2: Remove Custom Domain from GitHub Pages Settings

1. **Go to your GitHub repository:**
   - Navigate to `https://github.com/shreeramgs/shreeramgs.github.io`

2. **Open Settings:**
   - Click on the **"Settings"** tab (at the top of the repository)

3. **Go to Pages section:**
   - Scroll down in the left sidebar and click on **"Pages"** (under "Code and automation")

4. **Remove Custom Domain:**
   - Look for the **"Custom domain"** section
   - If you see `shreeramgs.com` listed:
     - Click the **"Remove"** button next to it
     - Confirm the removal
   - **Important:** Leave the custom domain field **empty** (don't add anything)

5. **Verify Source Branch:**
   - Under **"Source"**, make sure it's set to:
     - **Branch:** `main` (or `master` if that's your default branch)
     - **Folder:** `/ (root)`

6. **Save Changes:**
   - The changes should save automatically

---

## Step 3: Check for and Remove CNAME File

1. **Check if CNAME file exists:**
   - In your repository, go to the root directory
   - Look for a file named `CNAME` (it might be hidden)
   - If you see it, click on it

2. **Delete CNAME file:**
   - Click the **trash icon** (Delete file) button
   - Commit the deletion with message: "Remove CNAME file"
   - Click **"Commit changes"**

   **OR** if you prefer using terminal:
   ```bash
   git rm CNAME
   git commit -m "Remove CNAME file"
   git push origin main
   ```

---

## Step 4: Verify GitHub Actions Build

1. **Check Actions Tab:**
   - Go to the **"Actions"** tab in your repository
   - You should see a workflow run for "pages build and deployment"
   - Wait for it to complete (should show a green checkmark ✅)

2. **If build fails:**
   - Click on the failed workflow to see error details
   - Common issues:
     - Syntax errors in `_config.yml` (check YAML formatting)
     - Missing dependencies (usually auto-resolved by GitHub)

---

## Step 5: Wait for DNS Propagation

After removing the custom domain:
- **Wait 5-10 minutes** for GitHub Pages to update
- GitHub Pages may take a few minutes to rebuild and deploy

---

## Step 6: Test Your Site

1. **Visit your GitHub Pages URL:**
   - Go to: `https://shreeramgs.github.io`
   - The site should now load correctly

2. **If you still see 404:**
   - Clear your browser cache (Ctrl+Shift+Delete)
   - Try incognito/private browsing mode
   - Wait a few more minutes and try again
   - Check the Actions tab to ensure the build succeeded

---

## Step 7: Verify All Links Work

Test these pages:
- `https://shreeramgs.github.io` (home page)
- `https://shreeramgs.github.io/publications/`
- `https://shreeramgs.github.io/research/`
- `https://shreeramgs.github.io/projects/`

---

## Troubleshooting

### Still Getting 404?
1. **Check repository name:** Must be exactly `shreeramgs.github.io`
2. **Check branch name:** Should be `main` or `master` (not `gh-pages`)
3. **Verify `_config.yml`:**
   - `url: "https://shreeramgs.github.io"`
   - `baseurl: ""` (empty)
4. **Check GitHub Pages status:** Settings → Pages should show "Your site is live at https://shreeramgs.github.io"

### Build Errors?
- Check the Actions tab for specific error messages
- Verify YAML syntax in `_config.yml` (no tabs, proper indentation)
- Make sure `index.md` exists in the root directory

### Custom Domain Still Showing?
- Double-check Settings → Pages → Custom domain is empty
- Verify CNAME file is deleted
- Wait 10-15 minutes for DNS cache to clear

---

## Summary of Changes Made

✅ Updated `_config.yml`:
- Changed `url` to `"https://shreeramgs.github.io"`
- Changed `repository` to `"shreeramgs.github.io"`

✅ Created `index.md`:
- Added home page content

✅ Updated `_data/authors.yml`:
- Changed `uri` to `"https://shreeramgs.github.io"`
- Fixed `twitter` to `"shreeramgs666"`

---

## Next Steps After Setup

Once your site is live:
1. Update any external links that point to `shreeramgs.com`
2. Update your social media profiles with the new URL
3. Update your email signature if it includes the old domain
4. Consider setting up redirects at your old domain (if you still own it)
