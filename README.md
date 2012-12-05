This script was written to convert output from Hugin, the free panorama tool that runs on any platform (http://hugin.sourceforge.net).  

Early in Hugin's development, it did not crop the output.  So, unless you were creating a full 360x180 panorama, you would get all the pixels visible in the preview viewing area.  This often lead to a large, blank, alpha-channel area around your stitched composite image.  Being an ImageMagick aficionado, I sought to a) keep all the pixels, b) trim down to the smallest circumscribed rectangle, and c) set the color of the alpha-channel (background layer) - often to white.

Thus, this script.  I have decided to put it up on github in case anyone else might find it useful or wish to contribute.  I am adding various options, such as specifying the background color [-b color] (default: white), JPEG quality level [-j 1-100] (default: 90), possibly a toggle for smallest circumscribed or largest inscribed cropping, and a -q for quiet mode.

