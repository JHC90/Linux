# Rollout Webmin

1. Rollout Ubuntu(Headles)
2. [Standard-Update-Upgrade-DistUpgrade-Reboot](./../RolloutUbunutServerOnHyperV/RolloutUbuntuServerHyperV.md#UpdateUpgradeDistUpgrade)
3. Checkpoint on HyperV
4. Rollout 1: 1 nach diesem [link](https://vitux.com/install-and-configure-webmin-on-ubuntu/)
5. short notice
   1. >sudo nano /etc/apt/sources.list

   füge folgende Zeile am Ende der Datei ein:
   >deb http://download.webmin.com/download/repository sarge contrib
   ![](imgs/2020-05-06-11-31-12.png)
   1. >wget http://www.webmin.com/jcameron-key.asc
   2. >sudo apt-key add jcameron-key.asc
   3. >sudo apt-get update && sudo apt-get upgrade
   4. >sudo apt install webmin
   5. Done => warten bis durchgelaufen dann unter "webminServerIP":10000 // https://jupyterServer:10000
   6. Die Credentials sind initial jene, mit welchen webmin auf der CLI installiert wurde.
   
   ![](imgs/2020-05-07-14-42-40.png)
   7. ggf Checkpoint im HyperVisor