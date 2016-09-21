# install-opencv-mac

# install homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# follow these commands
1) brew tap homebrew/science
2) brew install opencv
3) cd /usr/local/Cellar/opencv/*youropencvversion*

# setting up python

1) cd /Library/Python/2.7/site-packages/
2) ln -s /usr/local/Cellar/opencv/*youropencvversion*/lib/python2.7/site-packages/cv.py cv.py
3) ln -s /usr/local/Cellar/opencv/*youropencvversion*/lib/python2.7/site-packages/cv2.so cv2.so

# setting up pythonpath

1) cd
2) sudo nano ~/.bash_profile
then add the following line
3) export PYTHONPATH=`brew --prefix`/lib/python2.7/site-packages:$PYTHONPATH

# Success!

python -> import cv
