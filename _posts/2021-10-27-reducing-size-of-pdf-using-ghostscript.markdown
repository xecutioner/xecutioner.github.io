---
layout: post
author: kapil
---
# Reducing size of pdf using ghostscript.

There might be couple of times when you are working sharing documents across and PDF's as we know can be bloted up quite unreasonable. 
Here is a shortcut to quickly reduce the size, 

## Installing the ghostscript. 

  Ghostscript is ready available as a [brew package]9https://formulae.brew.sh/formula/ghostscript)
you can easily install it by doing . 
```
brew install ghostscript
```
If you have a big pdf file called input.pdf then do the foo as follows.
 
```
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook \
-dNOPAUSE -dQUIET -dBATCH -sOutputFile=output.pdf input.pdf
```
