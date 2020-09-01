# Sniper 7.2 Installation
Notice: The official website of Sniper has a guide of installation. However, it is out of date. It only fits old Sniper versions. If you choose Sniper 7.1, do not follow their instruction.  

# Environment  
Ubuntu 20.04  
Sniper 7.2
gcc 7.3  
g++ 7 

# Installing
* Download Sniper 7.2 from their official website http://snipersim.org/w/Download  or just use ` $ wget http://snipersim.org/download/aa88c9767229ce77/packages/sniper-latest.tgz`

* Download Pin kit 3.7 https://software.intel.com/en-us/articles/pin-a-binary-instrumentation-tool-downloads or request here [driver for 3.7](https://drive.google.com/file/d/1KeBtlAwSmhglFz0JPi5aCRkweyylbW-w/view?usp=drive_web)
* Extract Pin into sniper/pin_kit  

```bash
$sudo apt-get install libc6-dev-i386  
$g++ --version, to get your_g++_version  
$sudo apt-get install g++-your_g++_version-multilib  
$sudo apt-get install lib32z1-dev  
$make  
```

* If make failed, there will be a notice for the missing part, install those missing part.  
* If "usr/bin/env: ‘python’: No such file or directory", check your environment. Usually, if your python version is higher, it cannot be detected. Use following command to install python  
$sudo apt-get install python-minimal  

# Test
```bash 
$cd test/fft  
$make run  
```

