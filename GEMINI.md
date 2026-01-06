# Project Context: Megat's Website (Jekyll)

## Project Overview
This project is a personal static website for **Megat Iskandar Hashim Bin Ismail**, hosted on GitHub Pages (`megatih.github.io`). It is built using [Jekyll](https://jekyllrb.com/) and utilizes the [Beautiful Jekyll](https://beautifuljekyll.com/) theme by Dean Attali.

The site features a blog, an "About Me" section, and links to various social media profiles.

## Building and Running

### Prerequisites
*   Ruby
*   Bundler

### Commands
*   **Install Dependencies:**
    ```bash
    bundle install
    ```
*   **Run Local Server:**
    ```bash
    bundle exec jekyll serve
    ```
    The site will be available at `http://localhost:4000`.

## Development Conventions

### Content Management
*   **Blog Posts:**
    *   Located in `_posts/`.
    *   Filename format: `YYYY-MM-DD-title.md` (e.g., `2025-10-29-setting-up-ubuntu.md`).
    *   **Front Matter:** Must include `layout: post`, `title`, `subtitle`, and `tags`.
*   **Pages:**
    *   Located in the root directory (e.g., `aboutme.md`).
    *   **Front Matter:** Must include `layout: page` and `title`.

### Configuration
*   **Main Config:** `_config.yml` controls site-wide settings like title, author, navigation links (`navbar-links`), social links, and enabled plugins.
*   **Theme:** The project uses the `beautiful-jekyll-theme`. Custom styles can be added to `assets/css/` if configured in `_config.yml`, though the theme primarily uses `assets/css/beautifuljekyll.css`.

### Assets
*   **Images:** Store in `assets/img/`.
*   **CSS/JS:** Located in `assets/css/` and `assets/js/`.

### Key Directories
*   `_layouts/`: HTML templates for different page types (`post`, `page`, `home`).
*   `_includes/`: Reusable HTML snippets (e.g., `header.html`, `footer.html`, social links).
*   `_data/`: Data files (currently `ui-text.yml`).
