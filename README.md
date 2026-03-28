# Jack Dechow Personal Website

Personal academic website for Jack Dechow, built with Jekyll and the Minimal Mistakes remote theme, and deployed via GitHub Pages at [dechowjack.github.io](https://dechowjack.github.io).

## Structure

- `index.md`: homepage content and hero configuration
- `_pages/`: site pages such as research, publications, resources, and CV
- `_data/navigation.yml`: top-level navigation
- `assets/css/main.scss`: site-level style overrides
- `assets/images/`: profile photos, page imagery, and research figures
- `assets/files/`: downloadable files such as the CV PDF

## Local Development

This site uses Bundler-managed Jekyll dependencies.

1. Install Ruby `3.0+` and Bundler.
2. Install dependencies:

```bash
bundle install
```

3. Serve locally:

```bash
bundle exec jekyll serve
```

4. Open the local URL printed by Jekyll, usually `http://127.0.0.1:4000`.

## Notes

- GitHub Pages builds the site from this repository using the gems declared in `Gemfile` and `_config.yml`.
- The current repo does not use blog posts or Atom feeds; it is maintained as a static research/personal site.
- Large visual assets should be resized or compressed before committing so page loads remain fast.

## Maintenance Checklist

- Keep page `excerpt` values populated so metadata is useful in search/social previews.
- Prefer putting reusable styling in `assets/css/main.scss` instead of inline HTML `<style>` blocks.
- Verify external links periodically, especially profile links and DOI targets.
