# Arrange pictures in your gallery
ArrangeGallery is a Python3 tool built to organize your image gallery using face recognition. It identifies individuals in the images and arranges them into a neat file structure where photos of the same person are grouped together. Additional functionalities are the generation of slideshows, resizing of all images, detection and removal of duplicate images, and creating face collages for specified people.

## The Idea
We take thousands of pictures on our devices, and we often want to find photos of certain people, but scrolling through all the pictures is inefficient and annoying. This project aims to automate the task of organizing pictures in your gallery with face recognition to sort photos by the people they contain.

## How it works
Faces are recognized in the photos found in the images directory with the face_recognition Python library and comparisons are made between identified faces to group images of the same person together. All identified images are then moved to a new directory where they are sorted by the individual they contain.
In addition to this core functionality, you can also generate face collages for a specific person, create slideshows with various filters based on Computer Vision algorithms, resize or crop all images in an album, and detect and remove duplicate images.

## How it was built
The python3.8 program mainly relies on the face_recognition library for facial detection and comparison. Other libraries such as pandas, numpy, and opencv-python are used for data management and image processing tasks. Multiprocessing was utilized to optimize performance when handling large albums, and checkpointing was used to maintain long running tasks, creating a form of caching that improves efficiency and minimizes repetitive calculations.

## Bugs and challenges
A challenge was optimizing the program to handle large image albums efficiently. Another thing to consider was that face recognition in images varies in accuracy depending on the quality and resolution of the pictures.

## Things learned
During this project I learned to work with Python libraries like face_recognition, pandas, numpy, and opencv-python. It served as practical application of computer vision concepts, particularly face detection and comparison algorithms. The use of multiprocessing and checkpointing for optimization and efficiency in data processing tasks was interesting for handling large datasets.

## Roadmap
The next step would be to add functionalities for additional filters for slideshow creation and more advanced face recognition techniques for better accuracy. It also needs some improvements particularly for handling very large image albums.
