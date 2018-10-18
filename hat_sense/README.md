# Sense-Hat


## Official (on the Pi)

```
wget -O - http://www.raspberrypi.org/files/astro-pi/astro-pi-install.sh --no-check-certificate | bash
```

## Explicit

Requirements:

```
sudo apt-get install libjpeg-dev python-rtimulib
sudo apt-get install git
pip install -e 'git+https://github.com/RPi-Distro/RTIMULib.git#egg=rtimulib&subdirectory=Linux/python'
```

Library:

```
pip install sense-hat
```

## Notes

The use of the Sense-Hat requires enabling I2C. This can be done:

- from the command line:

```
sudo raspi-config nonint do_i2c 0
```

- via the `Advanced Options` of `sudo raspi-config`.
- or completely manually (on the Pi) via:

```
echo -e "\ni2c-dev" | sudo tee -a /etc/modules
echo -e "\ndtparam=i2c1=on\ndtparam=i2c_arm=on" | sudo tee -a /boot/config.txt
```

