# gpages-gallery

A Simple Photo Gallery for GitHub Pages, so there is no online image
sizing. There are exising jekyll plugins that generate image
galleries, but these cannot run natively on github pages, requiring a
local jekyll installation. We sidestep this problem by using jekyll to
generate the site from a CSV list of photos, captions, etc.


# Usage

Fill `_data/images.csv` with the list of images. You can add more
columns, and later use these in the template, but at the minimum, you
must have:
 - `image_src`, which is the file name of the image. The image should
   have a low res copy in `assets/images/gallery-thumbnail`, and a
   high-res copy in `assets/images/gallery-full`, both with the same
   name, which is contained in the column `image_src`
 - `title` 
 - `caption`


## Templating
    
