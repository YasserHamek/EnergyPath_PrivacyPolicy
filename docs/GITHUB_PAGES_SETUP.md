# GitHub Pages Setup for Energy Path Privacy Policy

This guide explains how to host the Energy Path privacy policy on GitHub Pages.

## Setup Instructions

### Step 1: Push the docs folder to GitHub

Make sure the `docs/` folder is committed and pushed to your repository:

```bash
git add docs/
git commit -m "Add privacy policy for App Store submission"
git push origin master
```

### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/YasserHamek/EnergyPath
2. Click **Settings** (gear icon in the top menu)
3. In the left sidebar, click **Pages**
4. Under **Source**, select:
   - **Branch:** `master`
   - **Folder:** `/docs`
5. Click **Save**

### Step 3: Wait for Deployment

GitHub will automatically build and deploy your site. This usually takes 1-2 minutes.

You can check the deployment status in the **Actions** tab of your repository.

## Privacy Policy URLs

Once deployed, your privacy policies will be available at:

| Language | URL |
|----------|-----|
| English | https://yasserhamek.github.io/EnergyPath/privacy-policy.html |
| Arabic | https://yasserhamek.github.io/EnergyPath/privacy-policy-ar.html |
| French | https://yasserhamek.github.io/EnergyPath/privacy-policy-fr.html |

## App Store Connect Configuration

Use the **English URL** as your Privacy Policy URL in App Store Connect:

```
https://yasserhamek.github.io/EnergyPath/privacy-policy.html
```

## Updating the Privacy Policy

To update the privacy policy:

1. Edit the HTML files in the `docs/` folder
2. Update the "Last updated" date
3. Commit and push your changes
4. GitHub Pages will automatically redeploy

## Troubleshooting

### Site not showing?

- Make sure the `docs/` folder is on the `master` branch
- Check that GitHub Pages is enabled in Settings > Pages
- Wait a few minutes for initial deployment
- Check the Actions tab for any build errors

### Custom domain (optional)

If you want to use a custom domain:

1. Add a `CNAME` file to the `docs/` folder with your domain
2. Configure your domain's DNS to point to GitHub Pages
3. Update the privacy policy URL in App Store Connect

## Files in this folder

- `index.html` - Redirects to English privacy policy
- `privacy-policy.html` - English privacy policy
- `privacy-policy-ar.html` - Arabic privacy policy (RTL)
- `privacy-policy-fr.html` - French privacy policy
- `GITHUB_PAGES_SETUP.md` - This setup guide
