# Shell

• Die Shell bezeichnet die Benutzerschnittstelle zwischen Anwender und (Unix-)System, also ein
Programm, um Kommandos zu verarbeiten, etwa auf Dateien zuzugreifen oder andere
Programme auszuführen
• Die Bash-Shell (Bourne-again shell) ist die Standard-Shell in Linux, du kannst sie z.B. mit einem
Terminal ausführen
• Man unterscheidet die mit Passwort gesicherten Login-Shells und Non-Login-Shells sowie
interaktive und nicht-interaktive Shells [VGL](./Initialisieren.md)
• Im Terminal wird stets der aktuelle Pfad angegeben, in dem die Shell operiert, dabei steht die
Tilde ~ für das Home-Verzeichnis
• Beim Arbeiten mit Dateien kannst du absolute oder relative Pfadangaben verwenden:
absolute Pfadangaben gehen von einem übergeordneten Verzeichnis aus, beginnen mit mit /
und können sich auf sämtliche vorhandenen Dateien beziehen (also auch solche, die sich nicht
im aktuellen Verzeichnis befinden), während relative
 Pfade auf Dateien verweisen, die sich im
aktuellen Ordner befinden
• In der Umgebungsvariablen sind die Pfade zu den Programmen gespeichert, die du ausführen kannst. [Vgl](./Bash-ScriptingInANutshell.md)
• Indem man in eine Datei (ohne Endung) Terminal-Befehle schreibt, kann man Shell-Skripte
erstellen, die dann auch im Terminal ausgeführt werden kann; diese Shell-Skripte müssen als
erste Zeile eine sogenannte Shebang-Zeile enthalten, in der mitgeteilt wird, mit welchem
Programm dieses Skript ausgeführt werden soll, für Bash-Skripts benutzt du:

>#!/<Ordner>/bash

• Beachte, dass Programme unter Linux standardmäßig nicht ausgeführt werden dürfen und du sie erst freigeben musst
• Du kannst eine Datei manuell wie folgt zum Ausführen freigeben: in der grafischen
Benutzeroberfläche auf den Ordner rechtsklicken -> Properties/Eigenschaften ->
Permissions/Zugriffsrechte -> Allow executing file as program/Datei als Programm ausführen // in der CII nutze den Command **chmod**
• Um ein Programm ohne Pfadangabe ausführen zu können, musst du den Pfad in der
Umgebungsvariablen ergänzen
• Für permanente Anpassungen der Umgebungsvariablen musst du die bashrc – Datei editieren
und dort den Befehl für die Erweiterung der Umgebungsvariablen ergänzen; diese Datei ist
verborgen und du musst sie erst sichtbar machen
• Du erkennst verborgene Dateien in Linux daran, dass ihre Namen mit einem Punkt beginnen,
z.B. .bashrc

 [Vgl](./Bash-ScriptingInANutshell.md)