# Lubbock Rodent Sealing

A static informational website about rodent control in Lubbock, Texas. Built as a clean, mobile-responsive site ready for GitHub Pages deployment.

## Site Structure

```
.
├── index.html                                       # Homepage with article grid
├── what-does-rodent-exterminator-do/                # MAIN ARTICLE (featured)
│   └── index.html
├── how-to-choose-rodent-exterminator-lubbock/       # Referring article 1
│   └── index.html
├── rodent-service-visit-cost-lubbock/               # Referring article 2
│   └── index.html
├── signs-you-need-professional-rodent-exterminator/ # Referring article 3
│   └── index.html
├── about/
│   └── index.html
├── contact/
│   └── index.html
├── css/
│   └── style.css
├── sitemap.xml
├── robots.txt
├── .nojekyll
└── README.md
```

## Internal Linking Structure

The three referring articles each link contextually to the main featured article:

- **How to Choose a Rodent Exterminator** → links to main article in the inspection section
- **Service Visit Cost in Lubbock** → links to main article in the components section
- **Signs You Need a Professional** → links to main article in the professional service section

Plus each article has a CTA box at the bottom directing to the main article.

## Deploying to GitHub Pages

1. Create a new GitHub repository
2. Push these files to the `main` branch
3. Go to repository **Settings** → **Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Save — the site will be live at `https://<username>.github.io/<reponame>/` within a few minutes

For a custom domain, add a `CNAME` file with your domain name.

## Updating Canonical URLs

After deploying, update the `<link rel="canonical">` URLs in each HTML file to match your actual deployed URL. Currently set to `https://lubbockrodentsealing.github.io/` placeholder.

## Tech Notes

- Pure static HTML/CSS — no build process, no dependencies
- Mobile-responsive design
- Sticky header navigation
- SEO meta tags on every page
- Clean folder-based URLs (no .html extensions in production)
- `.nojekyll` file present to prevent GitHub from processing as Jekyll
