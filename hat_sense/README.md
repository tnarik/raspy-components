# Sense-Hat

Requirements:

```
sudo apt-get install libjpeg-dev python-rtimulib
sudo apt-get install git
pip install -e 'git+https://github.com/RPi-Distro/RTIMULib.git#egg=rtimulib&subdirectory=Linux/python'
```
Also requires enabling I2C. This can be done via the Advanced Options of `sudo raspi-config` or manually (from the Raspberry Pi) via:

```
echo -e "\ni2c-dev" | sudo tee -a /etc/modules
echo -e "\ndtparam=i2c1=on\ndtparam=i2c_arm=on" | sudo tee -a /boot/config.txt
```

The library:

```
pip install sense-hat
```
