Install OS
==========
Elementary OS or
Lubuntu

Install chrome
==============
sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
sudo apt-get update
sudo apt-get install google-chrome stable

Install Nodejs
==============
sudo add-apt-repository ppa:chris-lea/node.js
sudo apt-get update
sudo apt-get install python-software-properties python g++ make nodejs

Install Protractor
==================
Install according to: (use sudo)
https://egghead.io/lessons/angularjs-getting-started-with-protractor

Install jdk
===========
sudo apt-get install openjdk-7-jre

Install grunt and bower
=======================
sudo npm install -g grunt
sudo npm install -g bower

Edit /etc/hosts
===============
add <ip for system under test> <url for system under test>
example:
172.5.16.148   svm

Export appliance
================
cd /Applications/VMware\ Fusion.app/Contents/Library/VMware\ OVF\ Tool
./ovftool --acceptAllEulas /Users/brandon/Documents/Virtual Machines.localized/LTestAgent.vmwarevm/LTestAgent.vmx ~/VMWareShared/TestAgent.ova
