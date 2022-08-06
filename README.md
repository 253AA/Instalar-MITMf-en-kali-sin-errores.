# Instalar-MITMf-en-kali-sin-errores.
```
sudo apt install python2-dev python-setuptools libpcap0.8-dev libnetfilter-queue-dev libssl-dev libjpeg-dev libxml2-dev libxslt1-dev libcapstone4 libcapstone-dev libffi-dev file
```
```
sudo nano /etc/apt/sources.list
```
***Aqui tienes que pegar los siguientes repositorios:***
```
deb http://http.kali.org/kali kali-rolling main non-free contrib 
deb-src http://http.kali.org/kali kali-rolling main non-free contrib
```
**Continuamos desde la consola**
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install python3-pip -y
```
```
sudo apt install python-pip
```
```
sudo pip install virtualenvwrapper
```
```
sudo pip2 install virtualenvwrapper
```
```
sudo nano ~/.zshrc
```
***Aqui pega al inicio de la zsh el siguiente comando:***
```
source /usr/local/bin/virtualenvwrapper.sh
```
**Continuamos en nuestra consola**
```
mkvirtualenv MITMf -p /usr/bin/python2.7
```
```
git clone https://github.com/byt3bl33d3r/MITMf
```
```
cd MITMf && git submodule init && git submodule update --recursive
```
```
sudo pip install -r requirements.txt
```
```
sudo pip2 install ipy user_agents pyopenssl service_identity configobj Flask dnspython beautifulsoup4 capstone python-magic msgpack-python requests pypcap chardet pyinotify pycrypto pyasn1 cryptography Pillow netaddr scapy dnslib Twisted lxml pefile
```
```
./mitmf.py -h
```
# Iniciar MITMf

```
cd MITMf
```
```
mkvirtualenv MITMf -p /usr/bin/python2.7
```
```
./mitmf.py -h
```

