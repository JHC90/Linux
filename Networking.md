# Networking

## Debian
nutzt zentral Datei Namens /etc/interfaces. Ubuntu nutzt Networkmanager

### GUI
![](imgs/2020-06-19-07-11-54.png)

**DHCP / Statisch**

![](imgs/2020-06-19-07-13-04.png)

### CLI


## Suse
nutzt Yast für die Configs.
CentOS = Datei /etc/sysconfig/network-scripts


![](imgs/2020-06-19-07-23-07.png)

> service network restart 

Für Statische IP 

![](imgs/2020-06-19-07-28-06.png)
Dann muss noch zusätzlich die DNS-Einträge hinterlegt werden


> vi /etc/resolv.conf
dort dann die eigenen DNS-Server hinzufügen, bzw hier ist eine DNS-Server hinterlegt

![](imgs/2020-06-19-07-31-24.png)

---

* Im Verzeichnis /etc/sysconfig/network-scripts befinden sich die Netzwerk-bezogenen
Einstellungen in Form von Konfigurationsdateien und Skripts
* Mit einem Texteditor können wir die Konfigurationsdateien entsprechend anpassen


> service network restart


