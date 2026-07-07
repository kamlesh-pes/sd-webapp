# Sahastra Digital — Sample E-commerce Page

A single-page storefront concept for **Sahastra Digital** (info@sahastradigital.com), built with plain HTML/CSS/JS — no build step, no dependencies beyond Google Fonts.

## Files
- `index.html` — the full page (hero, categories, product grid, footer)
- `assets/logo.png` — your logo, used in the header, hero card, and footer

## Host it on GitHub Pages
1. Create a new repository (e.g. `sahastra-digital-site`) and push these files to the root of the `main` branch:
   ```bash
   git init
   git add index.html README.md assets/logo.png
   git commit -m "Initial storefront"
   git branch -M main
   git remote add origin https://github.com/<your-username>/sahastra-digital-site.git
   git push -u origin main
   ```
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
5. GitHub will publish the site at `https://<your-username>.github.io/sahastra-digital-site/` within a minute or two.

## Customizing
- **Products**: each `<article class="prod-card">` in `index.html` is one product — duplicate the block to add more, or replace the emoji glyph in `.prod-media` with a real product photo (`<img src="assets/your-photo.jpg">`).
- **Colors**: all brand colors are CSS variables at the top of the `<style>` block (`--blue`, `--orange`, etc.) — matched to the logo's blue-to-orange gradient.
- **Cart/checkout**: this is a front-end demo only — the cart icon, "Add to cart" buttons, and newsletter form don't connect to a backend yet. Wire them up to a service like Shopify Buy Button, Snipcart, or a custom API when you're ready to sell for real.
