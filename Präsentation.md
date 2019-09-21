% BackupParty  
% keine Angst vor Datenverlust

# Agenda
* Warum Backups?
* Welche Arten von Backups gibt es?
* Wohin mit der Sicherung?
* Praxisteil
    * KeePassXC
    * Duplicati
    * Syncthing

# Warum Backups?
* Gegen welche Fehler kann ein Backup helfen?

# Warum Backups?
* Gegen welche Fehler kann ein Backup helfen?
    * Benutzungsfehler
    * Hardware-Defekt
    * Software-Defekt
    * Diebstahl
    * Feuer (oder andere Katastrophen)

# Welche Arten von Backups gibt es?
* **Kopie wichtiger Dateien oder Verzeichnisse**
* Kopie aller Dateisysteminhalte
* Datenträgerkopie (Image-Backup)

# Kopie wichtiger Datein oder Verzeichnisse
* Passwörter
* Bilder
* Dokumente
* Einstellungen
* ...

# Wohin mit der Sicherung?
1. ~~Backup Verzeichnis~~
2. ~~Backup Partition~~
3. ~~zweite Festplatte~~
4. externe Festplatte / NAS
5. anderes Gebäude / Cloud
6. Bankschließfach

# Praxisteil
* [Passwort-Manager KeePassXC](https://keepassxc.org/download)
* [Backup-Programm Duplicati](https://www.duplicati.com/download)
* [Datei-Synchronisation Syncthing (optional)](https://syncthing.net/)

|                        **Haftungsausschluss**                        |
|:--------------------------------------------------------------------:|
|Wir übernehmen keinerlei Haftung für Datenverlust, Geräteschäden, etc.|
|Ein Backup ist erst dann komplett, wenn auch die Wiederherstellung geprüft ist.|

# KeePassXC
* KeePassXC ist ein quelloffener Passwort-Manager, der für alle gängigen Desktop-Systeme angeboten wird.  
Passwort-Manager verwaltet die verschiedenen Passwörter in einer verschlüsselten Datenbank. Über ein Master-Passwort wird der Zugang zu dieser Datenbank geschützt.
* Diceware - sicheres Master Passwort finden
* Installation <[keepassxc.org/download](https://keepassxc.org/download/)>
* Auto-Type Einstellungen: `Strg+Alt+A`
* neue Datenbank anlegen
* neuen Eintrag anlegen

# Duplicati 1/3
* Duplicati ist eine freie Software zum Erstellen von Datensicherungen, die sowohl auf internen und externen Datenträgern (z.B. Festplatten, USB-Sticks) als auch auf Netzwerklaufwerken und bei Onlinespeicherdiensten ("Cloud") abgelegt werden können. Es eignet besonders zur regelmäßigen Sicherung von bestimmten Verzeichnissen und Dateien. Die Sicherungen werden grundsätzlich inkrementell angelegt und verschlüsselt.
* Installation <[duplicati.com/download](https://www.duplicati.com/download)>
* Einstellungen  
  Duplicati sendet standardmäßig einige Nutzungsdaten an die Entwickler und macht diese teilweise öffentlich verfügbar. Falls ihr dies nicht möchtet, solltet ihr im Hauptmenü unter dem Menüpunkt "Einstellungen" nach dem Stichwort "Nutzungsstatistiken" suchen und die Sammelei über das Dropdown-Menü und mit einem Klick auf "OK" unterbinden.

# Duplicati 2/3
* neue Sicherung hinzufügen
    1. "Name" für das Backup festlegen und optional eine  
        "Passphrase" vergeben (bei Online-Diensten dringend empfohlen)
    2. "Sicherungsziel" festlegen
    3. "Quell-Daten" festlegen  
        eventuell durch "Filter" Dateien "Ausschließen"
    4. "Zeitplan" festlegen
    5. "Sicherungs-Aufbewahrung" festlegen
* Sicherung ausführen

# Duplicati 3/3
* Sicherung wiederherstellen  
  Direkte Wiederherstellung von Sicherungsdateien
    1. "Sicherungsort" angeben
    2. "Passphrase" eingeben falls erforderlich
    3. Dateien und Zeitpunkt auswählen
    4. "Wiederherstellungsoptionen" wählen
        * Speicherort
        * Überschreiben?
        * Berechtigungen

# Syncthing 1/2
* Syncthing ist eine quelloffen geschriebene Dateisynchronisation mit Peer-to-Peer-Übertragungen. Es kann Dateien zwischen Geräten in einem lokalen Netzwerk oder zwischen entfernten Geräten über das Internet synchronisieren. Datenschutz und Datensicherheit sind zentraler Bestandteil der Software.
* Installation <[syncthing.net](https://syncthing.net/)>
* Einstellungen  
  Syncthing sendet standardmäßig einige Nutzungsdaten an die Entwickler und macht diese teilweise öffentlich verfügbar. Falls ihr dies nicht möchtet, solltet ihr über Aktionen unter dem Menüpunkt "Einstellungen" nach dem Stichwort "Nutzungsstatistiken" suchen und die Sammelei über das Dropdown-Menü und mit einem Klick auf "speichern" unterbinden.

# Syncthing 2/2
* Ordner Hinzufügen
    * Ordnerbezeichnung festlegen
    * Ordnerpfad auswählen
    * ggf. weitere Optionen festlegen
* Gerät hinzufügen
* Ordner teilen

# Links
* KeePassXC
    * [keepassxc.org](https://keepassxc.org)
    * [kuketz-blog.de/sicheres-passwort-waehlen-der-zufall-entscheidet/](https://www.kuketz-blog.de/sicheres-passwort-waehlen-der-zufall-entscheidet/)
    * [world.std.com/~reinhold/Diceware_German.pdf](http://world.std.com/~reinhold/Diceware_German.pdf)
* Duplicati
    * [duplicati.com](https://www.duplicati.com)
    * [digitalcourage.de/hochschulgruppe-bielefeld](https://digitalcourage.de/hochschulgruppe-bielefeld)
* Syncthing
    * [syncthing.net](https://syncthing.net/)

# Unterlagen
* Die Unterlagen zu diesem Workshop sind auf unserer GitLab Instanz unter der CC by-sa Lizenz veröffentlicht.  
[git.makerspace-gt.de/makerspace-gt-workshops/BackupParty](https://git.makerspace-gt.de/makerspace-gt/workshops/BackupParty)
* Wir freuen uns über Hinweise, Verbesserungen und Wiederverwendung!