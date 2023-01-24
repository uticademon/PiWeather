# PiWeather Kiosk - using PiZeroW and Hyperpixel 4.0 rectangle
PiOS Buster Lite
Hyperpixel legacy for 3B+

# Install software - use hyperpixel4 legacy for 3B+
curl -sSL https://get.pimoroni.com/hyperpixel4 | bash

sudo apt-get install --no-install-recommends xserver-xorg x11-xserver-utils xinit openbox
sudo apt-get install --no-install-recommends chromium-browser
sudo apt install xdotool

# Add ttf fonts to system
mkdir .fonts in home directory

place contents of Fonts folder into .fonts
load fonts into system using:

fc-cache -v -f

# Auto start browser
add .bash_profile file to home directory

# Display open tabs
make loop.sh executable (chmod u+x)
./loop.sh &

# Change urls
sudo nano /etc/xdg/openbox/autostart
