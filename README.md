# c-brugo.github.io

Personal website of Carlo Brugo, published with GitHub Pages at https://c-brugo.github.io.

Built with Jekyll, no theme. Every push to `main` updates the site.

## Updating content

All content lives in `_data/`; the pages read from these files, so there is no HTML to touch.

| File | Page |
|---|---|
| `experience.yml` | Experience |
| `education.yml` | Experience and home page |
| `activities.yml` | Activities |
| `certifications.yml` | Certifications |
| `projects.yml` | Projects |
| `skills.yml` | Home page |

Each file has an example at the top. For instance, to add a certification append to `_data/certifications.yml`:

```yaml
- name: AWS Certified Cloud Practitioner
  issuer: Amazon Web Services
  date: Oct 2026
  url: https://link-to-verify
```

Only `name` is required. When `projects.yml` is empty the Projects page shows a "coming soon" message.

Text on the home page is in `index.html`; name, email and social links are in `_config.yml`.

## Preview locally

```sh
gem install jekyll jekyll-seo-tag jekyll-sitemap
jekyll serve
```

Then open http://localhost:4000.
