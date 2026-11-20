# Images

## Adding an image

Paste an image, drop one onto the page, or type `/image` and pick one or more files. Olive saves the picture in an `assets/` folder beside the note and links it with a relative path, `![](assets/…)`, so the note and its images stay together and any Markdown viewer can show them. PNG, JPEG, GIF, WebP, SVG, AVIF and BMP are accepted.

Images referenced by an `https://` URL are shown as well. Your device fetches them from that address, as a web browser would.

## Working with an image

Click an image to show its toolbar, or right-click it for the same actions:

| Action | What it does |
| --- | --- |
| Zoom | Opens the image full screen. Double-clicking the image does the same |
| Copy image | Copies the picture itself, ready to paste into another app |
| Edit alt text | Sets the description written between `![` and `]` |
| Crop | Saves the part you keep as a new image file and points the note at it |
| Replace | Swaps in another picture, keeping the image's place in the note |
| Reset size | Returns a resized image to its natural width |
| Reload | Reads the file again after another app has changed it (right-click only) |
| Delete | Removes the image from the note |

To resize an image, drag its edge. A resized image is written as an HTML `<img>` tag with a `width`, because Markdown has no way to say how wide an image should be; dragging it back to its natural size returns it to plain `![](…)`.

**In the Mac app:** right-click an image and choose **Save image** to save the picture elsewhere on your Mac.

## Images when notes move

When you rename or move a note, the images in its own `assets/` folder move with it. Links to images kept anywhere else in the folder are rewritten instead, so they keep pointing at the same file. See [Links follow renames](links.md#links-follow-renames).

**In the Mac app:** when you delete an image from a note and no other note uses it, Olive removes the file from `assets/` the next time the note is saved, so unused pictures do not pile up. Only image files Olive could have created are removed. The VS Code extension leaves unused images in place.

---

Back to the [contents](README.md).
