# PerDrobe

Official academic project website source for TED University, Department of Computer Engineering. CMPE 491 – Capstone Design Project I, with continuation in CMPE 492, Academic Year 2026–2027.

**Status:** proposal stage. The academic website is deployed on GitHub Pages at https://beratergun.github.io/perdrobe/ . Deployment was verified on 16 October 2026. The publishing source is `main` / `/(root)`. The application, recommendation experiments and outcomes described on the site are planned work.

Team: Yiğit Özmut, Atay Aktürk and Seyid Berat Ergün. Supervisor: Ayşenur Birtürk. Both jury members are to be determined by the supervisor.

## Structure

```text
perdrobe/
  index.html
  styles.css
  .nojekyll
  .gitignore
  README.md
  assets/
    favicon.svg
    architecture.svg
    architecture.png
  documents/
    PerDrobe_CMPE491_Project_Proposal.pdf
    PerDrobe_CMPE491_Technical_Annex.pdf
  proposal/
    PerDrobe_CMPE491_Project_Proposal.docx
    PerDrobe_CMPE491_Technical_Annex.docx
    PerDrobe_LMS_Project_Description.txt
    PerDrobe_LMS_Submission.txt
```

No framework, build step, JavaScript, backend, analytics, API key or external font is required. All internal resources use relative paths and work under the `/perdrobe/` project prefix. Student numbers are omitted from the visible team section; the downloadable proposal includes all three student numbers supplied by the team.

## Publish with GitHub Pages

1. Sign in as `beratergun` and create a **public** repository named `perdrobe`. If using the commands below, create an empty repository without an initial README. If the repository already exists, inspect its contents and integrate these files rather than replacing unrelated work.
2. Copy the **contents** of this `perdrobe` folder into the repository root. `index.html` must be at the root, not inside another `perdrobe` directory. Preserve `.nojekyll` and the `documents`, `proposal` and `assets` folders.
3. With Git installed, run these commands from the copied repository directory:

```sh
git init -b main
git add .
git commit -m "Add PerDrobe academic project website and proposal"
git remote add origin https://github.com/beratergun/perdrobe.git
git push -u origin main
```

Authenticate using your normal GitHub sign-in method. Do not put tokens in project files. Alternatively, use GitHub's upload-files interface; check that nested folders and `.nojekyll` are present.

4. In the repository, open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, branch **main**, folder **/(root)**, then **Save**.
5. Wait for the Pages deployment to finish. Inspect the deployment status in the repository's Actions or Pages interface if it fails.
6. Open https://beratergun.github.io/perdrobe/ and verify that the page displays, the navigation reaches each section and **View project proposal** opens the correct PDF. Also test a narrow mobile window. A locally working page is not proof of public deployment.
7. Only after verifying the public site and PDF, submit that URL in the LMS.

GitHub's official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Preview locally

Open `index.html` directly, or run a static server from this directory (for example `python -m http.server 8000` if Python is installed) and visit `http://localhost:8000/`. No dependency installation is needed.

## Update reports without changing the project URL

- Edit the DOCX in `proposal/`, export a new PDF and replace `documents/PerDrobe_CMPE491_Project_Proposal.pdf` using the same filename. Keep the DOCX and PDF consistent. Update the visible proposal date in `index.html` if the revision date changes.
- Add subsequent reports and presentations under `documents/`. Turn the corresponding non-clickable “Coming later” row in `index.html` into an anchor pointing to the real file. Do not add a link until the file exists.
- Update scope, roadmap and results in the proposal and site together. Keep planned work distinct from demonstrated implementation and measured outcomes. Set both jury names only when the supervisor confirms them.
- Keep `index.html` at the root and retain the repository name `perdrobe`. Commit and push updates to `main`. The Pages address will remain the same.
- Check every document link after each deployment. On a case-sensitive host, filename capitalization must match exactly.

## Content and data boundaries

Core scope includes digital wardrobe management, personalized outfits, supported size guidance, Outfit Remix, wardrobe-aware shopping and lightweight social preference signals. Duo Match and visual extensions are conditional. No retailer API access, dataset selection, partnership, experimental result or institutional approval is asserted. No software license has been selected for the future application; do not infer one from the public website.

## Website presentation

The page uses local serif and sans-serif fonts, a warm paper background and restrained accent colors. The Outfit Remix example is illustrative and does not display a measured result. The architecture is rendered as responsive HTML layers. Navigation remains available while scrolling, with visible keyboard focus and reduced-motion support. The A/B/C comparison adapts to narrow screens without horizontal scrolling.

## Course proposal and technical annex

The main Project Proposal is one page: project name, live webpage URL, team members, supervisor, jury status and exactly two project-description paragraphs. The course instruction limits the description to 1–2 paragraphs; it does not state a total proposal page limit. One page is the chosen concise presentation, not a claimed mandatory page count.

The previous eight-page document is retained separately as a Technical Annex. It provides optional engineering detail and is not presented as an additional course requirement. Use `proposal/PerDrobe_LMS_Submission.txt` for the form fields and `proposal/PerDrobe_LMS_Project_Description.txt` for the description alone. Both jury names must be confirmed by the supervisor before the names requirement can be completed.

The course instruction also requires LMS submission and email delivery to the supervisor and jury. Publishing the page does not perform those submission steps. No email or LMS submission was made by this package.

## Official logo and final spacing revision

The primary proposal embeds TED University's official English horizontal logo, obtained from https://www.tedu.edu.tr/themes/custom/tedu/tedu-colorful-en.svg via the university's official corporate identity materials (https://www.tedu.edu.tr/en/kurumsal-kimlik). The logo is reproduced in its original colors and aspect ratio. It does not imply institutional approval of the project.

The main proposal remains one A4 page. Its unchanged 207-word project description consists of exactly two paragraphs, with 1.20 line spacing and 12 pt paragraph spacing. The editable Word file was exported using Microsoft Word, and the rendered PDF page was visually inspected. The project URL and the footer link to the Technical Annex are active PDF hyperlinks. Literature references remain in the annex; the main proposal describes planned project work and introduces no unsupported research claims.
