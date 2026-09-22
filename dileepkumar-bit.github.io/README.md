# Dileep Kumar Kalisetti — DevOps Engineer Portfolio

Personal portfolio site, published with GitHub Pages at **https://dileepkumar-bit.github.io/**

A single-page static site: plain HTML, CSS and JavaScript. No build step and no dependencies.

## Project structure

```
.
├── index.html                              # the whole site (markup, styles, scripts)
├── assets/
│   ├── profile.jpg                         # sidebar photo
│   ├── Dileep_Kumar_Kalisetti_Resume.pdf   # "Download Resume" button
│   └── portfolio-preview.png               # social-share image (1200×630)
├── robots.txt
├── sitemap.xml
└── .nojekyll                               # tells GitHub Pages to skip Jekyll
```

## Publish on GitHub Pages

1. Create a **public** repository named exactly `dileepkumar-bit.github.io`
   (leave "Add a README", `.gitignore` and license unchecked — they are already here).
2. From this folder:

   ```bash
   git init
   git add .
   git commit -m "Publish portfolio"
   git branch -M main
   git remote add origin https://github.com/dileepkumar-bit/dileepkumar-bit.github.io.git
   git push -u origin main
   ```

3. In the repository go to **Settings → Pages → Build and deployment**, set
   **Source** to *Deploy from a branch*, choose **main** and **/ (root)**, then **Save**.
4. After a minute or so the site is live at https://dileepkumar-bit.github.io/

## Updating the site

- **Resume:** replace `assets/Dileep_Kumar_Kalisetti_Resume.pdf` (keep the same filename), then commit and push.
- **Photo:** replace `assets/profile.jpg` (square image works best).
- **Text, skills, experience:** edit `index.html`.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000
