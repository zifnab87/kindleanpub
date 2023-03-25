### What is this?
Forked Version of (https://github.com/hmemcpy/kindleanpub) for ready made script to run in Windows 7 64bit

A small shell script that fixes garbled/broken image rendering on (older) Kindle devices of PDFs due to [some issue](https://groups.google.com/d/msg/leanpub/YxVlTlwNfpM/hV6hnKjXAQAJ) with Kindle's method of processing PNG files.

Using [Ghostscript](https://www.ghostscript.com/), this script will convert all images inside the PDF to JPEG using highest quality conversion.  
This will result in smaller output PDF size, and will make the images render properly on older Kindles (e.g. Kindle DX)

### Usage (tested with WINDOWS 7 64bit only)

Open wsl in Windows and navigate to the folder then execute

    $ ./pdfix.sh input.pdf

Will produce a file `input-fixed.pdf` in the same directory.

#### Example

Before (11.1MB) |  After (7.23MB)
:--------------:|:---------------:
![before](https://user-images.githubusercontent.com/601206/38953873-bd45cbf6-4358-11e8-8fcb-1fee5d25784a.png) | ![after](https://user-images.githubusercontent.com/601206/38953868-bb9775a2-4358-11e8-9047-51f6b43b3f50.png)
