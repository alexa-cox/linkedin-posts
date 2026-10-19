# LinkedIn Post Assets

Image and carousel files for my scheduled LinkedIn posts. A Google Sheet holds the post schedule, and a Pabbly Connect workflow reads that sheet each day and publishes the matching post. This repository exists only to host the files those posts need at stable, public URLs.

## Contents

```
assets/
  images/      One image per text post (PNG or JPG)
  carousels/   One PDF per carousel post
```

## File naming

Each file is named after its row in the schedule sheet so it is easy to match:

| Post type | Folder | Example |
|-----------|--------|---------|
| Text with image | `assets/images/` | `post-001.png` |
| Carousel | `assets/carousels/` | `post-014.pdf` |

## Using a file in the schedule sheet

Copy the file's raw URL into the matching sheet cell (Image URL or Document URL):

```
https://raw.githubusercontent.com/<username>/<repo-name>/main/assets/images/post-001.png
```

Before using a link, open it in a private browser window. If it shows only the image or PDF, it will work in the automation.

## Notes

- Files must stay in this repository, at the same path, for as long as a scheduled post still needs them. Renaming or deleting a file breaks the post that points to it.
- Carousel PDFs: max 100 MB and 300 pages, per the Pabbly Connect action.
- Do not add post text, personal data, or credentials to this repository.

## License

All rights reserved. See [LICENSE](LICENSE). The files in this repository are for my exclusive use.

## Contact

Alexandria Cox
