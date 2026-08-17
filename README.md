# Mustafizur Rohman — Portfolio Website

A responsive personal portfolio website for **Mustafizur Rohman**, a Video Editor & Graphic Designer based in Dhaka, Bangladesh.

The site presents selected creative work, services, an interactive pricing/rate card, payment information, social profiles, and a client contact form.

## ✨ Features

- Responsive desktop, tablet, and mobile layout
- Sticky navigation with mobile menu
- Hero section with professional introduction and stats
- About section with education/certification information
- Dynamic portfolio grid powered by JavaScript
- Portfolio filters: **All / Video / Graphics**
- Behance project links with thumbnails and project metrics
- Services section covering video editing, motion graphics, graphic design, and branding
- Interactive pricing/rate card with **USD / BDT** currency tabs
- Pricing search, category filter, and sorting controls
- Retainer plans, add-ons, rush pricing, tiers, and comparison sections
- Payment methods with one-click copy buttons
- Contact form connected to Formspree
- Scroll-reveal animations
- Active navigation state while scrolling
- Automatically updated copyright year
- No build system or package manager required

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Google Fonts: DM Serif Display, DM Mono, Outfit
- Formspree for contact-form submissions
- Behance-hosted portfolio thumbnails and project links

## 📁 Project Structure

```text
mustafizur-portfolio/
├── index.html      # Main website
├── README.md       # Project documentation
├── .gitignore      # Git ignore rules
├── LICENSE         # MIT license
└── robots.txt      # Search-engine crawler instructions
```

## 🚀 Run Locally

No installation is required.

### Option 1 — Open directly

Double-click `index.html` and open it in a modern browser.

### Option 2 — Use a local server

From the project folder:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

Using a local server is recommended when testing browser APIs such as the clipboard function and contact-form behavior.

## 🌐 Deploy with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `README.md`, `.gitignore`, `LICENSE`, and `robots.txt`.
3. Open **Settings → Pages** in the repository.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder.
6. Save the settings.
7. GitHub will publish the website at your GitHub Pages URL.

Because this is a static HTML/CSS/JavaScript website, no Node.js, npm, build command, or backend server is required.

## 📬 Contact Form

The contact form uses Formspree.

The current website contains this endpoint in the JavaScript:

```js
const FORMSPREE_ENDPOINT = "https://formspree.io/f/xaewpokk";
```

If you replace the Formspree form, update that value in `index.html`.

The form collects:

- Name
- Email
- Project type
- Project message

## 🎨 Customization

Most content can be edited directly inside `index.html`.

### Personal information

Update the hero, About, Contact, and footer sections.

### Portfolio projects

Projects are stored in the JavaScript `projects` array. Each project contains:

```js
{
  n: "Project Name",
  cat: "video",
  img: "IMAGE_URL",
  url: "PROJECT_URL",
  appr: 0,
  views: 0
}
```

Use `video` or `graphics` for `cat` so the portfolio filters continue working.

### Pricing

Pricing data is stored in the `rateData` JavaScript array. Each service contains USD and BDT prices for Basic, Intermediate, and Premium tiers.

### Social links

Update the social URLs in the Contact and Footer sections if your profiles change.

## ⚠️ Before Publishing

Check these items before making the repository public:

- Replace any outdated social/profile URLs.
- Confirm portfolio project URLs and thumbnails.
- Confirm pricing and payment information.
- Confirm the Formspree endpoint belongs to the intended account/form.
- Review public contact and payment details before publishing.
- Replace any placeholder content if you add new sections.

## 📄 License

This project is released under the MIT License. See `LICENSE` for details.

## 👤 Author

**Mustafizur Rohman**  
Video Editor & Graphic Designer  
Dhaka, Bangladesh

- Behance: https://www.behance.net/tg_mustafizur
- Upwork: https://www.upwork.com/freelancers/~01585c41ed8ebe7652
