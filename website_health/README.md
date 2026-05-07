# HealthBridge — Healthcare Website

A clean, responsive healthcare website built with vanilla HTML, CSS, and JavaScript. Zero dependencies. Ready for GitHub Pages.

## Pages

- **Home** (`index.html`) — Hero, stats, services preview, testimonials, CTA
- **About** (`about.html`) — Mission, values, team profiles
- **Services** (`services.html`) — Detailed service descriptions with tags
- **Contact** (`contact.html`) — Contact form, info cards, map placeholder

## Deploy to GitHub Pages

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose `main` (or `master`) branch, root `/`
5. Click **Save** — your site will be live at `https://<username>.github.io/<repo-name>/`

## Custom Domain / Subdomain

When you're ready to connect a custom subdomain:

1. Create a `CNAME` file in the root with your domain:
   ```
   health.yourdomain.com
   ```
2. Add a **CNAME record** in your DNS provider pointing to `<username>.github.io`
3. In GitHub repo **Settings → Pages → Custom domain**, enter your subdomain
4. Enable **Enforce HTTPS**

All internal links use relative paths (`href="about.html"`) so the site works at any path depth — root domain, subdomain, or subdirectory.

## Customization

- **Colors**: Edit CSS custom properties in `style.css` under `:root`
- **Content**: Edit the HTML files directly — all text is inline
- **Form**: The contact form currently simulates submission. To make it functional:
  - Use [Formspree](https://formspree.io) (free tier) — change `<form action="https://formspree.io/f/YOUR_ID" method="POST">`
  - Or use [Netlify Forms](https://docs.netlify.com/forms/setup/) if hosted on Netlify
- **Map**: Replace the map placeholder in `contact.html` with a Google Maps `<iframe>` embed
- **Images**: Replace SVG placeholders with actual photos

## Tech

- Pure HTML5, CSS3, JavaScript (ES6+)
- No frameworks, no build step, no dependencies
- Responsive (mobile-first breakpoints)
- Scroll-reveal animations via Intersection Observer
- Accessible navigation with ARIA labels
