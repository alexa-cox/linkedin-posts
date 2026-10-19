# LinkedIn Post Assets

Image and carousel files for my scheduled LinkedIn posts. A Google Sheet holds the post schedule, and a Pabbly Connect workflow reads that sheet each day and publishes the matching post. This repository exists only to host the files those posts need at stable, public URLs.

## Structure

Files are organized by year and month of the post date:

```
assets/
  2026/
    10-october/
      2026_10_26_image.png
      2026_10_28_carousel.pdf
    11-november/
      ...
  2027/
    01-january/
      ...
```

## File naming

`YYYY_MM_DD_type.ext`, where the date is the post's scheduled date and the type is `image` or `carousel`.

| Post type | Example |
|-----------|---------|
| Text with image | `2026_10_26_image.png` |
| Carousel | `2026_10_28_carousel.pdf` |

Rules: lowercase only, underscores instead of spaces. If there are ever two posts on one day, add a suffix (`2026_10_26_image_b.png`).

## Using a file in the schedule sheet

Copy the file's raw URL into the matching sheet cell (Image URL or Document URL):

```
https://raw.githubusercontent.com/alexa-cox/linkedin-posts/main/assets/2026/10-october/2026_10_26_image.png
```

Before using a link, open it in a private browser window. If it shows only the image or PDF, it will work in the automation.

## Notes

- URLs are case-sensitive and path-based. Do not rename or move a file once a scheduled post points to it, even if the post is rescheduled to another month.
- Carousel PDFs: max 100 MB and 300 pages, per the Pabbly Connect action.
- Do not add post text, personal data, or credentials to this repository.

## License

All rights reserved. See [LICENSE](LICENSE.md). The files in this repository are for my exclusive use.

## Contact

Alexandria Cox
