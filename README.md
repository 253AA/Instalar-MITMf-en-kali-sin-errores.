# Instalar-MITMf-en-kali-sin-errores.
**Iniciamos instalando pip2**
```
wget https://gist.githubusercontent.com/anir0y/a20246e26dcb2ebf1b44a0e1d989f5d1/raw/a9908e5dd147f0b6eb71ec51f9845fafe7fb8a7f/pip2%2520install -O run.sh 
```
```
chmod +x run.sh
```
```
./run.sh
```
**Instalando todas las dependencias**
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install python2-dev python-setuptools libpcap0.8-dev libnetfilter-queue-dev libssl-dev libjpeg-dev libxml2-dev libxslt1-dev libcapstone4 libcapstone-dev libffi-dev file
```
```
sudo apt install python3-pip -y
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
sudo ./mitmf.py -h
```

