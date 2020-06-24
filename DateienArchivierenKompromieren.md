# Archivieren

• Um Daten und Dateien sichern oder bereit zu stellen, bietet es sich an, diese in einer
Archivdatei als Ganzes einzupacken und zu komprimieren
• Spart Platz auf dem Speichermedium bzw. Bandbreite bei der Übertragung
• Das am häufigsten verwendete Programm zum Archivieren ist tar
• Dateien mit der Endung tar sind unkomprimierte Archive die mit tar -xf entpackt werden
können. Nach dem Entpacken bleibt die Archiv-datei weiterhin vorhanden
• Archive beinhalten meistens mehrere Dateien und oft auch Verzeichnisse. Diese können mit
tar -tf angezeigt werden
• Mehrere Dateien und Verzeichnisse können mit tar -cf zu einem Archiv zusammengefasst
werden
• Alternative zu tar ist cpio



# Komprimieren
• Bzip2(.bz2) und gzip(.gz) sind Kompressionsverfahren
• Bzip2 ist die neuere und effektivere Variante

• Alternative zu gzip und bzip2 ist xz

**Tarball**
• Ein Tarball ist eine mit tar erstellte und gzip oder bzip2 komprimierte Archivdatei