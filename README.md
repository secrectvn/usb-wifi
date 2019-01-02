

# Building
- git clone https://github.com/secrectvn/usb-wifi.git
- cd usb-wifi
- sudo apt-get install build-essential linux-headers-$(uname -r)
- make clean
- make
- sudo make install

# Building with DKMS
```bash
$ sudo apt-get install dkms  # if you've already installed dkms, skip this step.
$ sudo cp -R . /usr/src/mt7610u_sta-1.0
$ sudo dkms add mt7610u_sta/1.0
$ sudo dkms build mt7610u_sta/1.0
$ sudo dkms install mt7610u_sta/1.0
```

