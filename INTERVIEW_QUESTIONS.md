# Technical Interview Questions & Answers - TASK 6: GitHub Pages

---

### Q1: What is GitHub Pages?
**Answer:**
GitHub Pages is a static site hosting service provided directly by GitHub. It takes HTML, CSS, and JavaScript files directly from a repository, runs the files through an optional build process, and publishes them as a live website on the internet for free under a `github.io` domain or a custom domain.

---

### Q2: Can you host dynamic apps here?
**Answer:**
**No.** GitHub Pages only supports static web pages (client-side HTML, CSS, JavaScript, and static assets). It does not support server-side languages or runtimes (like Node.js Express, Python Django/Flask, PHP, Ruby on Rails) or backend database connections (like MySQL, MongoDB). However, you can host static frontend builds of React, Vue, or Angular that connect to external APIs via client-side fetch calls.

---

### Q3: What are the limits of GitHub Pages?
**Answer:**
The key limits of GitHub Pages include:
1. **Repository Size Limit**: Recommended maximum repository size of 1 GB.
2. **Bandwidth Limit**: Soft bandwidth limit of 100 GB per month.
3. **Build Limit**: Maximum of 10 builds per hour.
4. **No Server-Side Code**: Only static assets can be executed.
5. **Usage Policy**: It cannot be used for high-frequency e-commerce transactions, commercial bulk mining, or illegal activities.

---

### Q4: How do you update the website?
**Answer:**
To update the website, simply make changes to your local files (e.g., `index.html` or `style.css`), commit the changes, and push them to the designated GitHub Pages publishing branch (e.g., `git push origin main`). GitHub Actions automatically triggers a background deployment and updates the live site within a minute.

---

### Q5: What happens when you delete the repo?
**Answer:**
If you delete the GitHub repository, the GitHub Pages deployment is permanently removed, and the live website immediately goes offline, returning a `404 Not Found` error to visitors.

---

### Q6: What is the default file that loads?
**Answer:**
The default file that loads when a user visits the root URL of your GitHub Pages site is **`index.html`** (or `index.md`). If an `index.html` file does not exist at the root or selected publishing folder, GitHub Pages will look for a `README.md` file or return a 404 error.

---

### Q7: Can you use a custom domain?
**Answer:**
**Yes.** GitHub Pages fully supports custom domains (e.g., `www.yourname.com` or `portfolio.yourname.com`). You configure it by:
1. Adding a `CNAME` record in your DNS provider pointing to `<username>.github.io`.
2. Entering your custom domain under **Repository Settings > Pages > Custom domain** and enabling **Enforce HTTPS**.
