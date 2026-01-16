# SL Fashion Blog - GitHub Pages Setup

## Quick Setup for GitHub Pages

### 1. Create a GitHub Repository
- Go to github.com and create a new repository
- Name it `yourusername.github.io` for a user site, or any name for a project site

### 2. Upload These Files
Upload `index.html` and `style.css` to your repository

### 3. Enable GitHub Pages
- Go to repository Settings → Pages
- Under "Source", select "Deploy from a branch"
- Choose "main" branch and "/ (root)" folder
- Click Save

### 4. Connect Your Free Domain

#### From Namecheap (GitHub Student Pack):
1. Go to education.github.com/pack
2. Find Namecheap and claim your free .me domain
3. In Namecheap dashboard, go to Domain List → Manage
4. Click "Advanced DNS"
5. Add these records:
   - Type: A Record, Host: @, Value: 185.199.108.153
   - Type: A Record, Host: @, Value: 185.199.109.153
   - Type: A Record, Host: @, Value: 185.199.110.153
   - Type: A Record, Host: @, Value: 185.199.111.153
   - Type: CNAME, Host: www, Value: yourusername.github.io

6. In GitHub repo Settings → Pages:
   - Add your custom domain (yourdomain.me)
   - Check "Enforce HTTPS"

### 5. Customize Your Site

Edit `index.html` to update:
- Your name/brand in nav and footer
- Social media links (Flickr, Facebook, Linktree)
- About section text
- Blog posts
- Style credits
- Inworld avatar name

Replace placeholder images with your own Flickr photos or uploads.

## File Structure
```
blog-site/
├── index.html    # Main page
├── style.css     # Pink theme styles
└── README.md     # This file
```

## Adding Blog Posts

For a simple static site, duplicate the blog-card HTML for new posts.
For more posts, consider using Jekyll (GitHub Pages supports it natively).

## Color Customization

Edit the CSS variables in style.css to adjust the pink theme:
```css
:root {
    --pink-dark: #d63384;
    --pink-main: #ff69b4;
    --pink-light: #ffb6c1;
    --pink-pale: #fff0f5;
    --pink-accent: #ff1493;
}
```
