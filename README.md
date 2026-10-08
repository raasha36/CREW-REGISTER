# Crew Register — GitHub Pages prototype

## New admin workflow
You do NOT need to send employee files to ChatGPT every time.

Open **Admin** inside the app:
- Employee Master → choose KOAA/SDAH → upload `.xlsx`, `.xls`, or `.csv`
- The importer auto-detects ID, NAME and up to 3 phone columns.
- Add/edit/delete employees from the browser.
- Download the current employee directory as Excel.
- Train Lists → upload the SDAH workbook when you have it.
- The importer supports Batch A/B/C workbook sheets and train/ID-slot detection.

## Employee file examples
Accepted column names include:
- ID / ID Card No / Employee ID
- NAME / NAME OF STAFF / Full Name
- PHONE / PHONE 1 / PHONE 2 / PHONE 3

## Current storage
This is still a prototype. Data is stored in browser localStorage and is NOT shared between phones.

## Admin login
The current prototype has a temporary frontend login. Open `index.html` and find:
`ADMIN_EMAIL`
`ADMIN_PASSWORD`

The email is pre-set to the admin email already specified for this project. The password is intentionally a placeholder because the admin password is not present in the project context available to this build. Change it before publishing.

This is NOT secure authentication. When we add cloud storage, admin authentication will be moved server-side.

## GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html` to the repository root using GitHub's website.
3. Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
4. Open the generated Pages URL.
5. On Android Chrome use ⋮ → Add to Home screen / Install app.

No Git installation is required.
