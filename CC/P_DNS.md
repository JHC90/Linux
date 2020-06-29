CheckDNS dig // in [Linux]()

1. welche DNS-Server werden in einer Datei gepflegt
   > cat /etc/resolv-conf7
   > nmcli

2. Auflösung von DNS 
   1. nslookup ist obsolet
   ![](imgs/2020-06-27-09-48-55.png)
   1. host
   
   > host www.google.com
   ![](imgs/2020-06-27-09-49-34.png)
   > host -t ns www.google.de 
   > host -t mx www.google.de 
   > host -t mx www.google.de  8.8.8.8 | Reverse von ip auf 
   ![](imgs/2020-06-27-09-51-43.png)

   1. dig
   >dig www.google.de

   ![](imgs/2020-06-27-09-53-12.png)

   > dig @8.8.8.8 google.de ns | Frage an Google DNS
   > dig @192.168.178.1 -x 8.8.8.8 | Frage lokalen DNS

   1. etc/hosts
   > ping localhost
   > /etc/hosts

   ![](imgs/2020-06-27-09-57-49.png)

   somit ist in der Host-Datei jetzt ein Eintrag hinterlegt. Somit kann hier gezielt eine Manuelle Host-Auflösung geschehe