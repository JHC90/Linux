# Rollout Webmin

1. Rollout Ubuntu(headles)
2. update / Upgrade / distupgrade
3. Checkpoint on HyperV
4. Rollout 1: 1 nach diesem [link](https://vitux.com/install-and-configure-webmin-on-ubuntu/)
5. short notice
   1. >sudo nano /etc/apt/sources.list

   füge folgende Zeile am Ende der Datei ein:
   >deb http://download.webmin.com/download/repository sarge contrib
   2. >wget http://www.webmin.com/jcameron-key.asc
   3. >sudo apt-key add jcameron-key.asc
   4. >sudo apt update / Upgrade
   5. >sudo apt install webmin
   6. Done => warten bis durchgelaufen dann unter "webminServerIP":10000