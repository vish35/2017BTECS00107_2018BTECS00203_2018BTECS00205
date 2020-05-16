The project is about
-- Given sample images master sample as well as images
acquired while undergoing chemical processing to remove material. Finding the surface area for which 
the material has been removed.

Solution -
Color image segmentation is used. 

How does it work?
1. Input original image
2. Binarising original image 
3. Detecting contours in original image
4. Rectangular regions are formed around hexagonal materials
5. Removing the background from original image by performing Binary AND with binarised image
6. Removing Non-reacted material (white-gray coloured material) by colour based thresholding
7. Calculating percentage area of material reacted.

The project coded in python and image processing is done using OpenCV library.


The challenges faced were -
1) Too large dimension of images.
      For fast processing switched from single threaded --> multithreaded --> multiprocessing.
      
2) Uneven illumination of image and orientation of plate not fixed.

The file dip.py is the main program.

