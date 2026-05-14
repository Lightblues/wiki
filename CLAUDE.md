# Wiki

MkDocs-based personal knowledge base. Deployed to GitHub Pages via `notes.easonsi.site`.

## Quick Reference

- Theme: Material for MkDocs
- Python: 3.12+
- Deploy target: `Lightblues/wiki` repo → gh-pages branch → GitHub Pages
- Custom domain: `notes.easonsi.site` (CNAME → `lightblues.github.io`)
- Images: `cdn.jsdelivr.net/gh/lightblues/assets@main/wiki/...`

## Common Commands

```bash
pip install mkdocs mkdocs-material pymdown-extensions
mkdocs serve          # local preview (localhost:8000)
mkdocs build --clean  # build to site/
```

## Image Workflow

Images live in `Lightblues/assets` repo under `wiki/` directory.

```bash
# Add new images
cp new-image.jpg ~/Projects/output/assets/wiki/{topic}/
cd ~/Projects/output/assets && git add wiki/ && git commit && git push
```

URL pattern: `https://cdn.jsdelivr.net/gh/lightblues/assets@main/wiki/{topic}/{file}`

## Coding Style

- Docs in `docs/` as Markdown
- Navigation structure defined in `mkdocs.yml`
- Images referenced via jsdelivr CDN (assets repo)

## Related Projects

- Blog: `~/Projects/output/blog` → `blog.easonsi.site`
- Assets: `~/Projects/output/assets` → jsdelivr CDN
- DNS managed in blog repo: `~/Projects/output/blog/scripts/dns/`
