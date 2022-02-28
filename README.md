<p align="center"><img src="PycolorLogo.PNG"\></p>

# Pycolor_Video : Video Color Detection

- Pycolor_Video is a program that allows you to identify the main color present in a given area on a video.

# Requirements

- You will need to install the following libraries :

* numpy
* opencv

# How it works

- A video is given to the programm, which read it.
- The coordinates of the area to be inspected are to be entered in the code.
- The video is played frame by frame.
- The program copies the image into a new variable and converts each BGR (Blue,Green,Red) pixel into HSV (Hue, Saturation, Value).
    - I chose HSV rather than RGB because depending on the video given, the shades are more difficult to identify depending on the day, night or weather. You can see how it's work thanks to the HSV graph i put below.
    - I created them for a daytime video.
    - The HSV shades for each colour have been chosen by myself, and can be changed.
- A list of colours that can be identified is initialized as well as a list containing as many 0s as colours.
- Each pixel of the area to be inspected is analysed and increases the index of the colour identified in the list.
- At the end of the area analysis, the program selects the index with the highest score and then selects the colour assigned to that index.
- I have added two lines in the program that border the selected area and display the selected colour on the image displayed on the screen.
- The video containing the analysis is converted and recorded while the program is running and can be viewed at the end of the program.

# HSV Graph

<p align="center"><img src="640px-HSV_color_solid_cylinder_saturation_gray.png"\></p>

# Gif Output

<p align="center"><img src="data/gif/VideoOutput.gif"\></p>


 

