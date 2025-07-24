# Legal Documents Hosting Setup

## Option 1: GitHub Pages (Free & Easy)

1. **Enable GitHub Pages**
   - Go to your repository Settings
   - Navigate to Pages section
   - Set Source to "Deploy from a branch"
   - Select "main" branch and "/docs" folder
   - Save

2. **Custom Domain (Optional)**
   - Add `barrelbook.app` to Custom domain field
   - Create CNAME records pointing to GitHub Pages

3. **URLs will be:**
   - Without custom domain: `https://[username].github.io/BarrelBook/#privacy`
   - With custom domain: `https://barrelbook.app/#privacy`

## Option 2: Quick Alternatives

### Notion
1. Create pages for Privacy Policy and Terms
2. Share publicly
3. Use Notion URLs in the app

### Google Docs
1. Create documents
2. Share with "Anyone with the link"
3. Use sharing URLs

### Carrd.co
1. Create simple one-page site
2. Add both documents
3. Free with carrd.co subdomain

## Option 3: Your Own Hosting

1. **Upload to any web host**
2. **Update URLs in:**
   - `AuthenticationView.swift` (lines 94 & 104)
   - `Info.plist` (line 54)
   - `LegalView.swift` (if using in-app display)

## Testing the Links

Before TestFlight submission:
1. Verify all links work
2. Check mobile formatting
3. Ensure fast loading
4. Test in Safari and in-app browser

## App Store Requirements

✅ Privacy Policy URL in Info.plist
✅ Links accessible from authentication screen
✅ Both documents publicly accessible
✅ Mobile-friendly formatting