# Bo Peng's academic website

A personal academic website built with the original [al-folio](https://github.com/alshedivat/al-folio) template and its versioned Jekyll theme gems.

Intended address: **https://conancqu.github.io/**

## Publish on GitHub Pages

1. Create a **public** GitHub repository named **ConanCQU.github.io** under the ConanCQU account.
2. Upload the contents of this folder to the repository root (not an extra enclosing folder). Include `.github/workflows/deploy.yml`.
3. In **Settings → Pages → Build and deployment → Source**, select **GitHub Actions**.
4. Open the **Actions** tab and run **Deploy personal website**, or push another commit to `main` to trigger it.
5. Wait until the deployment succeeds, then visit https://conancqu.github.io/.

The workflow derives the deployment URL and path from GitHub Pages, so it also supports a project repository if its name changes.

## Edit content

| Content                  | File                      |
| ------------------------ | ------------------------- |
| Homepage                 | `_pages/about.md`         |
| Research                 | `_pages/research.md`      |
| Publications             | `_pages/publications.md`  |
| Online CV                | `_data/cv.yml`            |
| Email and GitHub links   | `_data/socials.yml`       |
| Name, URL, theme options | `_config.yml`             |
| Portrait                 | `assets/img/avatar.png` |

The content was prepared from the supplied resume and the updated admission information. Education dates, a graduate degree type, and a supervisor are omitted because they were not supplied. FlyWithMap is marked **in preparation for CVPR**, not as an accepted publication. The original resume PDF and its phone number are not included in the website.

## Local preview

Requires Ruby 3.2 or later, Bundler, and Node.js.

```sh
bundle install
npm ci
bundle exec jekyll serve --baseurl ''
```

Open http://localhost:4000/.

## License and theme

al-folio is distributed under the MIT license, preserved in `LICENSE`. The original theme attribution remains in the footer. Theme layouts, styles, and scripts are supplied by the pinned gems; no local runtime overrides have been added.
