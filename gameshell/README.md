
## deprecated 

#wget -O -  https://raw.githubusercontent.com/clockworkpi/apt/main/debian/KEY.gpg | sudo apt-key add - 

wget -q -O- https://raw.githubusercontent.com/clockworkpi/apt/main/gameshell/KEY.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/clockworkpi.gpg

echo "deb https://raw.githubusercontent.com/clockworkpi/apt/main/gameshell/ stable main" | sudo tee -a /etc/apt/sources.list.d/clockworkpi\_gs.list

sudo apt update

