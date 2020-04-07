# Samba Simple via Webmin
Mit Samba Simple meine ich eine Version ohne großartige Security Policies
Das Laufwerk wird hier via WebminGui erstellt



## Vorarbeit
1. Install Ubuntu Server Headless // Vorsicht beim [RolloutUbuntuOnHyperV](../RolloutUbunutServerOnHyperV/RolloutUbuntuServerHyperV.md)
> sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get dist-upgrade && sudo reboot
2. Install Openssh
3. install [webmin](./RolloutWebmin.md)

## Samba Installation from Mangament Laptop Web-Gui
Nach folgendem [Youtube-Tutorial](https://www.youtube.com/watch?v=XPh1vOKTjlQ)

1. unused Modules =>sambashare für Windows
   ![](imgs/2020-04-06-21-07-25.png)

2. Anlegen eines local Users<br>
   system => "Users and Groups"
   1. SambaUserLocal || SambaGroupLocal<br>
   ![](imgs/2020-04-06-21-30-32.png)

   2. SambaUser || SambaGroup => brauchts später bei der Anmeldung: ![](imgs/2020-04-06-21-33-35.png)

   

3. file Manager
Anlegen eines Neuen Dir in home für die Shared-Files
![](imgs/2020-04-06-21-14-51.png)
ändern der Permissions // zwar für jeden Zugänglich, dennoch habe ich vorher einen User angelegt. Diesen User brauch ich da Windows 10 als Samba Client keinen Zugangn ohne Credentials zulässt.
![](imgs/2020-04-06-21-15-24.png)
![](imgs/2020-04-06-21-17-39.png)

3. Samba-Connection
   1. Create File Share
   ![](imgs/2020-04-06-21-19-22.png)
   erstelle den SambaShare auf dem vorherigen Laufwerk:
   ![](imgs/2020-04-06-21-21-25.png)

   2. edit security
   ![](imgs/2020-04-06-21-23-19.png)
    ![](imgs/2020-04-06-21-24-34.png)
    erlaube writeable & guest zugriff
   ![](imgs/2020-04-06-21-24-14.png)

4. Anlegen eines Users:<br>
   SambaUserLocal || SambaGroupLocal<br>
   SambaUser || SambaGroup
5. Directory anlegen, das gesharet wird
   1. Vollzugriff gewährleisten
