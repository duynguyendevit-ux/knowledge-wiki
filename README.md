# My Wiki

Personal knowledge base built with Obsidian + Quartz v4.

## 🌐 Live Site

https://duynguyendevit-ux.github.io/knowledge-wiki/

## 📝 Content

- **Fireworks:** Game design reference for mortar tubes and racks
- More topics coming soon...

## 🛠️ Tech Stack

- **Editor:** Obsidian
- **Generator:** Quartz v4
- **Deploy:** GitHub Actions → GitHub Pages

## 🚀 Workflow

1. Edit markdown files in Obsidian (or any editor)
2. Push to `main` branch
3. GitHub Actions auto-build and deploy
4. Live in ~1 minute

## 📁 Structure

```
.
├── fireworks/              # Fireworks technical references
├── .obsidian/              # Obsidian vault config
├── .github/workflows/      # GitHub Actions
└── quartz.config.ts        # Quartz configuration
```

## ✍️ Writing Guidelines

- Use YAML frontmatter for metadata:
  ```yaml
  ---
  title: Page Title
  tags: [tag1, tag2]
  date: 2026-06-07
  ---
  ```
- Wiki links: `[[page-name]]`
- Standard Markdown + Obsidian flavor

## 🔧 Maintenance

- Token: `ghp_RJ...bZTR` (repo + workflow scopes)
- Deployment branch: `main` (allowed in github-pages environment)
- Build time: ~45s
