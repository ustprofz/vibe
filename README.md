# VIBE Lab — GitHub Pages website

A new website for VIBE Lab (Ventures in Business Engineering), University of St. Thomas, Opus College of Business. This replaces the introductory VIBE Club page with a lab-focused site, current learning tools, student showcases, shared-project examples, initiatives, people, and a development roadmap.

## Publish on GitHub Pages

1. Unzip `VIBE_Lab_GitHub.zip` on your computer.
2. Open your existing VIBE GitHub repository, or create a new public repository such as `vibe`.
3. Select **Add file → Upload files**. Upload **`index.html`**, the entire **`assets`** folder, and **`.nojekyll`** to the repository's top level. You may also include this README and the content notes. Do not upload only the ZIP or put the files inside an extra enclosing folder.
4. Commit the files to `main`.
5. Open **Settings → Pages**. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, and **Save**.
6. Wait for a successful Pages deployment, then open the published link shown in Settings → Pages. For a repository named `vibe`, it will normally be `https://ustprofz.github.io/vibe/`.

If you are replacing an existing GitHub Pages site, overwrite `index.html`, upload the new assets, and commit. Keep the existing Pages configuration if it already uses `main` and `/(root)`. The public page updates after the next successful deployment. Use a hard refresh if an old stylesheet remains cached.

**This website is entirely static.** It needs no Python service, Node build, API keys, database, or paid hosting. It links to the separate tools and student applications rather than copying their services into this repository. Its links use their existing public URLs. Assets within this website use relative paths, so it works from a GitHub project subdirectory.

GitHub's publishing documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Included sections

- VIBE Lab introduction and its faculty/staff-led, student-engaged experiential learning model.
- Financial Tools and Market Lab for high school and college learners.
- Student project showcases: ExitMatch, Big Dipper, and Exit Radar.
- Four expandable shared-project example briefs.
- Events: the Quantitative & Algorithmic Trading Hackathon.
- Initiatives: workshops and mentoring, high school outreach, and campus/industry collaborations.
- Development roadmap and clearly labelled goals through May 2028.
- Lab structure: faculty and staff leadership, student leadership, project teams, and a Board of Advisors made up of staff, faculty, and professionals.
- A separate creator credit for Jiang (Will) Zhang, including title and LinkedIn.
- Student interest form from the original page, professional contact links, and educational disclaimer.

The UST logo is bundled locally. Opus College of Business, the Opus Way of Teaching initiative, and VIBE Lab are identified throughout the page.

## Edit the site

| What to change | Where |
| --- | --- |
| Descriptions, projects, links, people, dates | `index.html` |
| Colors, typography, spacing, phone layouts | `assets/styles.css` |
| Phone menu and dated-event archive label | `assets/site.js` |
| Logo | `assets/ust-logo.png` |

To add a showcase, duplicate one `<article class="showcase-item">` and update its name, description, links, and accessible link labels. To add a shared-project example, duplicate a `<details class="project-brief">` block.

Keep future goals separate from completed outcomes. The shared-project briefs are examples, not claims of finished products. The learning tools are described as faculty-created; the three linked student demonstrations are not claimed as completed VIBE Lab commissions.

The hackathon is dated **2026**. Its badge switches to “2026 event archive” after December 5, 2026, using the America/Chicago date. To feature a later event, update its dates and text in `index.html`, then update or remove the archive-date logic in `assets/site.js`. The page deliberately leaves workshop times and rooms to current organizer communications.

If updating CSS or JavaScript, consider changing the `?v=3` suffix on the corresponding references in `index.html` to `?v=4` so returning visitors fetch the new assets.

## Local preview

You can open `index.html` directly in a browser. Alternatively, from this folder run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`. No installation or build is needed.

## Publication status

This package is ready to upload. It has not been pushed to your GitHub repository or published on your behalf. Existing external applications keep their own hosting, data connections, and availability.
