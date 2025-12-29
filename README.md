# GitHub Pages Setup for Privacy Policy & Terms

## Files Created

- `index.html` - Landing page with links to privacy and terms
- `app/privacy.html` - Privacy Policy (French + English)
- `app/terms.html` - Terms of Service (French + English)

## How to Enable GitHub Pages

### Step 1: Push to GitHub

```bash
git add docs/
git commit -m "Add privacy policy and terms of service for app store submission"
git push
```

### Step 2: Enable GitHub Pages

1. Go to your GitHub repository
2. Click **Settings**
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Branch: Select **main** (or **master**)
   - Folder: Select **/docs**
5. Click **Save**

### Step 3: Wait for Deployment

GitHub will deploy your site in 1-2 minutes. You'll see:
- "Your site is live at `https://nursing509.github.io/Nursing_509/`"

Or if you have a custom GitHub username, it might be different.

### Step 4: Get Your URLs

Your privacy policy will be at:
- `https://nursing509.github.io/Nursing_509/app/privacy.html`
- `https://nursing509.github.io/Nursing_509/app/terms.html`

**Note:** Replace `nursing509` with your actual GitHub username if different.

### Step 5: Update the App

Update `/Users/guensley/Development/Nursing_509/lib/screens/consent_screen.dart`:

**Line 60:** Change to:
```dart
const url = 'https://nursing509.github.io/Nursing_509/app/privacy.html';
```

**Line 72:** Change to:
```dart
const url = 'https://nursing509.github.io/Nursing_509/app/terms.html';
```

### Step 6: Add to App Store Listings

**Google Play Console:**
- App content → Privacy policy → Add URL

**Apple App Store Connect:**
- App Information → Privacy Policy URL → Add URL

---

## Testing

After deployment, test the links:
1. Open the URLs in a browser
2. Verify content displays correctly
3. Test on mobile devices
4. Test links in the app's consent screen

---

## Optional: Custom Domain

If you want cleaner URLs like `https://nursing509.app/privacy`:

1. Buy domain (e.g., via Google Domains, Namecheap)
2. Configure DNS CNAME record
3. Update GitHub Pages settings with custom domain
4. Wait for SSL certificate (automatic)

Result: `https://nursing509.app/app/privacy.html`

---

## Files Are Ready!

Your privacy policy and terms are complete and app-store compliant. Just enable GitHub Pages and update the app with the final URLs.
