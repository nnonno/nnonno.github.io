# nnonno.github.io

Source for Yifu Wu's personal website: https://nnonno.github.io/

Built with [Hugo](https://gohugo.io/) (v0.145.0 extended) and the Hugo Blox Academic CV theme.
GitHub Actions (`.github/workflows/publish.yaml`) builds the site and deploys it to GitHub Pages on
every push to `main`.

## Local preview

```bash
hugo server
```

## Where things live

- `content/authors/admin/_index.md`: bio, education and work history
- `content/_index.md`: homepage sections
- `config/_default/`: site configuration (`params.yaml`, `menus.yaml`, ...)

## Credits

Theme: [Hugo Blox Academic CV](https://github.com/HugoBlox/theme-academic-cv), MIT License (see
`LICENSE.md`).
