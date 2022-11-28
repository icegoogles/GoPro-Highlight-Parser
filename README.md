# GoPro-Highlight-Parser
This project is to extract the highlights of GoPro-videos.

It only works for the highlights that were manually selected on the GoPro or a smartphone that is connected to the GoPro via the GoPro App.
Highlights selected in GoPro-Quick are not stored inside the MP4-file.


# How to use
## Easy method for windows:
1. For Windows just download the GP_Highlight_Extractor.exe and Drag and drop the videofile(s) onto the exe

## Method with Python:
1. Install Python 3.X on your system (for example via the micosoft store) (python version 3.8 or higher recommended)
2. Download the repository (or just the "GP Highlight Extractor" python-file)

## Result:
2. Drag and drop the videofile(s) onto the "GP Highlight Extractor.py"/"GP_Highlight_Extractor.exe" file

![drag and drop](/images/drag_and_drop_onto_file.jpg)

3. A txt-file will be created in the directory of the Video-file(s)

![created txt-file](/images/created_txt.jpg)

4. Inside the txt-file all Highlights are stored in the following format

![Formatting of the txt](/images/inside_txt.jpg)

# Tip
Premiere Pro uses the Media-Timecode of the GoPro footage and therefore does not start at 00:00. To fix this Issue, go to: 

EDIT > PREFERENCES > MEDIA

and set 'Timecode' to "Start at 00:00:00:00"!

# Info
Tested and developed on Windows 10 on Python 3.8.
The footage for testing was from the GoPro HERO6, but it should work for other models as well.

The code for extracting the mp4 boxes/atoms is from 'Human Analog' (https://www.kaggle.com/humananalog):
https://www.kaggle.com/humananalog/examine-mp4-files-with-python-only
