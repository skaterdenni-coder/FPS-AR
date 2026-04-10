Abwandlung der AR-Demo von:edoardomignano  Link: https://github.com/edoardomignano/ar-demo
diese version wurde um einen Datenupload und Sharing Funktion erweitert. 


🚀 AR Model Viewer
Ein leichtgewichtiger, webbasierter 3D-Modell-Viewer mit Augmented Reality (AR) Unterstützung. Lade deine .glb-Dateien hoch, betrachte sie im Browser und teile sie per Link mit anderen.

✨ Features
3D Viewer: Interaktive Ansicht von Modellen (Rotation, Zoom, Fullscreen).

AR-Modus: Betrachte Modelle in deiner echten Umgebung (unterstützt WebXR, Scene-Viewer und Quick-Look).

Cloud-Upload: Automatischer Upload zu Litterbox (Catbox). Erzeugt einen teilbaren Link, der 24 Stunden gültig ist.

Mobile Ready: Optimiert für Smartphones und Tablets.

Deep Linking: Parameter-Unterstützung (?model=URL), um Modelle direkt über die URL zu laden.

🛠️ Technologien
Frontend: HTML5, CSS3, JavaScript (ES6+).

3D Rendering: Google Model-Viewer.

Hosting/API: Litterbox für temporäres Asset-Hosting.

🚀 Installation & Nutzung
Da es sich um eine reine Client-seitige HTML-Datei handelt, ist keine Installation notwendig:

Klone das Repository:

Bash
git clone https://github.com/DEIN-BENUTZERNAME/ar-model-viewer.git
Öffne die index.html in einem modernen Webbrowser.

Wichtig: Für die AR-Funktionen muss die Seite über HTTPS aufgerufen werden (z. B. via GitHub Pages).

📖 Bedienung
Modell wählen: Ziehe eine .glb-Datei in das Upload-Feld oder klicke darauf.

Warten: Das Modell wird hochgeladen und im Viewer initialisiert.

Teilen: Kopiere den generierten Link unter dem Viewer, um ihn an Freunde oder Kollegen zu senden.

AR: Klicke auf dem Smartphone auf "AR starten", um das Modell in den Raum zu projizieren.

⚠️ Einschränkungen
Dateityp: Aktuell werden nur .glb (GLTF Binary) Dateien unterstützt.

Gültigkeit: Da Litterbox genutzt wird, werden hochgeladene Dateien nach 24 Stunden automatisch gelöscht.

Browser-Support: AR-Funktionen erfordern Chrome (Android) oder Safari (iOS mit Quick Look Support).
