# Wiki

MkDocs-based personal knowledge base. Deployed to `lightblues.github.io/wiki`.

## Quick Reference

- Theme: Material for MkDocs
- Python: 3.10+
- Deploy target: `Lightblues/wiki` repo (gh-pages branch)

## Common Commands

```bash
pip install mkdocs mkdocs-material pymdown-extensions
mkdocs serve          # local preview (localhost:8000)
mkdocs build          # build to site/
```

## Coding Style

- Docs in `docs/` as Markdown
- Navigation structure defined in `mkdocs.yml`
- Images via jsdelivr CDN (assets repo)
