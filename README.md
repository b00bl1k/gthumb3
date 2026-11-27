# gThumb3

An image viewer and browser utility.

![Image](data/appdata/ss-viewer.png)

## About this fork

gThumb3 is a fork of the original [gThumb](https://gitlab.gnome.org/GNOME/gthumb)
project. Since the upstream project has moved to GTK 4 and libadwaita, this fork
was created to keep maintaining the GTK 3 based branch of the application.

## Features

 * Image browser

   + Browse your hard disk showing you thumbnails of image files.
   + Thumbnails are saved in the same database used by Nautilus so you
     don't waste disk space.
   + Automatically update the content of a folder.
   + Copy, move, delete images and folders.
   + Bookmarks of folders and catalogs.

 * Image viewer

   + View single images (including GIF animations).  Supported image
     types are: BMP, JPEG, GIF, PNG, TIFF, TGA, ICO, XPM, JXL, AVIF.
   + Optional support for RAW and HDR (high dynamic range) images.
   + View EXIF data attached to JPEG images.
   + View in fullscreen mode.
   + View images rotated, flipped, mirrored.

 * Image organizer

   + Add comments to images.
   + Organize images in catalogs, catalogs in libraries.
   + Print images and comments.
   + Search for images on you hard disk and save the result as a catalog.
     Search criteria remain attached to the catalog so you can update it
     when you want.

 * Image editor

   + Change image hue, saturation, lightness, contrast and adjust colors.
   + Scale and rotate images.
   + Save images in the following formats: JPEG, PNG, TIFF, TGA.
   + Crop images.
   + Red-eye removal tool.

 * Advanced tools

   + Import images from a digital camera.
   + Slide Shows.
   + Set an image as Desktop background.
   + Create index image.
   + Rename images in series.
   + Convert image format.
   + Change images date and time.
   + JPEG lossless transformations.
   + Find duplicated images.

## Extensions

  gThumb3 has a plug-in system for extensions. Some standard features
  are implemented as extensions and are supplied with the standard
  distribution. Users may write (and share) additional extensions.

## Licensing

  This program is released under the terms of the GNU General Public
  License (GNU GPL), either version 2, or (at your option) any later version.

  You can find a copy of the license in the file COPYING.

## Dependencies

  Mandatory libraries:

  * glib >= 2.38.0
  * gtk >= 3.16
  * libpng
  * zlib
  * libjpeg
  * gsettings-desktop-schemas

  While not mandatory, the following libraries greatly increase gThumb3's basic usefulness:

  * exiv2 - embedded metadata support
  * gstreamer, gstreamer-plugins-base, gstreamer-video - audio/video support
  * libtiff - tiff writing support

  Other optional libraries:

  * libraw - some support for RAW photos
  * librsvg - display SVG images
  * libwebp - display and save WebP images
  * libjxl - display JPEG XL images
  * libheif - display and save AVIF images
  * lcms2, colord - color profile support
  * champlain, champlain-gtk - view the place a photo was taken on a map
  * clutter, clutter-gtk - enhanced slideshow effects
  * libsoup, json-glib, webkit2gtk, libsecret - upload images to and
    download images from some web services such as Facebook, Flickr
  * brasero - write images and comments to CDs
  * bison, flex - web albums

## Installation

    cd gthumb
    meson build
    ninja -C build
    sudo ninja -C build install

## Acknowledgements

Many thanks to Paolo Bacchilega, Michael J. Chudobiak and all the
contributors and translators of the original gThumb project for many years
of work on this excellent application. This fork would not exist without
them. See the [AUTHORS](AUTHORS) file for the list of contributors.
