# Directory und File Handling

[Link zu Permissions](../Permissions.md)

## Directories
* **Directory Creation**
  > mkdir
  > mkdir test

  erstellt einen Folder

  > mkdir -r /FolderGibtsNochNicht/FolderGibtsAuchNicht

  Mit dem Schalter -r werden ganze Verzeichnisstrukturen übernommen


* **Remove Directory**
1. rmdir /test=> löscht lediglich leere Directories und keine Files
2. rm /test => löscht sowohl files als auch leere directories
3. rm -r /test => löscht rekursiv Directories

* **Change Directory**
  > cd
  >cd test = cd ./test
  >cd /etc/network/

  wechsel in das neue Verzeichnis // "Verzeichnis" = entweder absolutes oder Relatives Verzeichnis

  - Absolute Verzeichnise beginnen immer im Root-Verzeichnis **/**
  - Relative Verzeichnisse beginnen immer imaktuelle Verzeichnis **.**

Es ist egal ob ich zum schluss das "/" angebe oder nicht sprich 

  1. Der Befehl cd nimmt Pfadangaben als Parameter entgegen. Diese können wir absolut oder
  relativ angeben
       1. Absolute Pfade
  Starten mit einem / und beschreiben den Pfad zum gewünschten Verzeichnis
  ausgehend vom obersten Punkt im Dateisystem
       1. Relative Pfade
  Beschreiben den Weg zum Ziel ausgehend v*m aktuellen Standort
  2. Die Variable $OLDPWD enthält das vorige Verzeichnis, indem man sich befunden hat


  ## Files

* **Erstellen eines File**
  1. touch
  2. mit Editor
  3. mit Umleitung == echo "Test" >> FileName.txt

* **Kopie eines File**
  >cp file1 file2

* **Kopie eines Dir**
  >cp -r Dir1 Dir2

* **Verschieben/Umbenennen**
  >mv -r Dir1 Dir2
  >mv file1 file2



* **Links eines files**
  >ln -r Dir1 Dir2