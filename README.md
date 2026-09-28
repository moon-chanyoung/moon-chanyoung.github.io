# moon-chanyoung.github.io

Personal website of Chanyoung Moon, built on [AcademicPages](https://github.com/academicpages/academicpages.github.io) (Jekyll) and served by GitHub Pages at <https://moon-chanyoung.github.io>.

## Updating content

Most of the page is generated from the YAML files in `_data/`:

| File | Section |
| --- | --- |
| `news.yml` | News (newest first) |
| `research.yml` | Research intro and the three area cards |
| `publications.yml` | Publications (add `links:` with `label`/`url` pairs for PDF, code, slides) |
| `experience.yml` | Experience |
| `education.yml` | Education |
| `honors.yml` | Honors & Awards |
| `activities.yml` | Activities |
| `navigation.yml` | Top menu |

The hero (name, role, one-line statement, notice), intro paragraph, profile buttons, and contact box are in `_pages/about.md`.

Files:

- CV: `files/Chanyoung_Moon_CV.pdf` (overwrite it with the same name to update every CV link)
- Profile photo: `images/profile.jpg` (square, at least 400 px)
- Favicons: `images/favicon*`, `images/apple-touch-icon-180x180.png`

The single-page layout is `_layouts/home.html`; its styles are in `_sass/layout/_home.scss`. Colors are CSS variables at the top of that file (`--cm-accent` sets the accent color for both light and dark themes).

## Local preview

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>. Pushing to `main` redeploys the site.
