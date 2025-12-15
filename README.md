# DMARC Analyser Landing Page

Static landing page for [DMARC Analyser](https://github.com/helliott20/dmarc-analyser).

## Deployment

This site is designed to be hosted on GitHub Pages.

### Setup

1. Push this folder to the `dmarc-analyser-website` repo
2. Go to **Settings > Pages** in GitHub
3. Set source to "Deploy from a branch"
4. Select `main` branch and `/ (root)` folder
5. Save

Your site will be available at `https://helliott20.github.io/dmarc-analyser-website/`

### Custom Domain

To use a custom domain (e.g., `dmarcanalyser.io`):

1. Add a `CNAME` file with your domain:
   ```
   dmarcanalyser.io
   ```

2. Configure DNS with your registrar:
   - For apex domain: Add `A` records pointing to GitHub's IPs
   - For www: Add `CNAME` record pointing to `helliott20.github.io`

See [GitHub's documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) for details.

## Structure

- `index.html` - Main landing page
- `pricing.html` - Pricing page with calculator
- `CNAME` - Custom domain configuration (add if needed)

## Links

All "Sign In" and "Start Free Trial" buttons link to:
- `https://app.dmarcanalyser.io/login`

Update these if your app is hosted at a different URL.

## Styling

Uses [Tailwind CSS CDN](https://tailwindcss.com/docs/installation/play-cdn) for styling. No build step required.
