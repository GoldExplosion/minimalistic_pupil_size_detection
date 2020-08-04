#Minimalistic pupil size detection
The is an simple image processing program with the objective of detecting the size of the pupil.

Citation:​ L. Vázquez Romaguera et al (2015) Pupil Segmentation Approach on Low Resolution
Images DOI: 10.1007/978-3-319-13117-7_110 

The algorithm is:

1) input
2) selecting the channel in rgb
3) histogram equalization
4) thresholding
5) Morphological closing operation
6) Morphological opening operation
7) Find the largest object of connect components8) Draw a rectangle around the largest object
9) determine the pupil size by calculating the average of the sides of the rectangle

Disadvantages:
1) it will not give accurate results unless you provide an image of an well lit eye
2) since it finds the largest component after thresholding, there must not be a dark and big component other than the pupil.
