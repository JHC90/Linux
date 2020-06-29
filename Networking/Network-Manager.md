<h1>Networkmanager - GUI</h1>

Hier konfigurieren wir die IP-Adressen mit einer GUI und anschließend auf der CLI.

# GUI

## IPv4
![](imgs/2020-06-26-14-56-41.png)
hier kann entweder via Automatisch/DHCP oder statisch (=Manuell) hinterelegen. 


mehrer redundaten DNS-Server
die werden mit einem Komma getrennt
![](imgs/2020-06-26-14-57-49.png)

## IPv6
**Reaktivierung**
nach einer Änderung muss die Schnittstelle reaktiviert werden. Reaktivieren = einmal an und wieder ausschalten:
![](imgs/2020-06-26-15-03-32.png)

# CLI
hier gibt es unterschiedliche Ansätze. Im großen und ganzen gibt es die Datei 
```/etc/network/interfaces```

für jede ProtokollVersion (IPv4 oder IPv6) muss eine eigene Konfig erstellt werden

## IPv4