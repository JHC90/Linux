# Quotas

Quota = Effiziente Nutzung von Festplattenspeicher indem man jedem User maximalen Speicher zuweist und damit performt

[Ergänzung zu User und Gruppen](./UserAndGroupManagement.md)
[Theorie zu Quotas]()
**Erstellt Quota für User**
>quotacheck –c -u /Verzeichnis

**Erstellt Quota für Gruppe**
>quotacheck –c -g /Verzeichnis 

**Quota aktivieren**
>quotaon /dev/sdb1 

**Quota deaktivieren**
>quotaoff /dev/sdb1 

**Konfiguration von Quotas für Benutzer**
>edquota –u Benutzer 

**Konfiguration von Quotas für Gruppe**
>edquota –g Gruppe 