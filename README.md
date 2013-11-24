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
# Unity Tweak Tool
```shell
sudo apt-get install unity-tweak-tool
```
# Disable Shopping Suggestions
```shell
gsettings set com.canonical.Unity.Lenses disabled-scopes "['more_suggestions-amazon.scope', 'more_suggestions-u1ms.scope', 'more_suggestions-populartracks.scope', 'music-musicstore.scope', 'more_suggestions-ebay.scope', 'more_suggestions-ubuntushop.scope', 'more_suggestions-skimlinks.scope']"
```
# TLP
```shell
sudo add-apt-repository ppa:linrunner/tlp && \
sudo apt-get update && \
sudo apt-get install tlp tlp-rdw && \
sudo tlp start
```
# Bumblebee
```shell
sudo apt-get install bumblebee bumblebee-nvidia
```
Fix optirun bug
```shell
sudo ln -s /usr/lib/x86_64-linux-gnu/libturbojpeg.so.0 /usr/lib/x86_64-linux-gnu/libturbojpeg.so
```
# Restricted Extras
```shell
sudo apt-get install ubuntu-restricted-extras libavformat-extra-53 libavcodec-extra-53
```
# VLC
```shell
sudo apt-get install vlc
```
# Open terminal here
```shell
sudo apt-get install nautilus-open-terminal && \
nautilus -q
```


