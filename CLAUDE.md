# Development Instructions

## Setup Environment
To set up the development environment in Termux:
```bash
pkg install ruby
gem install jekyll bundler
```
Note: Ensure `make` and `clang` are installed if building native extensions for gems:
```bash
pkg install make clang libffi zlib
```

## Build and Serve
- Build the site:
  ```bash
  jekyll build
  ```
- Serve locally:
  ```bash
  jekyll serve
  ```
  Note: If links don't resolve locally due to `baseurl`, use:
  ```bash
  jekyll serve --baseurl ""
  ```

## Project Configuration
- **Engine:** Jekyll 4.x
- **Markdown:** kramdown (GFM)
- **Highlighter:** rouge
- **Output:** `_site/` (ignored in git)
