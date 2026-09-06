Project: Twitch_SlipStream

Twitch_SlipStream (vaft) ist ein hochentwickeltes Userscript zur automatischen 
und lautlosen Blockierung von Twitch-Videowerbung (Prerolls & Midrolls).

---------------------------------------------------------------------------------------------------

    Beschreibung:
      Das Skript basiert auf der revolutionären backupSwapFirst-Logik. 
      Sobald Twitch eine Werbewelle startet, fängt das Skript die Playlist-Anfrage 
      ab und schaltet im Hintergrund blitzschnell auf alternative, 
      werbefreie Datenpipelines um (z. B. offizielle mobile Streams oder Popout-Pipelines). 
      Falls die hochauflösenden Kanäle temporär komplett überlastet oder ad-verseucht sind, 
      greift das Skript auf eine automatische 360p-Drosselung zurück, 
      um den Stream am Leben zu erhalten, 
      und schaltet nach dem Werbeblock unsichtbar wieder auf 1080p bei 60 FPS hoch.
---------------------------------------------------------------------------------------------------

    Features: 
        🚀 backupSwapFirst-Technologie: 
      - Kein lokales Herausschneiden im Video-Player nötig – verhindert Ladekreise und Player-Abstürze.
      
      🖥️ Nested-Frame-Filter:
      - Klinkt sich nur in das primäre Video-Element ein und ignoriert versteckte 
        Twitch-Hintergrund-Frames (schont CPU & RAM auf Multi-Monitor-Setups).
        
      🔒 Anti-A/V-Desync-Schutz:
      - Automatischer Soft-Reload und Audio-Click-Mute bei harten Stream-Wechseln.
      
      📱 iOS-optimiert:
      - Angepasste Parameter verhindern die berüchtigten Safari-Dauerschleifen.
---------------------------------------------------------------------------------------------------

Installationsanleitung (Desktop / Google Chrome):
---------------------------------------------------------------------------------------------------
  - Für die Nutzung auf dem Desktop unter Google Chrome wird ein Userscript-Manager benötigt. 
    Wir empfehlen Tampermonkey oder Violentmonkey.
---------------------------------------------------------------------------------------------------
    Variante A: Installation via Tampermonkey:
    
    1. Erweiterung installieren: 
    Öffne den Chrome Web Store und installiere Tampermonkey für Google Chrome.
    
    2. Neues Skript erstellen: 
    Klicke auf das Tampermonkey-Icon in deiner Browser-Leiste und wähle "Neues Skript erstellen".
    
    3. Code einfügen: 
    Lösche den gesamten Standardtext im Editorfenster komplett.
    Kopiere den vollständigen Quellcode des Twitch_SlipStream Skripts und füge ihn in den leeren Editor ein.
    
    4. Speichern: 
    Drücke die Tastenkombination Strg + S (Windows) bzw. Cmd + S (Mac) 
    oder klicke oben links auf Datei ➔ Speichern.
    
    5. Twitch starten: 
    Öffne Twitch.tv oder lade einen aktiven Stream neu.
---------------------------------------------------------------------------------------------------

    Variante B: Installation via Violentmonkey:
    
    1. Erweiterung installieren: 
    Öffne den Chrome Web Store und installiere Violentmonkey für Google Chrome.
    
    2. Neues Skript erstellen: 
    Klicke auf das Violentmonkey-Icon und wähle das "+"-Symbol ➔ "Neues Skript".
    
    3. Code einfügen: 
    Ersetze den vorhandenen Vorlagentext im Editorfenster vollständig mit dem Twitch_SlipStream - Quellcode.
    
    4. Speichern: 
    Klicke oben rechts im Editor auf das Disketten-Symbol ("Speichern & Schließen").
---------------------------------------------------------------------------------------------------


Schritt-für-Schritt-Anleitung für iOS (Safari) mit Tampermonkey: 
---------------------------------------------------------------------------------------------------
  - Da Apple im normalen Safari-Browser die tiefe Manipulation von Video-Netzwerk-Workern stark einschränkt,
  ist die Nutzung der offiziellen Tampermonkey-App auf dem iPhone der stabilste Weg,
  um Streams ohne Dauerschleifen werbefrei zu halten.
---------------------------------------------------------------------------------------------------

    Schritt 1: Die Tampermonkey-App laden und vorbereiten
    1. Öffne den App Store auf deinem iPhone oder iPad.
    2. Suche nach „Tampermonkey“ (von Jan Biniok) und installiere die App.
    3. Öffne die Tampermonkey-App auf deinem Gerät. Du siehst nun ein Interface,
       das wie ein eigener Webbrowser aufgebaut ist.

---------------------------------------------------------------------------------------------------

    Schritt 2: Das Twitch_SlipStream - Skript hinzufügen
    1. Tippe in der App unten oder oben auf das Zahnrad-Symbol, um in das Dashboard zu gelangen.
    2. Wechsel auf den Reiter „Übersicht“ (oder Installed Scripts).
    3. Tippe oben rechts auf das „+“ (Plus-Symbol), um ein neues, leeres Skript zu erstellen.
    4. Lösche den automatisch generierten Beispiel-Text im Editor-Fenster komplett heraus, sodass das Feld absolut leer ist.
    5. Kopiere den vollständigen, deutschen Twitch_SlipStream - Quellcode (v68.5.7) in deiner Zwischenablage.
    6. Füge den gesamten Code in das leere Editor-Feld der App ein.
    7. Tippe oben links im Editor-Menü auf „Datei“ (bzw. das Disketten-Symbol).
    8. Wähle „Speichern“ aus.
    9. In deiner Übersicht wird das Skript nun als aktiv mit dem Namen Twitch_SlipStream gelistet.
   
---------------------------------------------------------------------------------------------------
    Schritt 3: Twitch in Safari öffnen und genießen
    1. Der Live-Check: Sobald eine Werbewelle rollt, klinkt sich die App ein. 
       Oben links im Videobild ploppt sofort ein Banner auf. Z.b. mit der Meldung 
       "Blocking midroll ads (autoplay)"  
---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------


Schritt-für-Schritt-Anleitung für iOS (Safari) mit Userscripts:
---------------------------------------------------------------------------------------------------
  - Da Apple den Zugriff auf tiefgreifende Browser-Erweiterungen unter iOS einschränkt, 
  nutzen wir die offizielle Safari-Erweiterung Userscripts (Open-Source), 
  um das Skript flugsicher über die iCloud auf deinem iPhone oder iPad auszuführen.
---------------------------------------------------------------------------------------------------

    Schritt 1: Die "Userscripts"-App installieren
    1. Öffne den App Store auf deinem iPhone/iPad.
    2. Suche nach der App "Userscripts" (Entwickler: Justin Wasack) und installiere sie.

---------------------------------------------------------------------------------------------------

    Schritt 2: Die Erweiterung in Safari aktivieren
    1. Öffne die Einstellungen (graues Zahnrad) deines iPhones.
    2. Scrolle nach unten und tippe auf den Menüpunkt Safari.
    3. Tippe unter der Kategorie Allgemein auf Erweiterungen.
    4. Wähle in der Liste Userscripts aus und lege den Schalter auf Ein (Grün).
    5. Tippe direkt darunter unter Berechtigungen für alle Websites auf Zulassen, 
       damit das Skript die Twitch-Datenströme untersuchen darf.

---------------------------------------------------------------------------------------------------

    Schritt 3: Den Skript-Ordner in der iCloud festlegen
    1. Öffne die installierte Userscripts-App direkt auf deinem iPhone-Bildschirm.
    2. Die App bittet dich, einen Arbeitsordner auszuwählen. Tippe auf "Set User Scripts Directory".
    3. Wähle einen Ordner in deiner iCloud Drive oder lokal auf dem iPhone (z. B. einen neu erstellten Ordner namens "Userscripts"). 
       Dieser Ordner dient als Verzeichnis, in dem deine Skripte liegen.

---------------------------------------------------------------------------------------------------

    Schritt 4: Das Twitch_SlipStream - Skript einspielen
    1. Erstelle auf deinem PC/Mac eine normale Textdatei, 
       füge den Twitch_SlipStream - Quellcode ein und benenne die Datei um in Twitch_SlipStream.user.js 
       (wichtig ist die Endung .user.js).
    2. Verschiebe diese Datei auf deinem Mac oder PC in den exakt selben iCloud-Ordner, 
       den du in Schritt 3 auf dem iPhone ausgewählt hast. 
    
    (Alternativ kannst du den Code auf dem iPhone kopieren, die "Dateien"-App öffnen,
    in dem Ordner eine Textdatei erstellen und den Code dort einfügen).

---------------------------------------------------------------------------------------------------

    Schritt 5: Funktionsprüfung auf dem iPhone
    1. Öffne Safari auf deinem iPhone und gehe auf twitch.tv.
    2. Tippe in der Adressleiste links auf das Erweiterungen-Symbol (das Puzzleteil- oder "Aa"-Symbol).
    3. Klicke auf Userscripts. Du siehst nun ein kleines Menü, 
       in dem das Skript Twitch_SlipStream aufgelistet ist.
    4. Stelle sicher, dass das Skript per Häkchen aktiviert ist. Sobald du einen Stream startest, 
       blockiert die Safari-Engine die Werbesegmente lautlos im Hintergrund.

---------------------------------------------------------------------------------------------------














