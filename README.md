# Mohamed Yasin — Portfolio Website

A static HTML5/CSS3 portfolio (minimal vanilla JS for nav + scroll effects). No frameworks, no build step.

## File structure

```
/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── images/
│   └── profile.jpg      ← your hero photo (already added)
├── assets/
│   └── (put your resume PDF here)
└── README.md
```

## Before you publish — fill these in

Search the project for these placeholders and replace them:

| Placeholder | Where | Replace with |
|---|---|---|
| `ADD-LINKEDIN-USERNAME` | `index.html` (Hero + Contact) | Your LinkedIn username, e.g. `mohamedyasin` |
| `ADD-GITHUB-USERNAME` | `index.html` (Hero + Contact) | Your GitHub username |
| `mohamedyashinmn@gmail.com` | `index.html` (Contact section, appears twice) | Your real email address |
| `assets/Mohamed-Yasin-Resume.pdf` | `index.html` (View Resume button) | Add your actual resume PDF at `assets/Mohamed-Yasin-Resume.pdf`, or update the path |

Use find-and-replace in your code editor (Ctrl/Cmd+Shift+F) to catch every instance.

## Replacing images

- **Profile photo:** `images/profile.jpg` is already set from the photo you provided. To swap it, replace that file with a new image of the same name (ideally a portrait, 1000px wide or more, JPG).
- **Resume PDF:** drop your resume into `assets/Mohamed-Yasin-Resume.pdf` (create the `assets` folder if it isn't there yet).

## Running locally

No build tools needed — just open `index.html` in a browser, or serve it locally:

```bash
# Python
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Deploying to Vercel (recommended, free)

1. Create a free account at [vercel.com](https://vercel.com).
2. Install the CLI: `npm install -g vercel` (or use the Vercel dashboard's drag-and-drop deploy).
3. From inside this project folder, run:
   ```bash
   vercel
   ```
4. Follow the prompts (accept defaults — it's a static site, no framework to select).
5. Vercel gives you a live URL immediately; running `vercel --prod` promotes it to your production domain.

**Or via the dashboard (no CLI):**
1. Go to vercel.com → "Add New Project" → "Deploy" tab → drag and drop this whole folder (or connect a GitHub repo containing it).
2. Leave build settings blank/default — Vercel auto-detects a static site.

## Deploying to Netlify (alternative, free)

1. Create a free account at [netlify.com](https://netlify.com).
2. Go to **Sites → Add new site → Deploy manually**.
3. Drag and drop this project folder onto the upload area.
4. Netlify publishes it instantly with a live URL.

**Or via GitHub:** push this folder to a GitHub repo, then in Netlify choose "Import from Git," pick the repo, leave the build command empty and publish directory as `/` (root).

## Updating content later

All text content lives directly in `index.html`, organized by section with HTML comments (`<!-- ============ HERO ============ -->` etc.) so you can find things quickly. Colors, spacing, fonts, and radii are controlled by CSS variables at the top of `css/style.css` under `:root` — change a value there and it updates everywhere it's used.
