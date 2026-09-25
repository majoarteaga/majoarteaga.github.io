# majoarteaga.github.io

Personal academic website of María José Arteaga-Garavito
(Assistant Professor of Finance, Mays Business School, Texas A&M University).

Live at <https://majoarteaga.github.io>. Built with Jekyll (originally based on the
[al-folio](https://github.com/alshedivat/al-folio) theme, MIT license; see `LICENSE`),
restyled with a clean look in Computer Modern Serif.

## Where things live

| What | File |
|---|---|
| Home page (bio, photo, links) | `_pages/about.md` |
| Research page | `_pages/research.md` |
| Teaching page | `_pages/teaching.md` |
| News items (one per file, newest first) | `_news/announcement_*.md` |
| CV (menu "cv" opens this PDF) | `assets/pdf/CV_MJAG.pdf` |
| Papers, slides, videos, photo | `assets/pdf/`, `assets/video/`, `assets/img/` |
| Look and feel (fonts, links, spacing) | `assets/css/main.scss` |
| Name, email, social handles, column width | `_config.yml` |

## Updating

- **CV:** replace `assets/pdf/CV_MJAG.pdf` with a file of the same name.
- **News:** copy an existing `_news/announcement_*.md`, change the `date:` and the text.
- Commit and push to `master`; the `deploy` GitHub Action builds the site into the
  `gh-pages` branch (about 2–3 minutes).

## Previewing locally (optional)

The GitHub build uses Ruby 3.2. On this Mac, Ruby 3.2 is installed via Homebrew (`ruby@3.2`):

```bash
export PATH=/opt/homebrew/opt/ruby@3.2/bin:$PATH
bundle config set --local path ~/.gem-cache/majoarteaga
bundle install
bundle exec jekyll serve    # open http://localhost:4000
```

`.bundle/`, `Gemfile.lock`, `_site/` and `.jekyll-cache/` are git-ignored build artifacts.
