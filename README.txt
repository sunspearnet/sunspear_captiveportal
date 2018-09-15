Connect to the tomato router
username is root
password is admin
Under Administration - Scripts - Wan Up, paste the following lines
++++++++++++++++++++++++++++
#!/bin/sh
cd /tmp/splashd
rm splash.html
rm bg.jpg
wget https://raw.githubusercontent.com/sunspearnet/sunspear_captiveportal/master/splash.html
wget https://github.com/sunspearnet/sunspear_captiveportal/raw/18f2b2b628b8ea9c9c981d37f41aa848c072ed66/bg.jpg -O bg.jpg
++++++++++++++++++++++++++++
