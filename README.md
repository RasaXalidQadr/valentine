# Valentine Mini-Site

This small static site shows a playful "Can I be your Valentine?" card with two buttons. It includes a GIF of a cat and a confetti celebration when "Yes" is clicked.

How to publish on GitHub Pages

1. Create a new GitHub repository (public or private with Pages enabled).
2. From your project folder (`C:\Users\rasax\OneDrive\Desktop\val`) run these commands in PowerShell:

```powershell
# Initialize git (if you haven't already)
git init
git add .
git commit -m "Initial Valentine site"
# Replace <your-remote-url> with the repo HTTPS URL from GitHub (e.g. https://github.com/you/repo.git)
git remote add origin <your-remote-url>
# Push to the main branch (create branch if necessary)
git branch -M main
git push -u origin main
```

3. Enable GitHub Pages:
- Open your repository on GitHub.
- Go to `Settings` → `Pages` (or `Pages` in the left sidebar).
- Under "Build and deployment" choose `Deploy from a branch` and set the branch to `main` and folder to `/ (root)`.
- Save. GitHub will publish your site at `https://<your-username>.github.io/<repo-name>/` (or for a user/org Pages site, at `https://<your-username>.github.io/`).

Notes
- `index.html` is included so the site is served at the repo root.
- Ensure the `cat-hugs.gif` file is in the project root so the GIF displays on the site.

Alternative quick deploy: Use Netlify Drop by zipping the project folder and dragging it to https://app.netlify.com/drop for a fast anonymous deploy.
