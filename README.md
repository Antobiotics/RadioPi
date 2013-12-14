RadioPi
=======

Vintage radio on the raspberry pi


### Raspberry Pi login:
```
user: radio
pass: buddha

user: pi
pass: raspberry
```

### Dependencies:

```
sudo apt-get install mpd mpc
```

### Modules:

```
sudo modprobe snd_bcm2835
```

### Setup:

#### Setting up MPD:

#### Conf files:

```
/etc/mpd.conf

audio_output {
    type                    "oss"
    name                    "My OSS Device"
    device                  "/dev/sound/dsp"
    format                  "44100:16:2"
}

```
[mpd wiki](http://www.musicpd.org/)
#### Service Managment

```
sudo /etc/init.d/mpd restart
```

### Usage:

```
mpc add http://relay3.slayradio.org:8000/
```
