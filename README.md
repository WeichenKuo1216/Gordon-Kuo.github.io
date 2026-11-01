# Wei-Chen (Gordon) Kuo — personal homepage

A minimal, five-page academic website balancing operations research and professional engineering. Plain HTML and CSS, no dependencies, build step, tracking, or JavaScript required. Native HTML disclosure controls make research summaries expandable.

## Files

```text
index.html            Home, research interests, contact
research.html         Research topics and expandable summaries
resume.html           Education, ASML/IMS experience, CV placeholder
projects.html         Selected project descriptions
courses.html          Coursework and materials placeholders
assets/styles.css     Responsive layout, print styles, colors
assets/favicon.svg    Initial-based favicon
.nojekyll             Serve static files directly on GitHub Pages
README.md             Setup and content checklist
```

## Preview

Open `index.html` directly, or run `python -m http.server 8000` in this folder and visit http://localhost:8000. Stop the server with Ctrl+C.

## Intended repository and URL

Repository: https://github.com/WeichenKuo1216/Gordon-Kuo.github.io

With the current owner and repository name, the site is a **project site** at https://weichenkuo1216.github.io/Gordon-Kuo.github.io/ . A repository name alone does not create a new GitHub username. The address https://gordon-kuo.github.io/ requires the GitHub account or organization `Gordon-Kuo` and its corresponding user-site repository, or use a custom domain.

All local links and assets use relative paths, so both project sites and user sites work.

## Publish after reviewing the content

1. Upload all five HTML files, the `assets` folder, and `.nojekyll` into the repository root on `main`. README and .gitignore may also be included. Keep the folder structure.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select **main** and **/(root)**, then **Save**.
5. Wait for GitHub's Pages deployment to finish, then open the URL shown in Settings → Pages. Later pushes to `main` publish updates automatically.

Official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

No custom domain or deployment workflow is needed. This folder has not been published by creating these files.

## Page structure

Navigation uses real separate pages: Home, Research, Resume, Projects, Courses. Research opens its own page; Home retains interests and contact; Resume holds education and engineering experience. Courses deliberately lists no invented course enrollments. Each page marks its current navigation link.

## Personalize before publishing

Content is based on the supplied brief and topics recovered from the earlier planning chat. That chat was a proposal, not a CV: review every topic and description. No degree title, employment dates, job titles, achievements, paper citations, numerical results, or publication status have been inferred.

- Confirm name styling, introductory bio, interests, research topics, and selected projects.
- Add NCKU degree, department, graduation year, ASML/IMS roles and dates.
- Replace the portrait placeholder with your own image, e.g. `assets/portrait.jpg`, using `<img src="assets/portrait.jpg" alt="Wei-Chen Kuo" width="210" height="263">`. Set `width:100%;height:auto` on the image in CSS.
- Add verified research abstracts, collaborators, dates, paper links and public code links. Remove draft notices only once the associated copy is reviewed.
- Put your CV at `assets/cv.pdf` and replace the CV placeholder with `<a href="assets/cv.pdf">Download CV (PDF)</a>`.
- Replace the email placeholder with a `mailto:` link to the address you want public. The connected account's email has deliberately not been published.
- Replace the LinkedIn placeholder with your public profile link.
- Remove any topic you do not want public. Add Micron, awards, news, and further experience only with verified details.
- Update the description in `<head>` when changing the introduction. Add a canonical URL only after confirming the final live address.

## Design and maintenance

The reference direction is https://burakydin.com/: an understated academic introduction, research interests, recent work, and expandable abstracts. The reference could not be fetched in this session; the implementation follows the supplied description rather than claiming a pixel match. Original typography, muted green links, a restrained portrait area, and thin rules keep the page easy to scan.

Edit content in the corresponding HTML page; keep the shared navigation consistent across all five pages; edit colors and spacing in `assets/styles.css`. The layout changes to one column below 700px. It includes semantic landmarks, a skip link, visible keyboard focus, reduced-motion support and print styles. Missing CV/contact items are text, not broken links.

## Review checklist

- Inspect the page on desktop and a narrow phone viewport.
- Tab through navigation and links; open research summaries with Enter or Space.
- Confirm local links and assets work at the project URL above.
- Confirm every personal claim and remove draft notes after review.
- Check the PDF and public contact links once supplied.
