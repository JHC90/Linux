# Autostart Optionen in Linux

## bashRc
Das ist user Spezfisch und somit logischerweise auch abhängig von der User-Anmeldung

 Die versteckte Datei „.bashrc“ liegt im Home-Verzeichnis jedes Benutzers und gilt folglich für den angemeldeten Benutzer. Alle dort enthaltenen Kommandos werden beim Start des Terminals abgearbeitet. Normalerweise dienen die „Bash Run Commands“ (bashrc) allein dem Terminal-Komfort mit Aliases, Functions, Prompt und Definitionen weiterer Variablen. Es ist auch sicher nicht praktikabel, jeden Terminal-Start mit diversen, eventuell sogar grafischen Programmen zu begleiten. 

 **BSP-Implementierung bashRc**<br>
 hiermit werden die Dateien als Pfadvaribalen jedes Mal bei der Anmeldung geladen<br>
>echo 'export PATH=$PATH:$HOME/.local/bin' >> ~/.bashrc

Neustarten der Bash
>source ~/.bashrc

---

##  rc.local
Befehle, die unabhängig vom angemeldeten Benutzer in jedem Fall abgearbeitet werden sollen, können Sie auf Debian-basierten Systemen (Debian, Ubuntu, Mint, Raspbian) in der Datei „/etc/rc.local“ unterbringen. Diese Befehle werden schon vor der Benutzeranmeldung ausgeführt. Nur Abmelden und nachfolgendes Neuanmelden löst daher die „rc.local“ nicht aus. Um die Datei zu bearbeiten, benötigen Sie root-Recht: 

 **BSP-Implementierung rc.local**<br>

 >sudo gedit /etc/rc.local

 airflow webserver --daemon && airflow scheduler --daemon<br>

**BSP:**
1. 

 ---