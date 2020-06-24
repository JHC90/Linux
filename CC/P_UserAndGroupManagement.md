# Usermanagement
[Theorie zu User und Gruppen Management](../UserUndGruppen.md)

1. Useradd
   1. Useradd um einen Systemuser anzulegen => **Kein** Home-Verzeichnis
   > useradd asterix -r
   > passwd asterix

   2. Useradd um einen Useraccount anzulegen => hat ein Home-Verzeichnis
   > useradd -m obelix -c "Kommentart oder Name oder whateveer" -g Hauptgruppe -G zusäzlicheGruppen -s /bin/bash -d /home/Obelix
   > passwd obelix


## Eigene Programme für die Userverwaltung
1. addUser
2. delUser