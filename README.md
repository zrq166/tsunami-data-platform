# TsunamiDataDownload
A SJTU PRP project, which can download tsunami caused by earthquake data by a button. <br>
Author: Junwei Deng, Runqing Zhou

## Version

### V0.1 (2018.5.12)
### V0.2 (Internal Version)
### V0.3 (2018.8.28)
### V1.0beta (plan to be released on mid December)
### V1.0 (plan to be released on 2019.1.1)
Include bug fix, code restruction and a more user-friendly command line interface. So, users are recommanded to wait until then. Moreover, a library is on schedule with a fully written document so that tsunami researcher can tailor their own program easily.

## Install

### Windows

#### 0.Make sure you have installed python3.x(3.6 is recommanded) and pip3 and some necessary library.

You can check it like this.<br>
![avatar](./image/version.JPG)<br> 
Install from https://www.python.org/<br>
And make sure you have these package.(Version is just for recommendation)<br>
![avatar](./image/13.jpg) <br>
You can follow the instructions bellow to install them.

#### 1.	Press Win+R together and enter cmd.

 ![avatar](./image/1.png)<br>

#### 2.	Install packages

Enter pip install requests just as the following picture shows.

![avatar](./image/2.png) 

If the installation is successful, it will show as follows.
 
![avatar](./image/3.png) 

Similarly, enter pip install numpy.
![avatar](./image/4.png)  

![avatar](./image/5.png) 

The installation of the next three ones are all similar.<br>
 ![avatar](./image/6.png) 

 ![avatar](./image/7.png) 

 ![avatar](./image/8.png) 

#### 3.	Install an important package called basemap

Go to *http://www.lfd.uci.edu/~gohlke/pythonlibs/*.
On the page, press CTRL +F and enter basemap and pyproj for quick positioning.  There are several versions, and you need to choose one of them. 32 and 64 on win refer to the Python version installed, and the Numbers behind cp refer to the Python version.<br>
![avatar](./image/9.png) <br>
![avatar](./image/14.JPG) <br>
Download one of them to a file. Next, you need change directory to the file and enter pip install xxx(xxx is the name of .whl you have downloaded)
For example, I download basemap-1.1.0-cp36-cp36m-win32.whl, and I put it in the directory E:\JI\prp\p1. So I need to enter the following things in cmd.
 ![avatar](./image/10.png) 

#### 4.Install another two packages

![avatar](./image/11.png) 

![avatar](./image/12.png)

### Note:

Please shut down the anti-virus software(especially 360) when you run the program.<br>
![what](http://code.cdn.mozilla.net/for-firefox/badges/assets/I-Use-Firefox.png)
 



## Update Information(until 2018.8.28)
### 2018.03.07 Deng
Creat this project and upload:<br> 
1. settings.py(for Input index)<br>
2. GetUsgsData.py(for get earthquake information and save it in ./cache/earthquake.csv)<br>
3. UpdateDartStation.py(for get all Dart stations' information and save them in ./cache/DartStationRecord)<br>
4. PRP_GUI.py(Demo GUI)
### 2018.03.09 Deng
Upload:<br>
1. earthquake.py(a class for earthquake)<br>
2. GetDartData(for get a certain Dart station data when a certain earthquake happened and calculate the relative time from the earthquake and the water height)<br>
3. ./cashe(for Professor to check if the modules do things correctly)<br>
fixed:<br>
1. README.md(for better record the update information)
### 2018.03.23 Zhou
Upload:<br>
1. ChooseDartStation.py(choose for five stations nearest to the earthquake.epi)<br>
### 2018.03.23 Deng
Upload:<br>
1. RemoveTidesPolynomialFit.py(Signal process part using polynomial fit)<br>
2. main.py(just run it and get the result)[partly finished]<br>
fixed:<br>
1. README.md<br>
2. bug fixed<br>
3. add two interesting result pictures(I believe DartData_52402.jpg is a Tsunami I catch for the earthquake at 2018-02-25T17:44:43.920Z)
### 2018.03.27 Deng
Fixed:<br>
1. Common line UI.<br>
2. File system<br>
3. Dpi of picture generated by matplotlib <br>
4. Bunch of bugs(bug 9999.000)
### 2018.04.01 Zhou
Fixed:<br>
1. UpdateDartStation.py(make it able to decide whether we need to update the station list)<br>
### 2018.04.01 Deng
Upload:<br>
1. RemoveTidesFilter.py(used to remove the tides by high-pass filter)<br>
Fixed:(main.py/RemoveTidesPolynomialFit.py)<br>
2. filesystem optimize<br>
3. bug fixed<br>
4. detailed information are added<br>
### 2018.05.12 Deng
All project has been pushed.<br>
Version 0.1
### 2018.08.28 Deng
Huge amount of Bug Fixed<br>
Version 0.3
