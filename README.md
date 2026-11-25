# RIP Bozotendo

A documentation site for the console guides and notes originally hosted on Rentry.

## Local preview

```bash
pip install -r requirements.txt
zensical serve
```

## Build

```bash
zensical build --clean --strict
```

The source content is preserved from the supplied Rentry HTML exports. Internal links between the four pages have been updated for this site; original external references are retained.
