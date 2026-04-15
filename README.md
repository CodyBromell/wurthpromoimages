# Würth Promo Images

Product image hosting for Würth UK promotional materials.

## Why this exists

Our CMS deletes uploaded images periodically. This repo is the permanent source of truth — images here are referenced by direct URL, so nothing breaks when the CMS wipes its own files.

## How to use an image in the CMS

Every image in this repo has a permanent public URL. Pattern:

```
https://raw.githubusercontent.com/<your-username>/wurthpromoimages/main/<filename>
```

Example — the wireless mouse image:

```
https://raw.githubusercontent.com/<your-username>/wurthpromoimages/main/Wireless%20mouse%20-%20WTE.png
```

(Spaces in filenames become `%20` in URLs.)

Paste that URL into the CMS image field instead of uploading the file, and it will load directly from GitHub.

## Adding new images

1. Drop the image file into this folder
2. Commit and push:
   ```bash
   git add .
   git commit -m "Add <image name>"
   git push
   ```
3. The raw URL is available immediately.

## Naming convention

`<Product name> - WTE.<ext>` — keep it human-readable, the filename ends up in the URL.
