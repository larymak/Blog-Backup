## How to Create a Screen Recorder Using Python

As a programmer, you can always utilize your skills by developing tools that can serve the same purpose as other software you need, like in this case a screen recorder. In this article, we are going to make use of Python. Python performs a variety of tasks, one of them being able to create a screen recorder.

In this tutorial guide, we will be using Python to create a screen recorder that can help you accomplish some common basic tasks just like any other software available out there. We will also be able to add some integrations to our app such as the webcam functionalities.

## What is a Screen Recorder?
A screen recorder can enable one to create and showcase demo videos, record games, and create tutorial videos that can be shared online on social media platforms such as YouTube and Twitch. In the market today many software exists that can help you achieve all this easily though. In this tutorial, you will learn how to create your own screen recorder using Python that you can further extend to your own needs.

### Python Modules Needed 

In order for us to have our application up and running, we will need to make use of some Python modules that will make it easier to develop the application They include:

* Numpy – This module will help us convert images captured into an array and pass them to openCV
* openCV – It will enable us to save the captured images in a video format.
* Pyautogui – to capture images on the screen.

## Creating a Screen Recorder 

Now, before we start writing the code for our application, we will need to make sure that we have all the necessary tools for this task. That is:

* Python should be installed in our system.
* A code editor to help us write our code – in this case, any code editor between [Pycharm](https://www.jetbrains.com/pycharm/download/), [VS Code](https://code.visualstudio.com/download), [Atom](https://atom.io/) or any of your choice will be fine.

Having ensured that we have the first step completed now we can move ahead and begin with our development. Earlier we listed some of the modules that we will need to create our app, now let’s begin by first installing them into our system.

### Step 1: Installing the modules 

To install `numpy`, we will use the pip command on either the terminal or command prompt. 

```bash
pip install numpy
```

Similarly to install `pyautogui` and `opencv` we make use of pip by executing the commands below: 

```bash
pip install pyautogui
```
&
```bash
pip install opencv-python
```

### Step 2: Import installed modules 

In order for us to use the modules that we have installed, we will need to import them. The code below allows us to do this. But first make sure that you do have a python file already created where we will be writing our code:

```python
import cv2
import numpy as np
import pyautogui
```

### Step 3: Set screen resolution

Depending on the screen size you are using you are most likely to assign different resolution parameters at this stage. It is also important to note that not everyone is likely to get or know the resolution of their screen, so using `pyautogui.size()` function will help us automatically return the correct height and width of the screen.

```python
SCREEN_SIZE = tuple(pyautogui.size())
```

But still, if you are able to get the screen resolution you can opt to use this method instead.

```python
resolution = (1920, 1080)
```

### Step 4: Create VideoWriter object

First, we begin by specifying the video codec, this is basically the encoding format of the video that will be captured. Next, we specify the format in which our output will be stored. In this case, our preferred mode is `.avi`, you can set any format you are comfortable with like `.mp4`.

It’s also in this line that you can specify the path where you want to store the recorded file, in this case, it will be stored in the same folder as our `.py` file. We also go ahead and set our fps value, in this case, we assign it to 20.

Finally, we use the `VideoCapture()` function to activate the webcam and capture from it.

```python
fourcc = cv2.VideoWriter_fourcc(*'XVID')
out = cv2.VideoWriter('output.avi', fourcc, 20.0, (SCREEN_SIZE))
webcam = cv2.VideoCapture(0)
```

This article was originally posted on my page on Sweetcode, read the rest of the [code and explanation on the page](https://sweetcode.io/how-to-create-a-screen-recorder-using-python/).


I appreciate your time reading.

Your support will be really appreciated

<a href="https://www.buymeacoffee.com/lary" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Connect With me at [Twitter](https://twitter.com/larymak1) | [GitHub](https://github.com/larymak) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi)  | 

Enjoy Coding ❤.