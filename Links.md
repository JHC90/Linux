#Links


* Ein Link ist ein Verweis auf eine andere Datei oder ein Verzeichnis
* Hardlinks (= vgl eine Datei mit mehreren Namen)
    * Es handelt es sich um ein- und dieselbe Datei auf die mittels eines Inodes
referenziert wird. Dies ist ein Verweis auf eine Datei, allerdings in der DateisystemTabelle – quasi die ID der Datei.
    * Hardlinks können nur innerhalb einer Partition existieren
    * Hardlinks können nur auf Dateien angewendet werden, nicht auf Verzeichnisse
    * Wird ein Hardlink gelöscht, so besteht die Originaldatei noch weiter
* Softlinks / Symbolic Links, kurz: Symlinks
  * Mit Symlinks können Verweise, also Links partitionsübergreifend erstellt werden
    * Das gilt gleichermaßen für Dateien und Verzeichnisse
    * Sie    sind deutlich einfacher zu erkennen, da sie mit Pfaden arbeiten
    * Wird die Originaldatei gelöscht, existiert keine Kopie mehr