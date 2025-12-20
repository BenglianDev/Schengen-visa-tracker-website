# Schengen Visa Tracker Website

A mobile-optimized website for the Schengen Visa Tracker app.

## Live Preview

The website is ready to deploy at: https://schengenvisatracker.com

## Contents

- `index.html` - Main website (single-page, all sections included)
- `images/app-icon.png` - App icon
- `images/screenshots/` - App screenshots for tutorial

## Sections

1. **Hero** - App introduction with download button
2. **Features** - 6 key features of the app
3. **App Preview** - Screenshot carousel
4. **Tutorial** - 6-step guide with screenshots
5. **Pricing** - €2.99 lifetime purchase info
6. **Privacy Policy** - Full privacy policy
7. **Contact** - Support email link
8. **Footer** - Navigation links

## Deployment to GitHub Pages (Free)

### Option 1: Quick Setup

1. Create a new repository on GitHub named `schengenvisatracker.com` (or any name)
2. Upload all files from this folder to the repository
3. Go to **Settings** → **Pages**
4. Under "Source", select **main** branch and **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/repository-name/`

### Option 2: Using Git Command Line

```bash
cd schengen-website
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/schengenvisatracker.com.git
git push -u origin main
```

Then enable GitHub Pages in repository settings.

## Connect Your Custom Domain (schengenvisatracker.com)

### Step 1: Add Custom Domain in GitHub

1. Go to your repository **Settings** → **Pages**
2. Under "Custom domain", enter: `schengenvisatracker.com`
3. Click **Save**
4. Check "Enforce HTTPS" (after DNS propagates)

### Step 2: Update DNS at GoDaddy

1. Log in to GoDaddy
2. Go to **My Products** → **DNS** for schengenvisatracker.com
3. Delete any existing A records or CNAME for @ or www
4. Add these **A records** (for apex domain):
   - Type: A, Name: @, Value: `185.199.108.153`
   - Type: A, Name: @, Value: `185.199.109.153`
   - Type: A, Name: @, Value: `185.199.110.153`
   - Type: A, Name: @, Value: `185.199.111.153`
5. Add **CNAME record** (for www):
   - Type: CNAME, Name: www, Value: `YOUR_USERNAME.github.io`
6. Save changes

DNS propagation takes 24-48 hours. After that, your site will be live at https://schengenvisatracker.com

## Alternative Hosting Options

### Netlify (Free)
1. Go to https://netlify.com
2. Drag and drop the `schengen-website` folder
3. Site is instantly live
4. Add custom domain in site settings

### Vercel (Free)
1. Go to https://vercel.com
2. Import from GitHub or upload folder
3. Site is instantly live
4. Add custom domain in project settings

## Support

Email: schengenvisatracker@gmail.com
