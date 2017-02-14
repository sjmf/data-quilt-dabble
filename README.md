# Double Dabble Data Quilt Hack

Graphs have never been so cuddly!

# Setup

We used the [Adafruit Capacitive Touch hat](https://www.adafruit.com/product/2340) 
for Raspberry Pi. Grab the git repo for the chip here:

```
git clone https://github.com/adafruit/Adafruit_Python_MPR121.git
```

I modified the `keyboard.py` example to map letters instead of arrow keys.
The diff is included in the file `patch.diff`. Apply with: 

```
cd Adafruit_Python_MPR121
git apply ../patch.diff
```

Running the keyboard example maps the touch sensors to key presses which are
handled in `index.html`, which we ran fullscreen in Chrome.



