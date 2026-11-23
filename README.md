# open-he-mchose.github.io

> **⚠️ AI-generated content.** The configuration in this repository and the documentation it publishes were
> produced almost entirely by an AI assistant (Claude, by Anthropic), directed and tested by the maintainer.

Website of the [open-he-mchose](https://github.com/open-he-mchose) organization:
**https://open-he-mchose.github.io/**. Unofficial, not affiliated with MCHOSE.

This repository holds only the site configuration. The content is the Markdown of
[open-he-mchose/docs](https://github.com/open-he-mchose/docs) — edit pages there.

## How it is published

`.github/workflows/pages.yml` checks out this repository and `open-he-mchose/docs` side by side, builds the
site with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) in strict mode (broken links
fail the build) and deploys it to GitHub Pages. It runs on every push here, daily at 03:17 UTC, and on demand
(Actions → *Publish site* → *Run workflow*).

One-time setup: Settings → Pages → Source: **GitHub Actions**.

## Local preview

```sh
# directory layout: open-he-mchose/{docs, open-he-mchose.github.io}
python3 -m venv ../.venv-mkdocs && ../.venv-mkdocs/bin/pip install -r requirements.txt
../.venv-mkdocs/bin/mkdocs serve        # http://127.0.0.1:8000/
```

The navigation (order of pages) is in `mkdocs.yml`: add new pages of `docs` there.
