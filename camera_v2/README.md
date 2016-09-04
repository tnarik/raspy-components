# Camera Module v2


## Official (on the Pi)

Use the commands `raspistill` or `raspivid`

## Explicit

Library:

```
pip install picamera
```

## Notes

The use of the Camera V2 requires enabling it. This can be done:

- from the command line:

```
sudo raspi-config nonint do_camera 0
```

- via the main options of `sudo raspi-config`.
