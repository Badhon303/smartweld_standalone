# smartweld_standalone

sudo apt update && sudo apt upgrade  
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -  
sudo apt-get install nodejs  

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -  
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list  
sudo apt install yarn  
sudo curl --compressed -o- -L https://yarnpkg.com/install.sh | bash  
restart terminal & yarn --version  

sudo apt-get install tmux  
tmux new -s mysession  
tmux attach-session -t mysession  
ctrl+b d  

sudo ufw status  
sudo ufw enable  
Security group expose 3000  

sudo apt install -y mosquitto  
sudo systemctl status mosquitto  
sudo systemctl stop mosquitto  
sudo systemctl start mosquitto  
sudo systemctl restart mosquitto  


# oracle  
$ sudo iptables -I INPUT 6 -m state --state NEW -p tcp --dport 80 -j ACCEPT  
$ sudo netfilter-persistent save  
