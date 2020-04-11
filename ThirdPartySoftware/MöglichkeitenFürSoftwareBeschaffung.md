# Möglichkeiten der Softwarebeschaffung

In Ubuntu gibt es mehrere Möglichkeiten Software zu beschaffen. Nachdem jedes Tutorial(egal zu welchem Thema) gefühlt einen anderen Weg der Softwarebeschaffung wählt, gehe ich hier lediglich auf die Möglichkeiten ein, wie Software beschafft werden kann. Diese "Beschaffungstutorial" basiert auf folgenden Tutorials:
**Basic-Tutorial**
Das [Basic-Tutorial](https://www.ubuntupit.com/how-to-install-software-in-ubuntu-linux-a-complete-guide-for-newbie/) liefert zahlreiche Beschaffungsmöglichkeiten und deren Erklärung

# GUI
   ## Software Center
   ## DEB-Files

# CLI
## apt-Commands / apt-get install *
## dpkg / *.deb-files

   Im Grunde wird hierbeit die Datei heruntergeladen, entpackt und dann installiert. Das ganze soll mit SU-Rechten gemacht werden. Ergo braucht man hierfür auch kein repo, die Adresse erhält man einfach durch das browsen. 
   Der Name dpkg ist eine Abkürzung für Debian Package. Das Debian-Software-Paket-Format wurde im Debian-Projekt entwickelt, allerdings wird dieses Paketformat und das Paketverwaltungsprogramm dpkg auch von anderen Software-Distributionen verwendet.
    1.  Hier wird zunächst ein File heruntergeladen. Bspw via wget (bsp-Command: "wget --content-disposition https://packages.gitlab.com/gitlab/gitlab-ce/packages/debian/buster/gitlab-ce_12.9.2-ce.0_amd64.deb/download.deb")
    2. Navigation zu dem File:
   
    
    cd "Dahin wo man das File hingeladen hat"
    
Installation des Files

    sudo dpkg -i gitlab-ce_12.9.2-ce.0_amd64.deb/download.deb

Aufösen der Depencies

    sudo apt-get install -f

Packet entfernen

    dpkg -r 'paketname'

Packete auflisten

    dpkg -l
    

## Flatpak
## Snap Packages
## AppImage
## PPA
## Package Manager
##  Source Code
##  Web Browser
##  pip