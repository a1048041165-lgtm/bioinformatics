# Bioinformatics Portfolio

A single-page portfolio site for a bioinformatics scientist. It highlights research focus areas, selected projects, and publications, and is ready to deploy with GitHub Pages.

## Running locally

1. Clone the repository and open it in your browser:

   ```bash
   git clone <your-fork-url>
   cd bioinformatics
   python -m http.server 8000
   ```

2. Visit `http://localhost:8000` to view the site.

## GitHub Pages deployment

### Automated deployment (recommended)

This repository includes a GitHub Actions workflow that publishes the site to GitHub Pages automatically:

1. Fork the repository on GitHub and push your changes to the `main` branch.
2. In **Settings → Pages**, set **Source** to **GitHub Actions**.
3. On the next push to `main`, the `Deploy to GitHub Pages` workflow will build and publish the site. The live URL is available in the workflow summary as `page_url` and will follow `https://<your-username>.github.io/<repo>/`.

### Manual branch deployment

If you prefer configuring Pages without Actions:

1. Commit your changes and push to GitHub.
2. In **Settings → Pages**, choose **Deploy from a branch**, select the `main` branch, and the root directory (`/`).
3. Save. GitHub Pages will publish the site at `https://<your-username>.github.io/<repo>/`.

If you prefer to keep the site in a `docs/` folder, move `index.html` and `assets/` into `docs/` and select `/docs` as the GitHub Pages source.

## Customization tips

- Update copy (headline, metrics, projects, publications) in `index.html`.
- Adjust the color palette, typography, or spacing in `assets/styles.css`.
- Replace links in the contact section with your actual email and social profiles.
- Add analytics or form handling by wiring a service to the static contact form button.
