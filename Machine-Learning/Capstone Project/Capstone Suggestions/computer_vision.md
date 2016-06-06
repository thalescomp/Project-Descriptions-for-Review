# Project 5: Capstone Project
## Computer Vision Track
### Build a Social Image Description Platform

The **Computer Vision Track** Capstone Project is part of a number of suggested areas of research for the final project of the Machine Learning Engineer Nanodegree. Below you will find a pre-constructed project which you may use to satisfy the Capstone Project requirement. The included resources are non-exhaustive and you are free to pursue your own research beyond what is provided. Before you begin, be sure that you are familiar with the [Capstone Project rubric](https://review.udacity.com/#!/rubrics/108/view), the [Capstone Project description](https://github.com/udacity/Project-Descriptions-for-Review/blob/master/Machine-Learning/Capstone%20Project/Capstone%20Project.md), and the [project report template](https://github.com/udacity/machine-learning/blob/master/projects/capstone/project_report_template.md). These resources will be necessary to complete the Capstone Project, regardless of which domain or problem you choose to work on.

### Project Description
Build a social image description platform. Users can upload an image that they would like to have described, the image is then surfaced in other users? streams and one or more users describe it. Over time, the system learns associations between words used to describe an image and the visual features found in it, and gets better at predicting descriptions on its own. You can use one of (or a combination of) several different methods to gather features from images, including (but not limited to):
- Visual Bag of Words
- Gist
- SIFT, SURF, or other local feature descriptors
- Shape Context

For labeling, you can treat a description as a simple bag-of-words. A more advanced model could parse the description string entered by a user to understand sentence structure and semantics, and later generate descriptions that sound natural.

### Project Setup
If you are building a desktop application/program or web application, follow the Python instructions in the [Computer Vision Development Setup and Reference guide](https://docs.google.com/document/d/1ny4P-1Oybe7qIoZwIFSBnl7meOFT_QXX_ExUy2fNaEg/view). Next, clone and install the [Lumos](https://github.com/napratin/lumos) library. Play around with the library, create a copy of the sample code provided in the [README](https://github.com/napratin/lumos/blob/master/README.md#installation-and-usage), and modify it to do something fun. Make sure it runs as expected; you should be able to call it with a video or static image file as input on the command-line, or process the camera stream (default).

If you are building an Android or iOS application, you may need to use OpenCV for [Android](http://opencv.org/platforms/android.html) or [iOS](http://docs.opencv.org/2.4/doc/tutorials/introduction/ios_install/ios_install.html). Alternately, you may only need native functionality or other common libraries - it entirely depends on what algorithms (and how much of them) you want to implement.

### Tasks
Use the following instructions as a guideline to work on your project.

- Choose a target platform (desktop/web/Android/iOS), and design your overall application. Describe it as if you are building a proof-of-concept product, complete with user interface design (very simple mockups will do), intended scope, features.
- Clearly explain the computer vision/machine learning component within your application, including the inputs, desired outputs and some algorithms that you are considering.
- Build the user-facing of the system first, including a means to upload an image, show unlabeled images in a user?s stream/homepage, and store descriptions that are entered.
- Add screenshots of the system to your report explain usage scenarios and flows.
- Prepare a dataset for training and testing, so that you can repeatedly (and reliably) measure the performance of your system. You can use the system built so far to generate this dataset (perhaps with some help from your friends?!).
- Include statistics about your dataset in the report (no. of image, train-test split, etc.).
- Now implement and test your image-description matching algorithm.
  - *What computer vision and/or machine learning techniques did you use? What metric are you using to compare the predicted descriptions with the human-labeled ones?*
- Complete and improve your application by implementing any additional features.
  - *What does your final system do, and how different is it from the system you initially conceived? How well does it perform on seen vs. unseen examples?*
  
### Submitting your Project

Please refer to the [Capstone Project rubric](https://review.udacity.com/#!/rubrics/108/view) to self-evaluate your work before submitting. The following deliverables will be required as a single compressed archive:
- All of the necessary project code, datasets, supplementary files for your project
- Your project report as a PDF, which adheres to a similar structure of the [project report template](https://github.com/udacity/machine-learning/blob/master/projects/capstone/project_report_template.md)
- A README with title text **"Build a Social Image Description Platform"** along with instructions about running the code and acquiring datasets (if necessary).

### Available Courses 

- [Object Recognition and Scene Understanding](http://people.csail.mit.edu/torralba/courses/6.870/6.870.recognition.htm) (MIT)
- [Introduction to Computer Vision](https://www.udacity.com/course/introduction-to-computer-vision--ud810) (Georgia Tech and Udacity)
- [Introduction to Computer Vision](http://cs.brown.edu/courses/cs143/) (Brown University)

### Relevant Sources
- [Computer Vision: Algorithms and Applications](http://szeliski.org/Book/), by Richard Szeliski
- [Computer Vision: Models, Learning, and Inference](http://www.computervisionmodels.com/), by Simon Prince