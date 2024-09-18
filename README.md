# Moneypenny tech test

## Issues to Fix:

### 1. When you hover the "Buy now" button the background colour doesn't change.

This is due to line 31 `position: absoloute;` causing the pseudo element overlapping the button, I have fixed it by adding `pointer-events: none;` to the absoloutely positiond element.

It could also be fixed by removing the absoloute positioning, removing the :after pseudo element, or setting the z index to lower than the button's z index.

### 2. The styling on the image is missing its rounded borders.

Line 12 of the html doc was missing an 's' in 'class' so the styles weren't applying.

This could also be fixed by adding `overflow: hidden` to the wrapper element.

### 3. The page is slow to load due to unoptimized images.

I have resized the image file to 327 x 420 px. The original image is in the raw-images folder.
