# SeekCool Inc Website

A responsive, accessible, GitHub Pages-ready website for **SeekCool Inc**.

![SeekCool website preview](preview.png)

## Included

- Professional single-page company website
- Responsive desktop, tablet, and mobile layouts
- Accessible navigation, focus states, reduced-motion support, and semantic HTML
- Custom SVG logo and favicon
- SEO, Open Graph, Twitter card, sitemap, robots.txt, and organization structured data
- Custom 404 page
- GitHub Actions workflow for automatic GitHub Pages deployment
- No external fonts, frameworks, trackers, or runtime dependencies

## Public information used

The site copy is based on SeekCool's public LinkedIn profile and public nonprofit records. It describes SeekCool as an educational nonprofit that advances education and technology research through conferences, innovation support, industry-academic collaboration, publications, and workshops.

Before launch, review all wording, legal details, links, and brand assets as the organization owner.

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy with GitHub Pages

1. Create a GitHub repository, such as `seekcool-website`.
2. Add these files and push them to the `main` branch.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **GitHub Actions**.
5. The included `.github/workflows/pages.yml` workflow will deploy the site after each push to `main`.

Example command-line setup:

```bash
git init
git add .
git commit -m "Launch SeekCool website"
git branch -M main
git remote add origin https://github.com/YOUR-ACCOUNT/seekcool-website.git
git push -u origin main
```

## Connect `seekcool.org`

After the Pages deployment succeeds:

1. Verify the domain in the GitHub account or organization that owns the repository.
2. In **Settings → Pages → Custom domain**, enter `seekcool.org` and save.
3. Configure the required DNS records with the domain provider.
4. Enable **Enforce HTTPS** after GitHub provisions the certificate.

When deploying with a custom GitHub Actions workflow, GitHub manages the custom domain through repository settings; a `CNAME` file is not required.

## Update content

- Main page content: `index.html`
- Visual design: `assets/styles.css`
- Navigation and reveal behavior: `assets/script.js`
- Logo: `assets/logo.svg`
- Social preview: `assets/og-image.png`

## Brand note

The included logo is a newly created website concept, not a claim that it is SeekCool's previously registered or official logo. Replace it if an approved brand asset exists.
