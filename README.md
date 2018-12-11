Now Bbox saves to YOLO format by default

BBox-Label-Tool
===============

A simple tool for labeling object bounding boxes in images, implemented with Python Tkinter for Python 3.X.

-- For convert label to VOC notation(format), diselect the checkbox 'Save to YOLO format'
**Do not use two formats in one image!**

-- For multi-class task, modify 'class.txt' with your own class-candidates and before labeling bbox, choose the 'Current Class' in the Combobox and make sure you click 'ComfirmClass' button.


**Screenshot:**
![Label Tool](./screenshot.png)

Environment
----------
- python 3.X
- python PIL (Pillow)

Run
-------
$ python main.py

Usage
-----

1. Chose a folder click `Open folder`. The images in the folder, along with a few example results will be loaded.
2. To create a new bounding box, left-click to select the first vertex. Moving the mouse to draw a rectangle, and left-click again to select the second vertex.
  - To cancel the bounding box while drawing, just press `<Esc>`.
  - To delete a existing bounding box, select it from the listbox, and click `Delete`.
  - To delete all existing bounding boxes in the image, simply click `ClearAll`.
3. After finishing one image, click `Next` to advance. Likewise, click `Prev` to reverse. Or, input an image id and click `Go` to navigate to the speficied image.
  - Be sure to click `Next` after finishing a image, or the result won't be saved. 
4. If you want to convert label to yolo notation(format), enable the checkbox 'Save to YOLO format'
**Do not use two formats in one image!**
5. For multi-class task, modify 'class.txt' with your own class-candidates and before labeling bbox, choose the 'Current Class' in the Combobox and make sure you click 'ComfirmClass' button.
