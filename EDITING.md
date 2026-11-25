# Editing the Site

This guide explains how to make changes to RIP Bozotendo, add images and links, preview your work, and publish updates. You do not need to understand the website's CSS or Zensical configuration for ordinary content edits.

## Where the content lives

The site is built from files in the repository. The pages readers see are Markdown files (some of the migrated content uses HTML inside those files to preserve its original layout).

| Page | File to edit |
| --- | --- |
| Home page and gallery | `docs/index.md` |
| 3DS guide | `docs/3ds/index.md` |
| Steam Deck guide | `docs/steam-deck/index.md` |
| Wii guide | `docs/wii/index.md` |
| This editing guide | `docs/editing-guide.md` |

The navigation menu is configured in `mkdocs.yml`, which Zensical reads. Images and other page assets live under `docs/assets/`. The site's custom styling is in `docs/stylesheets/extra.css`.

**For normal updates, edit a page file under `docs/`.** You usually do not need to touch `mkdocs.yml`, the workflow in `.github/workflows/`, or the CSS.

## Option 1: Edit directly on GitHub

This is the easiest method for a quick typo fix or a small text/link change.

1. Open the [RIP-Bozotendo repository](https://github.com/MegalonVII/RIP-Bozotendo) and make sure you are signed in to an account with write access.
2. Open the file you want to change, using the table above to find it. For example, open `docs/3ds/index.md` for the 3DS page.
3. Select the pencil **Edit this file** control.
4. Make your change in the editor. The migrated pages contain some HTML, so preserve surrounding tags when editing those sections. If a paragraph is wrapped in `<p>...</p>`, keep the opening and closing tags balanced.
5. Use **Preview** if GitHub offers it for the file. Check your edits carefully; GitHub's preview is not a complete substitute for the actual site preview.
6. Select **Commit changes**, enter a short description such as `Fix 3DS guide typo`, and commit directly to `main` if this is a straightforward change.

The site has an **Edit this page** link configured in its theme. When you are viewing a page while signed in with write access, that link should take you to the corresponding source file on GitHub.

## Option 2: Edit on your computer (recommended for larger changes)

Editing locally is more comfortable for substantial rewrites, moving sections, adding several images, or checking the whole site before publishing.

### Set up the project once

1. Install [Python 3](https://www.python.org/downloads/) if it is not already installed.
2. Install [Git](https://git-scm.com/downloads/) or [GitHub Desktop](https://desktop.github.com/).
3. Clone the repository from GitHub, or open the local repository folder if you already cloned it.
4. Open a terminal in the project folder — the folder containing `mkdocs.yml`.
5. Create and activate a virtual environment:

   **macOS / Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

   **Windows PowerShell**
   ```powershell
   py -m venv .venv
   .venv\Scripts\Activate.ps1
   ```

6. Install the site's dependencies:
   ```bash
   python -m pip install -r requirements.txt
   ```

You only need to do the setup steps once per computer. Later, open the project folder and activate the existing `.venv` before running Zensical.

### Preview while editing

From the project folder, with the virtual environment active, run:

```bash
python -m zensical serve
```

Open the local address printed in the terminal (normally `http://127.0.0.1:8000/`). The preview refreshes when you save a file. Stop the preview with `Ctrl+C` in the terminal.

Before publishing, run a strict build:

```bash
python -m zensical build --clean --strict
```

If the command finishes without errors, the site built successfully. If it reports a warning or error, fix the reported issue and run it again. The generated `site/` folder is a build output; do not edit it or commit it.

## Adding or changing content

### Text and headings

The content files use Markdown, with some preserved HTML from the Rentry export. For new sections, Markdown is usually the simplest choice:

```markdown
## A new section

Write the explanation here. You can use **bold**, *italic*, and `inline code`.

### A smaller subsection

More details go here.
```

Use `##` for a main section within a page and `###` for a subsection. Keep the heading levels in a sensible order. Avoid changing existing heading text or IDs unless you also check links that point to those headings.

**Important:** Much of the migrated content is HTML. Add new Markdown sections between complete HTML elements; do not put Markdown headings or paragraphs inside an existing `<p>`, `<div>`, or other HTML element. When editing existing HTML, keep tags properly paired.

### Links to other pages

Use these paths when linking between the site pages:

| From | Link target |
| --- | --- |
| Home page | `3ds/`, `steam-deck/`, `wii/` |
| Any console page | `../`, `../3ds/`, `../steam-deck/`, `../wii/` |

For example, from the Wii page, link to the 3DS page like this:

```markdown
[See the 3DS guide](../3ds/)
```

To link to a section on another page, add its heading fragment, such as `../3ds/#section-heading`. The fragment is based on the heading's generated ID. If you change a heading, check and update links that use its old fragment.

External links can use their full URL:

```markdown
[Official documentation](https://example.com/)
```

### Adding images

1. Put the image file in `docs/assets/`. For tidiness, you can create a subfolder such as `docs/assets/images/` and keep new images there.
2. Give the file a clear name, using lowercase letters and hyphens where practical (for example, `3ds-home-menu.png`).
3. Reference it from the page. The path is relative to the page's folder:

   From the home page (`docs/index.md`):
   ```markdown
   ![A descriptive caption](assets/images/example.png)
   ```

   From a console page such as `docs/3ds/index.md`:
   ```markdown
   ![A descriptive caption](../assets/images/example.png)
   ```

Write useful alt text inside the square brackets so readers using assistive technology, or readers whose image does not load, know what the image shows. Keep image filenames and paths exactly the same, including capitalization.

### Code blocks

Use triple backticks around multi-line commands or code. Add a language name after the opening backticks when appropriate so syntax highlighting works:

````markdown
```bash
python -m zensical serve
```
````

For a single command or filename within a sentence, use single backticks: `mkdocs.yml`.

### Notes and warnings

Zensical supports callout blocks (admonitions). Put four spaces before the text inside the block:

```markdown
!!! note "Note"
    This is useful additional information.

!!! warning "Warning"
    Double-check this step before continuing.

!!! tip "Tip"
    A helpful shortcut or suggestion.
```

The existing migrated pages may also contain HTML callout blocks. It is fine to leave those as they are; use the Markdown form for new content.

## Publishing your changes

### If you edited on GitHub

Committing a change to `main` automatically starts the deployment workflow. No separate upload is required.

### If you edited locally

1. Review the changed files.
2. Run `python -m zensical build --clean --strict` and fix any errors.
3. Commit your changes with a clear message.
4. Push the commit to the repository's `main` branch.

For example, with Git:

```bash
git status
git add docs/
git commit -m "Update Steam Deck guide"
git push
```

If you changed configuration or styling too, stage those files as well (for example, `git add mkdocs.yml docs/`). With GitHub Desktop, review the changed-file list, enter a summary, commit, and select **Push origin**.

### Check that the site deployed

1. Open the repository's **Actions** tab.
2. Select the newest **Deploy documentation** run.
3. Wait for both the build and deploy jobs to finish successfully.
4. Open the published site and check the changed page, its images, and any links you added.

If the workflow fails, open the failed job and read the first reported error. Common causes include a broken image path, malformed Markdown/HTML, or an invalid link/configuration change. Fix the source file, commit, and push again.

The deployment workflow runs when changes are pushed to `main`, or when manually started from the Actions tab using **Run workflow**. GitHub Pages must be configured to use **GitHub Actions** as its source (Repository **Settings → Pages → Build and deployment → Source**).

## Things to avoid

- Do not edit files inside `site/`; that folder is generated during the build.
- Do not delete or rename an image without updating every page that references it.
- Do not rename existing page folders unless you also update `mkdocs.yml` and links to those pages.
- Do not remove `.github/workflows/deploy.yml`; it is what publishes updates automatically.
- Do not commit passwords, access tokens, private keys, or other secrets.
- When changing a heading, check links to its heading fragment (`#...`).

## A safe editing routine

For most changes, this is all you need to remember: edit the right file under `docs/`, preview it if the change is substantial, commit and push to `main`, then check the latest run in **Actions**. The live site updates after the deployment succeeds.
