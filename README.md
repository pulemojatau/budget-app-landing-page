# BudgetFlow — Landing Page

A clean, modern, responsive landing page for the **BudgetFlow** Flutter personal finance app.

Live demo: *(add your Cloudflare Pages URL here)*

---

## Project Structure

```
budget-app-landing-page/
├── index.html          # Main landing page
├── styles.css          # All styles (dark theme)
├── main.js             # Interactions (nav, lightbox, scroll reveal)
├── screenshots/        # App screenshots used in the gallery
│   ├── dashboard1.jpeg
│   ├── dashboard2.jpeg
│   ├── income.jpeg
│   ├── fixed-expenses.jpeg
│   ├── budget-allocation.jpeg
│   ├── categories-overview.jpeg
│   ├── spending.jpeg
│   ├── adding-funds.jpeg
│   ├── goals.jpeg
│   ├── transaction-histrory.jpeg
│   └── settings.jpeg
└── README.md
```

---

## Deploying to Cloudflare Pages

### Option 1 — Connect GitHub (recommended)

1. Push this repo to GitHub.
2. Go to [Cloudflare Pages](https://pages.cloudflare.com/) → **Create a project**.
3. Connect your GitHub account and select this repository.
4. Set build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (root)
5. Click **Save and Deploy**.

Cloudflare will deploy on every push to `main` automatically.

### Option 2 — Direct upload (no Git required)

1. Go to [Cloudflare Pages](https://pages.cloudflare.com/) → **Create a project** → **Direct Upload**.
2. Name your project (e.g. `budgetflow`).
3. Drag and drop the entire project folder (or zip it and upload).
4. Click **Deploy site**.

Your site will be live at `https://budgetflow.pages.dev` (or your chosen subdomain).

---

## Updating Links

Before deploying, update these placeholders in `index.html`:

| Placeholder | Where | What to replace with |
|---|---|---|
| `https://github.com/mojatau` | Nav, Hero, About, Footer | Your actual GitHub repo URL |
| Download APK `href="#"` | Hero CTA button | Direct link to your `.apk` file |
| Portfolio `href="#"` | About section | Your portfolio URL |

---

## Tech

- Pure HTML, CSS, and vanilla JavaScript — no build step, no dependencies
- Dark modern theme with Inter font (loaded from Google Fonts)
- Fully responsive (mobile, tablet, desktop)
- Accessible: semantic HTML, ARIA labels, keyboard navigation
- Screenshot lightbox with keyboard/click-outside dismiss
- Scroll-reveal animations via IntersectionObserver
