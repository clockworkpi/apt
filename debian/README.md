# Raspberry pi CM3
### Enable SPI0

SPI0 is disabled by default. To enable it, use *raspi-config*, or ensure the line **dtparam=spi=on** isn't commented out in `/boot/config.txt`

add **dtoverlay=spi-gpio35-39** under **dtparam=spi=on**, then reboot

after reboot,make suer there is a `/dev/spidev0.0`


-------------------------------------------------------------------------------------------------------------------

wget -O -  https://raw.githubusercontent.com/clockworkpi/apt/main/debian/KEY.gpg | sudo apt-key add - 

echo "deb https://raw.githubusercontent.com/clockworkpi/apt/main/debian/ stable main" | sudo tee -a /etc/apt/sources.list.d/clockworkpi.list

sudo apt update

sudo apt install devterm-thermal-printer


### How to test

echo "this is a test" > /tmp/DEVTERM_PRINTER_IN
