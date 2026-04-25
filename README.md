# simonecasolo.github.io

Personal academic / portfolio site built with [al-folio](https://github.com/alshedivat/al-folio).

## Local preview

Use Docker (recommended by al-folio):

```bash
docker compose pull
docker compose up
```

Then open `http://localhost:8080`. Alternatively install Ruby 3.3+ and run `bundle install && bundle exec jekyll serve`.

## Deploy

GitHub Actions builds the site and pushes to the `gh-pages` branch. In the repository **Settings → Pages**, set the publishing source to the **`gh-pages`** branch (not `master`).
