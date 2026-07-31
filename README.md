# EarthQuake Watcher - Developer Website

This repository contains the developer website for the EarthQuake Watcher Android app, including the required `app-ads.txt` file for AdMob verification.

## 📁 Files

- **index.html** - Main landing page for the app
- **privacy-policy.html** - Privacy policy (required for Google Play)
- **app-ads.txt** - AdMob verification file (required for ad monetization)

## 🚀 Quick Setup with GitHub Pages

### Step 1: Fork or Clone This Repository

```bash
git clone https://github.com/yourusername/earthquakewatcher-website.git
cd earthquakewatcher-website
```

### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll to **Pages** section (left sidebar)
4. Under **Source**, select **main** branch
5. Click **Save**
6. Wait 1-2 minutes for deployment

Your site will be available at:
```
https://yourusername.github.io/earthquakewatcher-website/
```

### Step 3: Verify app-ads.txt

After GitHub Pages is enabled, verify your app-ads.txt file is accessible:

```
https://yourusername.github.io/earthquakewatcher-website/app-ads.txt
```

You should see:
```
google.com, pub-5074870178134500, DIRECT, f08c47fec0942fa0
```

### Step 4: Update Google Play Console

1. Go to [Google Play Console](https://play.google.com/console)
2. Select **EarthQuake Watcher** app
3. Navigate to **Store presence** → **Store listing**
4. In **Contact details** section, add your website:
   ```
   https://yourusername.github.io/earthquakewatcher-website
   ```
5. Click **Save**

### Step 5: Verify in AdMob

1. Go to [AdMob Console](https://apps.admob.com)
2. Navigate to **Apps** → **EarthQuake Watcher**
3. Click **App Settings**
4. Scroll to **app-ads.txt** section
5. Click **"Check for updates"**
6. Wait for verification (typically 1-24 hours)

## 🌐 Using a Custom Domain (Optional)

If you want to use a custom domain (e.g., `earthquakewatcher.com`):

### Step 1: Buy a Domain

Purchase a domain from:
- [Namecheap](https://www.namecheap.com) (~$10/year)
- [Google Domains](https://domains.google) (~$12/year)
- [GoDaddy](https://www.godaddy.com) (~$12/year)

### Step 2: Configure DNS

Add these DNS records in your domain provider:

**For apex domain (earthquakewatcher.com):**
```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
```

**For www subdomain:**
```
CNAME www   yourusername.github.io
```

### Step 3: Configure GitHub Pages

1. In your repository, go to **Settings** → **Pages**
2. Under **Custom domain**, enter: `earthquakewatcher.com`
3. Click **Save**
4. Wait for DNS check to complete
5. Enable **Enforce HTTPS** (recommended)

### Step 4: Update Google Play Console

Update your website URL to:
```
https://earthquakewatcher.com
```

Your app-ads.txt will now be at:
```
https://earthquakewatcher.com/app-ads.txt
```

## 📝 Important Notes

### app-ads.txt Requirements

- **File name:** Must be exactly `app-ads.txt` (lowercase)
- **Location:** Must be at the root of your domain
- **Format:** Plain text file
- **Content:** Must match your AdMob publisher ID
- **Accessibility:** Must return HTTP 200 status

### Domain Matching

The domain in Google Play Console **MUST** exactly match where app-ads.txt is hosted:

✅ **CORRECT:**
- Play Store: `https://example.com`
- app-ads.txt: `https://example.com/app-ads.txt`

❌ **WRONG:**
- Play Store: `https://example.com`
- app-ads.txt: `https://different.com/app-ads.txt`

### Verification Timeline

- **GitHub Pages deployment:** 1-2 minutes
- **DNS propagation (custom domain):** 24-48 hours
- **AdMob verification:** 1-24 hours (sometimes up to 48 hours)

## 🔧 Troubleshooting

### app-ads.txt not found

1. Verify file is in repository root (not in a folder)
2. Check file name is exactly `app-ads.txt`
3. Ensure GitHub Pages is enabled
4. Wait a few minutes for deployment
5. Test URL in incognito browser

### Publisher ID doesn't match

1. Verify your AdMob publisher ID in AdMob console
2. Ensure app-ads.txt contains: `google.com, pub-5074870178134500, DIRECT, f08c47fec0942fa0`
3. No extra spaces or line breaks
4. File is plain text (not .doc or .pdf)

### Domain doesn't match

1. Ensure Google Play website field matches GitHub Pages URL exactly
2. Don't include trailing slash
3. Use HTTPS (not HTTP)
4. Wait for changes to propagate

## 📞 Support

For issues with:
- **GitHub Pages:** [GitHub Pages Documentation](https://docs.github.com/en/pages)
- **AdMob:** [AdMob Help Center](https://support.google.com/admob)
- **app-ads.txt:** [IAB Tech Lab Specification](https://iabtechlab.com/ads-txt/)

## 📄 License

This website is for the EarthQuake Watcher Android app.

**App Package:** com.paras.paras.earthquakewatcher

---

**Last Updated:** July 31, 2026
