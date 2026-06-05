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
├── images/
│   ├── pest-control-professional.jpg                # Featured image
│   ├── home-inspection-entry-points.jpg             # Content image 1
│   └── professional-sealing-cleanup.jpg             # Content image 2
├── css/
│   └── style.css
├── sitemap.xml
├── robots.txt
├── .nojekyll
└── README.md
```

## Media in the Main Article

The featured article includes:

- **1 Featured image** at the top (pest control professional with PPE)
- **2 Content images** in context — one in the inspection section, one in the exclusion section
- **1 YouTube video embed** — a professional rodent inspection walkthrough (Smith's Pest Management)
- All images have descriptive alt text and figcaptions for SEO and accessibility
- YouTube embed is responsive (16:9) on all screen sizes

## Internal Linking Structure

The three referring articles each link contextually to the main featured article:

- **How to Choose a Rodent Exterminator** → links to main article in the inspection section
- **Service Visit Cost in Lubbock** → links to main article in the components section
- **Signs You Need a Professional** → links to main article in the professional service section

Plus each article has a CTA box at the bottom directing to the main article.

## Deploying to GitHub Pages

1. Create a new GitHub repository
2. Push these files to the `main` branch
3. Go to repository **Settings** → **Pages** (under "Code and automation")
4. Under "Source", select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Save — the site will be live at `https://<username>.github.io/<reponame>/` within a few minutes

For a custom domain, add a `CNAME` file with your domain name.

## Updating Canonical URLs

After deploying, update the `<link rel="canonical">` URLs in each HTML file to match your actual deployed URL. Currently set to `https://lubbockrodentsealing.github.io/` placeholder.

## Image Credits

Featured and content images sourced from Unsplash (CDC photo library) — free for commercial use.

## Tech Notes

- Pure static HTML/CSS — no build process, no dependencies
- Mobile-responsive design
- Sticky header navigation
- Responsive YouTube video embed (16:9 aspect ratio)
- SEO meta tags on every page
- Lazy-loaded images for performance
- Clean folder-based URLs (no .html extensions in production)
- `.nojekyll` file present to prevent GitHub from processing as Jekyll
