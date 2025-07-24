# BarrelBook Legal Documents

This repository contains the legal documents for the BarrelBook iOS application.

## Live Site

Once deployed: https://[your-username].github.io/barrelbook-legal/

## Contents

- **Privacy Policy** - Data collection and usage policies
- **Terms of Service** - Usage terms and conditions
- **index.html** - Web interface for viewing documents

## Quick Setup (5 minutes)

### 1. Create GitHub Repository
- Go to [github.com/new](https://github.com/new)
- Repository name: `barrelbook-legal`
- Description: "Legal documents for BarrelBook iOS app"
- Public repository
- **Do NOT** initialize with README

### 2. Push This Code
```bash
# From your main BarrelBook project directory:
cd barrelbook-legal-temp
git init
git add .
git commit -m "Initial legal documents"
git branch -M main
git remote add origin https://github.com/[YOUR-USERNAME]/barrelbook-legal.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to your new repo on GitHub
2. Settings → Pages
3. Source: Deploy from a branch
4. Branch: `main` / `/ (root)`
5. Click Save

### 4. Update Your App
After GitHub Pages is live (takes 2-5 minutes), update these files in your BarrelBook app:

**AuthenticationView.swift** (lines 94 & 104):
```swift
// Change from:
openURL("https://barrelbook.app/privacy")
// To:
openURL("https://[YOUR-USERNAME].github.io/barrelbook-legal/#privacy")
```

**Info.plist** (line 54):
```xml
<!-- Change from: -->
<string>https://barrelbook.app/privacy</string>
<!-- To: -->
<string>https://[YOUR-USERNAME].github.io/barrelbook-legal/#privacy</string>
```

## Testing

Visit your GitHub Pages URL to ensure both documents load correctly:
- Privacy Policy: `https://[your-username].github.io/barrelbook-legal/#privacy`
- Terms of Service: `https://[your-username].github.io/barrelbook-legal/#terms`

## Custom Domain (Optional)

If you own a domain:
1. Add CNAME file with your domain
2. Configure DNS to point to GitHub Pages
3. Update URLs in your app

---

© 2025 BarrelBook. All rights reserved.