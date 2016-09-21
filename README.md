# install-opencv-mac

# install homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# follow these commands
1) brew tap homebrew/science <br />
2) brew install opencv <br />
3) cd /usr/local/Cellar/opencv/*youropencvversion* <br />

# setting up python

1) cd /Library/Python/2.7/site-packages/ <br />
2) ln -s /usr/local/Cellar/opencv/*youropencvversion*/lib/python2.7/site-packages/cv.py cv.py <br />
3) ln -s /usr/local/Cellar/opencv/*youropencvversion*/lib/python2.7/site-packages/cv2.so cv2.so <br />

# setting up pythonpath

1) cd <br />
2) sudo nano ~/.bash_profile <br />
then add the following line <br />
3) export PYTHONPATH=`brew --prefix`/lib/python2.7/site-packages:$PYTHONPATH <br />

# Success!

python -> import cv
