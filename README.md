# projects-site

The page behind **projects.northland.eco**: a private dashboard of my projects.

This repo holds only the viewer (one static `index.html`). It contains no project data.
After signing in with an emailed code, the page reads its data from Supabase, where
row-level security only returns it to allowlisted emails. Everyone else sees an empty page.

Built by `build.py` in the private `northland-inventory` repo; the nightly job there
republishes this file when the template changes. Do not edit `index.html` here.
