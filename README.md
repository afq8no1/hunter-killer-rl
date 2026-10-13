# Hunter-Killer · Q-Learning Demo

Three hunters with limited vision (6 cells, line-of-sight) learn via tabular
Q-learning to track and corner an assassin. Runs entirely client-side: no backend,
no build step. Play as the assassin with arrows/WASD or swipe.

## Run locally
    npm run dev        # serves ./public

## Deploy to Vercel
Option A, CLI:
    npm i -g vercel
    vercel            # preview
    vercel --prod     # production

Option B, GitHub:
1. Push this folder to a GitHub repo.
2. vercel.com > Add New > Project > import the repo.
3. Leave Framework Preset as "Other". No build command. Output directory is read from vercel.json (public).
4. Deploy.

## Structure
    public/index.html   the whole app (HTML + CSS + JS)
    vercel.json         static config (output dir, headers)
