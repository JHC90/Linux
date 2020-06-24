# Quotas

[PraxisQuotas](./Command-Container/Quotas.md), außerdem ist das eine Ergänzung zu den [User und Gruppenrichtlinien](./UserUndGruppen.md)

* Quotas ermöglichen die Speicherplatzbelegung für Benutzer und Gruppen zu begrenzen
* Wird auf Dateisysteme bzw. Partitionen angewendet
* Dadurch ist es möglich, dass die Benutzer ein bestimmtes Speicherkontingent für ihre
Homeverzeichnisse erhalten
* Wir unterscheiden in Softlimit und Hardlimit sowie eine Grace-Period, zu deutsch: Gnadenfrist
   * Wird das Softlimit von einem Benutzer überschritten, so darf dieser weiter Speicher
belegen bis zum Hardlimit
   * Das Hardlimit ist die definitive Grenze
   * Ist das Softlimit überschritten, läuft die Grace-Period an
* Während das Hardlimit obligatorisch ist, können wir das Softlimit auch weglassen
* Quotas sind per Default auf keiner normalen Distribution aktiv
* Unter Ubuntu installieren wir sie mit 
  >apt install quota 
  
  nach, unter CentOS mit 
  
  >yum install quota

* Zur Aktivierung, in der Datei /etc/fstab für das gewünschte Dateisystem usrquota für
Benutzerbegrenzungen und grpquota für Gruppenbegrenzungen ergänzen
* Quotas können für Benutzer und Gruppen konfiguriert werden (siehe [PraxisQuotas](./Command-Container/Quotas.md))