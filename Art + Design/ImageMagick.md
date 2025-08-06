---
created: 2025-07-22
modified: 2025-07-22
description: 
aliases: 
tags:
  - Art-Design
---

# Commands

|                                                                     Command                                                                      |                       Note                       |     Type      |
| :----------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------: | :-----------: |
| `magick mogrify -path output -resize 25% -quality 100 input/*.png`<br><br>`magick mogrify -path output -resize 256x256 -quality 100 input/*.png` | use in base folder with input and output folders | batch resize  |
|                                          `magick convert image.png -resize 25% -quality 100 image2.png`                                          |                                                  | single resize |

```
magick mogrify -path output -resize 25% -quality 100 input/*.png
magick mogrify -path output -resize 500x500 -quality 100 input/*.png
magick mogrify -path output -resize 256x256 -quality 100 input/*.png
magick mogrify -path output -resize 26.04% -quality 100 input/*.gif


```

# Resources

- https://imagemagick.org/
