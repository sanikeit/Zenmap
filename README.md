# Zenmap
Zenmap (GUI)

#Kali
As we all know zenmap is removed from kali so, here are the things you need to install it again.
first install both python files and Install zenmap.

#Ubuntu

Install ZenMap on Ubuntu 20.04 LTS Focal Linux
As Zenmap is not available anymore in the official repository of Ubuntu, thus we have to download and install it manually.

Update system
Run the system update command that will rebuild apt-cache and also update the already installed packages of our system.

sudo apt update
 

Install Nmap
Although while installing Zenamp, the Nmap would already be there, however, for those who want to try it out using the command line, installing it would be a nice idea.

sudo apt install nmap
 

Install Python GTK
Zenmap uses Python GTK for creating a graphical user interface, thus we have to install that as well on our Ubuntu 20.04 system before going forward.

Visit the http://archive.ubuntu.com/ubuntu/pool/universe/p/pygtk/and download the latest version. Example:

wget http://archive.ubuntu.com/ubuntu/pool/universe/p/pygtk/python-gtk2_2.24.0-5.1ubuntu2_amd64.deb

sudo apt install ./python-gtk2_2.24.0-5.1ubuntu2_amd64.deb 
 

Download and install Zenmap debian packge
As we are doing this manually, the current available Debian package for installation is zenmap v 7.x, here we are downloading that using the below command:

Go to http://archive.ubuntu.com/ubuntu/pool/universe/n/nmap/ and download the latest Zenmap Debian package.

You can also copy the link and use it with wget command:

wget http://archive.ubuntu.com/ubuntu/pool/universe/n/nmap/zenmap_7.60-1ubuntu5_all.deb
Now install it…

sudo apt install ./zenmap_7.60-1ubuntu5_all.deb
 

Run Zenmap as the root user
To access all the features, the Zenmap needs to be run as a root user, therefore on your command terminal simply type:

sudo zenmap
 

Updated Version
In case you want the current updated version of the Zenmap which is available on the official website of Nmap but in the RMP package format. Therefore, to use it on Debian-based systems, first, we have to convert the RMP package to Deb and for that, we can use the Alien tool.

Install alien

sudo apt install alien
 

Convert Zenmap RPM to Deb package
Go to the official website of Nmap and download the Zenmap rpm package. You can also use wget tool along with the link of the Package available on the website,  in case want to download using the terminal.

Convert Zenmap RPM package to Ubuntu Debian

For example, while doing the article the latest version was 7.91. If you have downloaded using the browser then it will be in the Downloads folder.

cd Downloads
check it

ls
After that use the alien command to convert it.

sudo alien zenmap-7.91-1.noarch.rpm
Now, you will have the Deb file at the same location, now install it.

sudo apt install ./zenmap_7.91-2_all.deb
Install updated version of nmap and zenmap on Ubuntu 20.04
