
[![LinkedIn][linkedin-shield]][linkedin-url]

# Face and Eye Detection

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project
      </a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
In this project we detect the face and eye of a person. 
We all know video is a collection of frames. So, we take a frame from video and then process it and implement our code on it. and show it on screen. import XML file of out training data. First step is to convert a frame in gray scale to pre-processing because in grey scale it reduce dimensions and reduce complexity. Then first we work on face, so, we train our model and make a rectangle on our face . Then we know eyes lies in our face rectangle, so, we apply another rectangle in our face rectangle on our eyes. then show this frame on the screen. We put this in while loop because we continue take the frames and when the frames are not coming it will automatically get's out of the loop.

<p align="center">
<img src="https://i.redd.it/vl8nmx8drhh31.jpg"
 alt="Logo" width="400" height="400">
</p>


### Built With

We use opencv to accomplish this task.
you must know about these terms also:
* Grayscaling : it is the process of converting an image from other color spaces e.g RGB, CMYK, HSV, etc. to shades of gray. It varies between complete black and complete white. Importance of Grayscaling is 
-> Dimension reduction: For e.g. In RGB images there are three color channels and has three dimensions while grayscaled images are single dimensional.
-> Reduces model complexity: Consider training neural article on RGB images of 10x10x3 pixel.The input layer will have 300 input nodes. On the other hand, the same neural network will need only 100 input node for grayscaled images.
-> For other algorithms to work: There are many algorithms that are customized to work only on grayscaled images e.g. Canny edge detection function pre-implemented in OpenCV library works on Grayscaled images only.

<p align="center">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRcxlaavHWVYhlLbtAgz9shUIgYbG1vkvKurA&usqp=CAUhttps://i.redd.it/vl8nmx8drhh31.jpg"
 alt="Logo" width="400" height="200">
</p>

* Cascade Classifier Training: Object Detection using Haar feature-based cascade classifiers is an effective object detection method proposed by Paul Viola and Michael Jones in their paper, "Rapid Object Detection using a Boosted Cascade of Simple Features" in 2001. It is a machine learning based approach where a cascade function is trained from a lot of positive and negative images. It is then used to detect objects in other images.
Here we will work with face detection. Initially, the algorithm needs a lot of positive images (images of faces) and negative images (images without faces) to train the classifier. Then we need to extract features from it.

* Image Thresholding: In this method, the pixel values of a grayscale image are assigned one of the two values representing black and white colors based on a threshold value. So, if the value of a pixel is greater than a threshold value, it is assigned one value, else it is assigned the other value.


<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
* Any python Compiler

### Installation

1. Install packages
   ```sh
   pip install opencv-python
   ```



<!-- USAGE EXAMPLES -->
## Usage
Although all facial recognition systems use face detection, not all face detection systems are used for facial recognition. Face detection can also be applied for facial motion capture, or the process of electronically converting a human's facial movements into a digital database using cameras or laser scanners. This database can be used to produce realistic computer animation for movies, games or avatars.

Face detection can also be used to auto-focus cameras or to count how many people have entered an area. The technology also has marketing applications -- for example, displaying specific advertisements when a particular face is recognized.

Another application for face detection is as part of a software implementation of emotional inference, which can, for example, be used to help people with autism understand the feelings of people around them. The program "reads" the emotions on a human face using advanced image processing.

An additional use is drawing language inferences from visual cues, or "lip reading." This can help computers determine who is speaking, which may be helpful in security applications. Furthermore, face detection can be used to help determine which parts of an image to blur to assure privacy.



<!-- ROADMAP -->
## Roadmap

1. In this AI world, opencv library is must to learn about AI. 
2. The main goal of this repository is to detect the human face and eye. We only require opencv library for this.
3. First a fall, we import opencv library.
4. Then we import haarcascade data of eye and face using cascade classifier and assign it to a variable.
5. Start the camera and use live camera using videocapture(0), if you want to perforn on any video then simply change 0 to 1 in videocapture.
6. Now, we use while loop to access video framewise.
7. Convert each frame to gray scale.
8. Now, we train our program to detect face using the haarcascade dataset.
9. Now understand, we now have the small area to work on to detect eye and the area is of rectangle on face. Apply the same process to detect eye.
10. Show the final result using the final frame.
11. Frame is changing continuously so when we show output frame it is like a video.
<p align="center">
<img src="https://miro.medium.com/max/1295/1*xiQFZb7bkjpdk4WFsOUpEg.jpeg"
 alt="Logo" width="750" height="600">
</p>


Here you go! This was a simple way to detect faces, eyes, and happiness.
<p align="center">
<img src="https://learnopencv.com/wp-content/uploads/2017/02/real-time-face-tracking.gif"
 alt="Logo" width="350" height="300">
</p>

## Contact

Aniket Yadav - [Medium](https://aniketyadavv.medium.com/) - [Gmail](https://yadavaniket0820gmail.com/)
<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/aniket-yadav-2008/
