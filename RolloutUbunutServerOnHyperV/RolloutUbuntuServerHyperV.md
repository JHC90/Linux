# Rollout Probleme
leider klappt der Rollout von Ubuntu Server häufig nicht auf dem Windows hyperv, da eine Konfig anders sein muss

hier mein Workaround



Normales erstellen via Whizzard
Generation2 bei der auswahl der geneartion
als iso die Ubuntu server 19.04
4 kerne / 8192 Ram
vor dem ersten Booten der VM in die Einstellungen,

dort unter sicherheit


!!!! das hier ist die FALSCHE Auswahl im Dropdpwn: "Microsoft Windows" !!!!
!!!! das hier ist die Richtige Auswahl im Dropdpwn: "Microsoft UEFI-Zertifizerungsstelle" !!!!



und als Vorlage unbedingt auf "Microsoft UEFI-Zertifizerungsstelle" wechseln:

![picture](./img/Solution.PNG)





danach sollte der Boot normal klappen.

es kann noch im weiteren zu einem Traceback-Fehler kommen, den konnte ich noch nicht lösen. Ich hatte aber soweit meine Fragestellung hier geklärt. Den Traceback löse ich das nächste mal. 
Eine Mögliche Lösung wäre,dass das IMG-File nicht gleichzeitig in zwei Rechnern drin sein kann, da der hyperv1 (level1) das img file für den spezfischen rollout blockt. Ich versuchs mal mit nem reboot des hyperv-Servers.

