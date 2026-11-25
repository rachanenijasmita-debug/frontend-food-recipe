# RecipeNest — Food Recipe App (Project 27)

A responsive **React + Vite** recipe-sharing frontend for the SDC review. It uses CSS Grid/Flexbox and browser **LocalStorage** for demo persistence.

## Modules and review demonstration

### User module
- Sign up and log in (accounts stored in LocalStorage)
- Browse/search recipes by title, ingredients, cuisine and dietary preference
- Filter recipes by cuisine and diet
- Open recipe details with ingredients and step-by-step preparation
- Save/unsave favorite recipes
- Submit recipes, rate recipes and create personal collections
- Share a recipe title using the browser clipboard

### Admin module
- Admin-only dashboard and navigation
- View recipe, user and saved-recipe counts
- Delete recipes
- View registered community accounts

## Demo admin account
- Email: `admin@recipenest.com`
- Password: `admin123`

For a user-module demonstration, sign up with a new email address, then show saved recipes, collections and recipe submission.

## Run locally
Requires Node.js (LTS recommended).

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. Verify a production build with:

```bash
npm run build
npm run preview
```

## Deploy to Vercel
1. Push this project folder to a GitHub repository (do not upload `node_modules` or `.env` files).
2. Sign in to Vercel and choose **Add New → Project**.
3. Import the GitHub repository.
4. Confirm framework preset **Vite**; Build command `npm run build`; Output directory `dist`.
5. Click **Deploy**. The included `vercel.json` rewrites client-side routes to `index.html`.
6. Open the generated deployment URL and test signup/login, user features and admin login. Copy the GitHub repository URL and Vercel URL for review.

## Storage / academic project note
Data is stored in the current browser's LocalStorage and is not shared between browsers or devices. This is a frontend demonstration, not production authentication: passwords are stored locally in plain text. Do not use real or sensitive passwords. A production app should use a secure backend and hashed passwords.

## Main files
- `src/main.jsx` — React components, User/Admin modules, authentication and LocalStorage logic
- `src/style.css` — responsive styling
- `index.html` — Vite entry document
- `vercel.json` — Vercel SPA rewrite
"# frontend-food-recipe" 
