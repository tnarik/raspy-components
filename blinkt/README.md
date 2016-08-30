# Blinkt!

To use the official library, run (on the Pi):

```
curl -sS get.pimoroni.com/blinkt | bash
```

Alternatively

```
pip install blinkt requests gpiozero rpi.gpio psutil
```

Legacy:

```
#apt-get install -y python-pip python-rpi.gpio python3-pip python3-rpi.gpio python-gpiozero python3-gpiozero python-psutil python3-psutil python-requests python3-requests
apt-get install -y python-pip python-rpi.gpio python3-pip python3-rpi.gpio python-gpiozero python3-gpiozero python-psutil python3-psutil
pip install blinkt requests
pip3 install blinkt requests
```

If you want to run some examples, you'll also need `tweepy`.