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

You can deploy the site directly from this repository without additional build steps:

1. Commit your changes and push to GitHub.
2. In the repository settings, open **Pages**.
3. Under **Source**, choose **Deploy from a branch** and select the `main` branch with the root directory (`/`).
4. Save. GitHub Pages will publish the site at `https://<your-username>.github.io/<repo>/`.

If you prefer to keep the site in a `docs/` folder, move `index.html` and `assets/` into `docs/` and select `/docs` as the GitHub Pages source.

## Customization tips

- Update copy (headline, metrics, projects, publications) in `index.html`.
- Adjust the color palette, typography, or spacing in `assets/styles.css`.
- Replace links in the contact section with your actual email and social profiles.
- Add analytics or form handling by wiring a service to the static contact form button.
