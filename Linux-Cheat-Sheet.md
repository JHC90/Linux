# Cheatsheet - Linux

## Install-Quick&Dirty
* sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get dist-upgrade -y && sudo reboot
* sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get dist-upgrade -y && sudo shutdown -f -t 0
* sudo apt-get install openssh-server
* sudo apt install net-tools

<hr>
## Basic Command-Navigation

<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Umsetzung</th>
    <th> mögliche Parameter</th>
  </tr>
  <tr>
    <td>clear</td>
    <td>löscht die Ausgabe auf der Kommandozeile</td>
    <td><br>
  </td>
  <tr>
    <td>pwd</td>
    <td>zeigt das aktuelle Verzeichnis</td>
    <td><br>
  </td>
  <tr>
    <td>mkdir Verzeichnis</td>
    <td>erstellt einen Folder</td>
    <td><br>
  </td>
  <tr>
    <td>cd "Verzeichnis"</td>
    <td>wechsel in das neue Verzeichnis // "Verzeichnis" = entweder absolutes oder Relatives Verzeichnis</td>
    <td>cd .. | wechsel ins höhere Verzeichnis || cd / = Wechsel ins root Verzeichnis || cd ~ = wechsel ins Home-Verzeichnis</td>
  </tr>
   <tr>
    <td>ls</td>
    <td>listet den Inhalt desVerzeichnises</td>
    <td>ls -a || auch die versteckten Dateien & </td>
  </tr>
  <tr>
    <td>man ls</td>
    <td>hier gehts um den "man" Bereich => ruft die Hilfe zu dem Befehl ls auf</td>
    <td></td>
  </tr>
  <tr>
    <td>echo "Hallo Linux"</td>
    <td>gibt den String Hallo Linux auf der Konsole aus</td>
    <td></td>
  </tr> 
  
</table>

<hr>

## Basic System-Abfragen

<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Umsetzung</th>
    <th> mögliche Parameter</th>
  </tr>
  <tr>
    <td>sudo hostnamectl set-hostname master-node</td>
    <td>Ändert den Hostname</td>
    <td>in diesem Falle auf den Namen "Master-node" </td>
  </tr>
  <tr>
    <td>hostname</td>
    <td>gibt den Hostname zurück</td>
    <td></td>
  </tr>
  <tr>
    <td>whoami</td>
    <td>gibt den User zurück</td>
    <td></td>
  </tr>
  <tr>
    <td>cat /etc/os-release</td>
    <td>Liefert infos über die OS-Version</td>
    <td><img src="./imgs/2020-04-11-08-37-07.png"></td>
  </tr> 
  
</table>





<hr>

## Basic File-Interaction

<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Umsetzung</th>
    <th> mögliche Parameter</th>
  </tr>
  <tr>
    <td>touch Datei.txt </td>
    <td>Erstelle eine neue Datei, mehr nicht :-)</td>
    <td></td>
  <tr>
    <td><br> nano Datei.txt ||<br> vi Datei.txt</td>
    <td>Erstelle eine Neue datei und wechsel direkt hinein mit dem jeweiligen Editor <a href="./Editoren/vi.md" >Vi</a> oder mit <a href="./Editoren/nano.md" >Nano</a></td>
    <td></td>
  <tr>
    <td>cat Datei.txt</td>
    <td>öffnet die Datei auf der Konsole</td>
    <td></td>
  </tr>
  
   <tr>
    <td>echo "Hallo Linux" > Datei.txt || cat Datei.txt</td>
    <td>Schreibt den String "Hallo Linux" in die Datei, wenn die Datei bereits besteht wird diese überschrieben</td>
    <td></td>
  </tr>
</table>

---
## Basic Networking
sudo apt install net-tools


<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Umsetzung</th>
    <th> mögliche Parameter</th>
  </tr>
  <tr>
    <td>sudo ip link set dev eth0 up </td>
    <td>Schaltet eine NIC ein</td>
    <td>Das kann brutal Nervig sein => ändern der /etc/network/interfaces -Datei, und den Auto boot setzten  bspw "aut eth1" reinsetzen</td>
  </tr>
   <tr>
    <td>sudo dhclient -v</td>
    <td>erneuert die IP//ipconfig release & renew in Linux</td>
    <td></td>
  </tr>
  <tr>
    <td>dig +short myip.opendns.com @resolver1.opendns.com</td>
    <td>zeigt die public ip</td>
    <td></td>
  </tr>  
  <tr>
    <td>nano /etc/network/interfaces</td>
    <td>in diesem File erstellt man die statischen IPs => muss logischerweise somit auch im DHCP so hinterlegt sein // v.a wenn ein Linux server vorliegt sollte der immer eine statische IP haben</td>
    <td>iface eth0 inet static ( hier steht normalerweise statt static, dhcp )<br> 
    
  
  address 192.168.1.1 <br>

netmask 255.255.255.0<br>

network 192.168.1.0<br>

broadcast 192.168.1.255<br>

gateway 192.168.1.254</td>
  </tr>  
<table>

