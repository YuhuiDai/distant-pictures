# distant-pictures
A simple server that serves webcam pictures to a website. 

In this lab, users would be able to press a button on the arduino board to take photos
and also be able to choose filters to apply to their images.

I used the "filterous" npm library and the main challenge is the asynchronous issues:
for instance, when an image is captured by webcam, the image would be read by the 
filterous library from npm library. In order to wait until the image to be saved,
I delayed the function call by using setTimeout. With this brute force solution,
users are able to capture pictures with desired filters.
