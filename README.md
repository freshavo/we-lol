# WE / 26 — Conference Planner

A single-file, mobile-friendly personal planner for WE26. It includes expenses and reimbursements, applications, workshops, a daily itinerary, company priorities, and networking contacts.

## Publish using GitHub Pages

1. Log in to GitHub and create a new **public** repository, for example `swe-conference-planner`. (On a free GitHub plan, GitHub Pages requires a public repository.)
2. Upload **`index.html`** to the **top level** of the repository, then commit it. You may also upload this README, but do **not** upload expense backups, receipts, or any personal data.
3. Go to **Settings → Pages** in the repository.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Choose the **`main`** branch and **`/(root)`** folder, then click **Save**.
6. Your site will be published at `https://YOUR-USERNAME.github.io/swe-conference-planner/` (replace `YOUR-USERNAME` and the repository name with yours). Check **Settings → Pages** for the actual published URL.

To update the published planner later, replace the repository's `index.html` with the new version and commit changes; GitHub Pages redeploys it.

## Budget math

- **Money left to spend** = budget − already-paid expenses (expenses with any reimbursement status except `Planned`).
- **Left after planned purchases** = budget − already-paid expenses − planned expenses.
- **Reimbursed** is a tracker, not extra room in your budget. Reimbursement funds do not replenish the approved funding cap. The default $1,000 amount can be edited from the Expenses page or Dashboard.
- This is a **spending budget**, **not a bank balance** or confirmation of what the WIN Empowerment Fund will reimburse. Eligibility and payment arrangements need to be checked separately.

## Keep your data safe

Data is stored locally in your **browser**, not in GitHub. It persists when you close and reopen the site in the same browser, as long as browser storage is retained. It does **not** sync between computers, browsers, or private-browsing sessions.

**Before moving from the downloaded HTML file to GitHub Pages:** open the old planner and click **Export backup**. On the live GitHub Pages site, choose **Import backup** and select that JSON file. Importing **replaces** the existing data on the receiving browser, so export first if the site already contains changes.

Never commit the exported JSON backup to a public GitHub repository. It may contain private expense, recruiter, or job-application details.

## Tech

No build step, third-party libraries, backend, or GitHub login required for site visitors. The website uses vanilla HTML/CSS/JavaScript and `localStorage`.
