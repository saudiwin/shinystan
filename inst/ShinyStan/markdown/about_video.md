---
title: "About Shinystan Video"
output: html_document
---

This page will create videos of MCMC parameter exploration relative to another variable or to the log-posterior on the y axis. It will either show multiple parameters of a single chain or multiple chains of a single parameter along the x axis. 


```
## [1] "Your system shows that the ffmpeg library is  present and the gg_animate package is  present"
```

If either of these are listed as "not present", please read the installation instructions below.

As this function relies on additional software (non-R) for support, please read through the following installation guidelines:

1. Install the ffmpeg package. It is included with the ImageMagick software for Windows or Mac OS at  <http://www.imagemagick.org/script/binary-releases.php>. After installing the software, you must restart R or Rstudio.

2. Install the gg_animate package in R or Rstudio from github using the following code:

```
devtools::install_github("dgrtwo/gganimate")
```

You are now ready to create movie files. Please be aware that the greater number of iterations you include in a movie, and the greater number of frames used to smooth the movie (see the options panel), the more time will be required to produce the result. For example, if you select 20 iterations and a frame smoothing factor of 10, this will require the production of 20 * 10 = 200 charts before the video can compile. Reducing the frame smoothing factor will produce a jumpy video.

The videos are produced in the .WEBM format. This format may not display in Safari or Internet Explorer without additional plugins; however, it will play correctly on Chrome and Firefox. The movie can also be uploaded directly to Youtube to share and/or watch. To share on Youtube, first download the movie to your computer using the download button at the bottom of the screen.
