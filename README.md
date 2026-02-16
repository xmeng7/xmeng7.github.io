# Xiangyu Meng - Personal Website

Static website for GitHub Pages deployment.

## Files Needed

To deploy this website, you need to upload the following files to your GitHub repository:

1. `index.html` - Main website file
2. `photo.PNG` - Your profile photo
3. `CV_Xiangyu_Meng.pdf` - Your CV
4. `Teaching_Statement_Meng.pdf` - Teaching statement
5. `Diversity_Meng.pdf` - Diversity statement
6. `TeachingEvaluation_Meng.pdf` - Teaching evaluation

## Deployment Steps

### 1. Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in (or create an account)
2. Click the "+" icon in the top right → "New repository"
3. Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
4. Make it **Public**
5. Click "Create repository"

### 2. Upload Files

**Option A: Using GitHub Web Interface (Easiest)**
1. In your new repository, click "Add file" → "Upload files"
2. Drag and drop all the files listed above
3. Click "Commit changes"

**Option B: Using Git Command Line**
```bash
# Navigate to your documents folder
cd /Users/xm2489/Library/CloudStorage/Dropbox/xm_web/documents

# Initialize git
git init

# Add files
git add index.html photo.PNG CV_Xiangyu_Meng.pdf Teaching_Statement_Meng.pdf Diversity_Meng.pdf TeachingEvaluation_Meng.pdf

# Commit
git commit -m "Initial website commit"

# Add remote (replace 'yourusername' with your GitHub username)
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" → "Pages" (in the left sidebar)
3. Under "Source", select "main" branch
4. Click "Save"

### 4. Access Your Website

Your website will be live at: `https://yourusername.github.io`

**Note:** It may take a few minutes for the site to go live after first deployment.

## Custom Domain (Optional)

If you want a custom domain like `xiangyumeng.com`:

1. Buy a domain from Namecheap, Google Domains, etc.
2. In your repository settings → Pages, add your custom domain
3. Update your domain's DNS settings to point to GitHub Pages
4. Create a `CNAME` file in your repository with your domain name

## File Structure

```
yourusername.github.io/
├── index.html
├── photo.PNG
├── CV_Xiangyu_Meng.pdf
├── Teaching_Statement_Meng.pdf
├── Diversity_Meng.pdf
└── TeachingEvaluation_Meng.pdf
```

## Notes

- All file paths are now relative (no `/files/` or `/photo/` prefixes)
- No Flask or Python required - pure static HTML
- Free hosting forever on GitHub Pages
- Automatically updates when you push changes to GitHub
