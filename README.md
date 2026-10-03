# Cats Gallery

Live site: https://artemonre.github.io/CatsGallery/

## Adding a work

1. Put the image in `images/` (e.g. `images/sleepy.jpg`).
2. Create `_works/sleepy.md`:

   ```
   ---
   title: Sleepy
   image: /images/sleepy.jpg
   order: 7
   ---

   First line of the poem,
   second line of the poem.

   A blank line starts a new stanza.
   ```

3. Commit and push. The page appears at `/works/sleepy/` in a minute or two.

## Marking a work as sold

Add `sold: true` to the work's header (between the `---` lines). A "Sold" badge appears
next to the title, and the Buy button (if any) is hidden. Remove the line to undo.

## Buy button

Add `buy_url: https://...` to a work's header to show a Buy button linking to that address.
It is hidden automatically when the work is sold.

The **file name** is the page's URL. Don't rename it after printing a QR code;
the title, image and poem can be changed freely. `order` sets the position in the gallery.
