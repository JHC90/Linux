# Cheatsheet - Linux

## Install-Quick&Dirty
* sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get dist-upgrade && sudo reboot
* sudo apt-get install openssh-server
* sudo apt install net-tools

## Fragestellung ob es für die RemoteWartung via VSCode ssh key braucht
https://code.visualstudio.com/docs/remote/troubleshooting
  <hr>


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
    <td>cd .. | wechsel ins höhere Verzeichnis || cd / = Wechsel ins root Verzeichnis || cd ~ = wechsel ins Home-Verzeichnis<br>
  </td>
  <tr>
    <td>touch Datei.txt </td>
    <td>Erstelle eine neue Datei, mehr nicht :-)</td>
    <td><br>
  </td>
  <tr>
    <td><br> nano Datei.txt ||<br> vi Datei.txt</td>
    <td>Erstelle eine Neue datei und wechsel direkt hinein mit dem jeweiligen Editor <a href="./Editoren/vi.md" >Vi</a> oder mit <a href="./Editoren/nano.md" >Nano</a></td>
    <td><br>
  </td>
  <tr>
    <td>cat Datei.txt</td>
    <td>öffnet die Datei auf der Konsole</td>
    <td></td>
  </tr>
  <tr>
    <td>ls</td>
    <td>liste den Inhalt des Verzeichnises in dem man eben ist</td>
    <td>ls -a || liefert weitere Information, wie den Besitzer des Files etc
  </td>
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
  <tr>
    <td>echo "Hallo Linux" > Datei.txt || cat Datei.txt</td>
    <td>Schreibt den String "Hallo Linux" in die Datei, wenn die Datei bereits besteht wird diese überschrieben</td>
    <td></td>
  </tr>
  <tr>
    <td>echo "Hallo Linux" >> Datei.txt || cat Datei.txt</td>
    <td>Schreibt den String "Hallo Linux" in die Datei, wenn die Datei bereits besteht wird der aktuelle Echo der bestehenden Datei angehängt</td>
    <td></td>
  </tr>
  <tr>
    <td>cp DateiName.txt DateiName2.txt</td>
    <td>Kopiert die Datei, wenn ein anderes Verzeichnis gewünscht, dann muss dieses entsprechenden angebgen werden. Hier wurde es lediglich im gleichen Folder kopiert</td>
    <td></td>
  </tr>
  <tr>
    <td>mv Datei.txt Datei2.txt</td>
    <td>Verschieben & umbenennen von Dateien</td>
    <td></td>
  </tr>

  <tr>
    <td>rm DateiName.txt</td>
    <td>löscht die Datei</td>
    <td>rm DateiName.txt -f || zwang die Datei zu löschen <br></td>
  </tr>
  <tr>
    <td>rm -r Verzeichnis</td>
    <td>löscht ein Verzeichnis</td>
    <td>der Schalter -r hat hier die Bedeutung rekursiv<br></td>
  </tr>
  <tr>
    <td>ps</td>
    <td>zeigt alle laufenden Prozesse</td>
    <td>ps aux<br>
    ps aux | grep mogod</td>
  </tr>
  <tr>
    <td>dig +short myip.opendns.com @resolver1.opendns.com</td>
    <td>zeigt die public ip</td>
    <td></td>
  </tr>
  
<table>