# Broken Arrow Towing

Static towing website with local, optimized images.

## Deploy to Vercel

Import `HasebRehman/brokenarrow` into Vercel and deploy the `main` branch.
Use the repository root as the Root Directory. The committed `vercel.json`
selects the Other framework preset, skips the build step, and serves
`brokenarrowtowing.html` at `/`. Images are served from `/images/`.

To preview locally, run `python -m http.server 8000` and open
`http://localhost:8000/brokenarrowtowing.html`.

## Contact form integration

The existing contact form posts to `/wp-json/nt/v1/contact`, which requires
the original WordPress backend. Static Vercel hosting does not provide that
endpoint. Connect a working backend and configure the Turnstile domain
before using the contact form in production.
