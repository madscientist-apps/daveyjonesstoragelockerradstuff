# Ghostie public images

Public image host for Ghostie. It holds only images that other services, such
as WriteStack, have to fetch from a public web address. Ghostie itself runs on
Aaron's Mac, so it has no public URL of its own.

- `note-images/<note id>/...` holds Note attachments. Ghostie uploads new ones
  itself through the GitHub API, using `GHOSTIE_IMAGES_GITHUB_TOKEN` in
  `.env.local`.
- Everything here is public. Put nothing private in this repo.
- Files are never overwritten. A replaced image gets a new file name, so a URL
  that is already in use keeps pointing at the same picture.

The canonical copy of every image also lives in the Ghostie repo under `data/`.
