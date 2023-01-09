# apt

```
#wget -O - https://raw.githubusercontent.com/clockworkpi/apt/main/debian/KEY.gpg | sudo apt-key add -  

wget -q -O- https://raw.githubusercontent.com/clockworkpi/apt/main/debian/KEY.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/clockworkpi.gpg

echo "deb https://raw.githubusercontent.com/clockworkpi/apt/main/debian/ stable main" | sudo tee  /etc/apt/sources.list.d/clockworkpi.list  
```

