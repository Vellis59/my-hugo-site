# port8080-blog

Static blog built with [Hugo](https://gohugo.io/) and the **PaperMod** theme.

## Requirements

- Hugo **extended** (this repo’s GitHub Pages workflow uses `hugo-version: 0.146.0`).
- Git (to pull the theme submodule).

## Theme

The theme is installed as a **git submodule**:

- `themes/PaperMod` → <https://github.com/adityatelange/hugo-PaperMod>

Clone with submodules:

```bash
git clone --recurse-submodules https://github.com/Vellis59/port8080-blog.git
cd port8080-blog
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Configuration

Main Hugo config file:

- `hugo.toml`

Notable settings:

- `baseURL`: `https://Vellis59.github.io/port8080-blog/`
- `theme`: `PaperMod`

## Local development

Run the development server:

```bash
hugo server -D
```

Then open the URL shown in the terminal (usually <http://localhost:1313/>).

## Build

Build the production site into `public/`:

```bash
hugo --gc --minify
```

## Content

Posts live under:

- `content/posts/`
