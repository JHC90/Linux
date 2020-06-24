# Public-Ip

**keywords**
*Public Ip, G-Drive auf CLI, delte in gdrive, upload in gdrive*



Dieses Skript wird auf einem Rapsberry-Pi ausgeführt und speichert mir nach einer zeitlichen Terminierung in den Cronjobs immer die aktuelle Public-Ip in einen entsprechenden Remote Folder.

```
cd /home/pi
dig @ns1-1.akamaitech.net ANY whoami.akamai.net > /home/pi/test.txt

# Download
# /home/pi/./gdrive-linux-rpi download 1gJqNupSowLDNm9iJkOYjJ1GUNkX95epF


# Delete all Files in Directory
# Verified : /home/pi/./gdrive-linux-rpi list --query "'1jHb5IrBNhuFO5t2UfG8XJGWqf8slO1B0' in parents" # => listet alle files in einem Remote-Directory
/home/pi/./gdrive-linux-rpi list --query "'1jHb5IrBNhuFO5t2UfG8XJGWqf8slO1B0' in parents" --no-header --max 0 | cut -d" " -f1 - | xargs -L 1 /home/pi/./gdrive-linux-r$

# Upload in Parentfolder
/home/pi/./gdrive-linux-rpi upload /home/pi/test.txt --parent 1jHb5IrBNhuFO5t2UfG8XJGWqf8slO1B0

```