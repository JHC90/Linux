# OpenSSH
mit OpenSSH wird ein SSH-Server auf dem Linux installiert, der sich für mich bewährt hat. Vor allem mit dem SSH-Client [MobaXTerm](https://www.google.com/search?client=firefox-b-d&q=mobaterm)

## Rollout
1. nach dem Rollout des OS erst den Standard:
 > sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get dist-upgrade && sudo reboot

 2. sudo apt-get install openssh-server

Ab jetzt ist der Server aus dem LAN für SSH-Clients mit dem Standard-User erreichbar. Der User root ist standardmäßig nicht für SSH freigeschalten. Jedoch kann in der laufenden SSH-Verbindung des Standardnutzers mit "Sudo su " gearbeitet werden.
