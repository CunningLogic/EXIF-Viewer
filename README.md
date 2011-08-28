# PicciMario EXIF analyzer v. 0.1

mario.piccinelli@gmail.com

This command line tool pronts a list of the EXIF data found in the passed image. The most important tags are decoded. All info about the EXIF standard is taken from http://www.exif.org/Exif2-2.PDF.

Usage:

  ./exifviewer.py filename
  
The package also contains anothere tool (exifreporter.py) which analyzes a JPG picture and prints a PDF report with informations about the file (as told by the filesystem) and about the image itself via its EXIF tags. Special care has been thrown in intepreting the GPS data, if present the report will contain a map of the location and an approximate reverse geocoding of the coordinates into their location name.

Usage:

  ./exifreporter.py -f filename -o reportname


# Requires:

* Tested on Python 2.6 on Linux and Mac Os X.

* Python Imaging Library (PIL). For Mac Os download from [here](http://www.pythonware.com/products/pil/). For Linux you should do something like:
  
  sudo apt-get install python-imaging python-imaging-tk

* ReportLab Toolkit (open source version). You can download it [here](http://www.reportlab.com/software/opensource/rl-toolkit/download/).