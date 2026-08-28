# Linkon SEN Portfolio

Static portfolio prepared for GitHub Pages.

## Publish

1. Create a **public** repository named `senlinkon009-dot.github.io`.
2. Upload `index.html`, `styles.css`, `script.js`, and the optional `assets` folder to the repository root.
3. Open **Settings → Pages** and set **Deploy from a branch**, branch **main**, folder **/(root)**.
4. The site will appear at `https://senlinkon009-dot.github.io/`.

## Add your content

- Profile photo: create `assets/profile.jpg`, then replace the placeholder block in `index.html` with `<img src="assets/profile.jpg" alt="Linkon SEN">`.
- Projects: replace the placeholder project titles, descriptions and `href="#"` links.
- Certificates: put certificate files in `assets/certificates/` and update the links.

GitHub Pages serves the frontend; Supabase provides the secure login, database, and file uploads.

## Enable the secure dashboard

1. Create a free Supabase project.
2. Open **SQL Editor**, paste `supabase-setup.sql`, and run it once.
3. In **Authentication → Users**, create the owner user `linkonsen2003@gmail.com` with your chosen password. Disable public user sign-ups in Auth settings.
4. Copy the Project URL and Publishable/anon key from **Project Settings → API** into `config.js`. Never use the `service_role` key.
5. Upload all updated files to the GitHub repository.
6. Open `https://senlinkon009-dot.github.io/admin.html` to log in and manage uploads.

The database and storage rules only permit the owner email to change content; public visitors have read-only access.
