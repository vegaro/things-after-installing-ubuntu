Things to do after installing Ubuntu
=========================
Last update was made for Ubuntu 13.10 Saucy Salamander
#Git
```shell
sudo apt-get install git && \
git config --global user.name "Cesar de la Vega" && \
git config --global user.email "cesarvegaro@gmail.com" && \ 
git config --global credential.helper cache && \
git config --global credential.helper 'cache --timeout=3600' && \
ssh-keygen -t rsa -C "cesarvegaro@gmail.com" && \
ssh-add ~/.ssh/id_rsa && \
sudo apt-get install xclip && \
xclip -sel clip < ~/.ssh/id_rsa.pub
```
Paste to GitHub

#Sublime Text
```shell
sudo add-apt-repository ppa:webupd8team/sublime-text-2 && \
sudo apt-get update && \
sudo apt-get install sublime-text
```
#Oh-my-zsh
```shell
sudo apt-get install zsh && \
sudo wget --no-check-certificate https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh
```
#Chrome
```shell
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - && \
sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list' && \
sudo apt-get update && \
sudo apt-get install google-chrome-stable
```
#Skype
```shell
sudo sh -c "echo 'deb http://archive.canonical.com/ubuntu/ saucy partner' >> /etc/apt/sources.list.d/canonical_partner.list" && \
sudo apt-get update && \
sudo apt-get install skype
```


