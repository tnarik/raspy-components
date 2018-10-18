# Unicorn-pHAT

Requires 


## Official

Run (on the Pi):

```
\curl -sS get.pimoroni.com/unicornhat | bash
```

## Explicit

Library:

```
pip install unicornhat
```

## Notes

Unicorn HAT/pHAT uses PWM for its data, which is also used for audio output through the headphone jack of the Pi. This could lead to some trouble depending on the distribution and the configuration of the Pi. One sympton is LEDs partially turning on. To correct this HDMI audio should be forced. 

To do so, please ensure the following is setup in `/boot/config.txt`:

```
hdmi_force_hotplug=1
```

With the PiZero that translates into installing Jessie Lite instead of Jessie (it seems to do the trick, probably because sound drivers are not loaded).

*** NEEDS ROOT TO EXECUTE (due to the access to /dev/mem) ***