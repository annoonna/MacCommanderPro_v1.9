# MacCommanderPro_v1.9

MacCommander ist ein Tool zur Fernverwaltung von macOS-Systemen via SSH. Durch die Integration von macFUSE lassen sich entfernte Verzeichnisse direkt im Finder mounten und bearbeiten. Optimiert für die Zusammenarbeit mit FileServerPro_macOS, um nahtlose Workflows zwischen Mac-PCs zu ermöglichen. sudo python3 main.py 
1. macFUSE Berechtigungen (Kernel Extensions)
Auf modernen Macs (M1, M2, M3) lässt Apple Drittanbieter-Treiber standardmäßig nicht zu. Du musst sie manuell im Wiederherstellungsmodus freischalten:
Mac ausschalten.
Einschaltknopf gedrückt halten, bis „Loading startup options“ erscheint.
Auf Optionen klicken -> Weiter.
Oben im Menü: Dienstprogramme -> Startsicherheitsdienstprogramm.
Wähle deine Festplatte aus und klicke auf Sicherheitsrichtlinien.
Wähle Reduzierte Sicherheit und setze den Haken bei: „Verwaltung von Kernel-Erweiterungen von verifizierten Entwicklern durch Benutzer erlauben“.
Startet den Mac neu.
Gehe zu Systemeinstellungen -> Datenschutz & Sicherheit. Scrolle nach unten und klicke bei der Meldung „macFUSE wurde blockiert“ auf Zulassen. Ein erneuter Neustart ist erforderlich.
2. Starten über das Terminal
Da das Programm tiefgreifende Rechte benötigt, muss es aktuell mit Administratorrechten gestartet werden:

bash
sudo python3 main.py


(Du wirst nach deinem Mac-Passwort gefragt. Während der Eingabe erscheinen keine Zeichen – das ist normal.)

