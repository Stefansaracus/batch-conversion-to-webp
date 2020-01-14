# WebP Converter
## Handy Python script that converts images to the WebP format.

It is always good to serve optimized & quality images on your website.
The WebP format is always recommended for everything web.

The aim of this script is to convert all your images in batch & organize them to a new directory.

---

## Why WebP?
WebP is the format developed with web in mind. It provides many performance benefits while serving the assets for your website. 

Reference: [web.dev](https://web.dev/serve-images-webp/)

---

## How the script works?
![Demo](demo/demo.gif "gif")

The script uses the [WebP library](https://developers.google.com/speed/webp/docs/precompiled) provided by Google for the conversion process.

You are required to copy the provided script to the directory where all your
images are being stored. Though not neccesary but suggested, that the directory should contain only the image files.

On running, the script will scan the current directory for images with extensions of '.jpg', '.jpeg' & '.png'. Next, using the following bash command, the script will convert the every selected image to '.webp' format.

Command: `cwebp -q 80 image.jpg -o image.webp`
where, 80 = typical output quality.

_Quality can be modified by editing the `quality` in the script._

Once converted, the images will be organized to a new directory named 'webp'.

_The name of the directory can be modified by editing the `dir_name` in the script._

**NOTE: Converted images will have the same name as they had before conversion.**

---

## Why this script?
This script can do the following:

* Detect for the missing images after conversion & restore them accordingly.
* If the missing images are present in the original directory, it organizes them accordingly.

Few more features are in progress. 

I hope you find this script useful, cheers!

---

`Code Plus Coffee`