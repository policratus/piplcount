# 👪 piplcount

Count how many humans (frontal faces) are in the scene (from cam feed or video file).

## 🎥 Sample
![piplcount](https://github.com/policratus/piplcount/blob/master/sample/piplcount.webp)

*Just Go With It*, Dir. Dennis Dugan. Perfs. Adam Sandler, Jeniffer Aniston. Columbia Pictures, 2011

## 🛠 Installation
Assuming that you've a Unix like OS or emulation, [git](https://git-scm.com/), [Python](https://www.python.org/) 3 and [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) installed, just issue:

```
mkvirtualenv piplcount
workon piplcount
git clone git@github.com:policratus/piplcount.git
cd piplcount
pip install -r requirements/requirements.txt
```

## ⚙ Usage
There are two options of use with `piplcount`: stream from a camera or a video file. To stream using you webcam, issue:

`./piplcount stream webcam`

If you want to stream from a video file, issue:

`./piplcount stream /path/to/your/video.file`

## ⛓ Dependencies
`Piplcount` uses heavily [OpenCV](http://opencv.org/) and was tested with OpenCV 3.3.0. Despite this dependency is added to `requirements.txt`, is **encouraged** to use a manually compiled version. This article from Manuel Ignacio López Quintero can help you: http://milq.github.io/install-opencv-ubuntu-debian/. It's important also to include the support for [ffmpeg](https://www.ffmpeg.org/) when compiling OpenCV.
