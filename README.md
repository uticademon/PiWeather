# PiWeather

# add ttf fonts to system
mkdir .fonts in home directory

place contents of Fonts folder into .fonts
load fonts into system using:

fc-cache -v -f

# auto start browser
add .bash_profile file to home directory

# display open tabs
make loop.sh executable (chmod u+x)
./loop.sh &

# change urls
sudo nano /etc/xdg/openbox/autostart
