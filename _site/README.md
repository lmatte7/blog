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
