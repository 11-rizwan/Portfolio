# Mohamed Rizwan N — Portfolio

Personal portfolio site for Mohamed Rizwan N, a backend / full-stack software developer based in Chennai, India.

It is a single static page: plain HTML, CSS and JavaScript in one file, with no build step and no dependencies.

## Features

- **Projects:** featured work with architecture diagrams, key metrics, tech tags and GitHub links
- **Experience, education and stack:** timeline plus grouped skills
- **Dark and light themes:** toggle in the nav, remembered between visits
- **Animation:** scroll reveals, typewriter role badge, animated architecture arrows, count-up numbers, scroll progress bar
- **Interactivity:** cursor spotlight in the hero, card tilt and glow, hoverable name, active nav highlighting, copy-email button
- **Responsive:** phones (with hamburger menu), tablets, laptops and large screens, with safe-area support for notched devices
- **Accessible:** keyboard focus styles, ARIA labels, and `prefers-reduced-motion` support that turns animation off

## Project structure

```
.
├── index.html   # the whole site (HTML + CSS + JS)
└── README.md
```

## Run locally

No install needed. Either:

- open `index.html` directly in a browser, or
- serve the folder with any static server:

```bash
# Python
python -m http.server 8000

# or Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to Vercel

1. Push this repo to GitHub.
2. Go to [vercel.com](https://vercel.com), sign in with GitHub, and choose **Add New → Project**.
3. Import the repo. Leave the framework preset as **Other**, with no build command and no output directory.
4. Click **Deploy**.

Every push to `main` redeploys automatically. Or use the CLI:

```bash
npm i -g vercel
vercel --prod
```

The site also works on any static host, such as GitHub Pages or Netlify.

## Customizing

Everything lives in `index.html`:

| To change | Look for |
| --- | --- |
| Colors, fonts | the `:root` and `[data-theme="light"]` variables at the top of `<style>` |
| Name, intro, roles | the `<header class="hero">` block, and the `roles` array in the script |
| Projects | the `<article class="card">` blocks inside `#projects` |
| Experience, education | the `.tl` and `.edu` blocks inside `#experience` |
| Skills | the `.grp` blocks inside `#stack` |
| Email, social links | the `#contact` footer, and the `email` variable in the script |
| Resume button | the `#resume` link in the hero |

Fonts (Cinzel, Plus Jakarta Sans, JetBrains Mono) load from Google Fonts, with system fallbacks if offline.

## Contact

- Email: [11.rizwan.mhd@gmail.com](mailto:11.rizwan.mhd@gmail.com)
- GitHub: [github.com/11-rizwan](https://github.com/11-rizwan)
