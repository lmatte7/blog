# Blog

Run these commands from the repo root (requires Ruby and Bundler).

## Setup

```sh
bundle install
```

## Build after changes

Add posts in `_posts/` as `YYYY-MM-DD-title.markdown` (copy an existing post for its front matter), then build:

```sh
bundle exec jekyll build
```

Generated files go into `_site/`.

## Local server

```sh
bundle exec jekyll serve
```

Open http://localhost:4000. Changes rebuild automatically; refresh your browser to see them. Restart the server after changing `_config.yml`. Stop with `Ctrl+C`.

## Deploy to GitHub Pages

In the repository's **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions**. Keep the custom domain set to `dumptrucksblog.com`.

The workflow in `.github/workflows/deploy-pages.yml` builds the site and deploys it on every push to `master`. You can also run it manually from the **Actions** tab using **Run workflow**. It builds `_site/` from source, so generated files do not need to be committed for deployment. No additional secrets are required.
