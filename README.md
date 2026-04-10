🚀 AR Model Viewer (Extreme Performance Edition)
Eine erweiterte Version der AR-Demo von edoardomignano. Diese Fassung wurde um ein leistungsstarkes Cloud-Hosting, eine Sharing-Funktion und ein Echtzeit-Performance-Monitoring ergänzt.

✨ Features
3D Viewer: Interaktive Ansicht von Modellen (Rotation, Zoom, Fullscreen).

AR-Modus: Native AR-Projektion via WebXR, Scene-Viewer (Android) und Quick-Look (iOS).

Performance Monitoring (Neu): Integrierter FPS-Zähler und Frametime-Analyse via Stats.js.

Uncapped Rendering: Optimierter Loop für maximale GPU-Auslastung jenseits der 60-FPS-Grenze (Benchmarking-ready).

GPU-Detection: Automatische Erkennung und Anzeige der aktiven Grafikeinheit.

Cloud-Upload: Automatischer Upload zu Litterbox (Catbox) mit 24-Stunden-Gültigkeit.

Deep Linking: Sofortiges Laden von Modellen über URL-Parameter (?model=URL).

🛠️ Technologien
3D Engine: Google Model-Viewer

Performance Tracking: Stats.js

Backend API: Litterbox (Temporäres Asset-Hosting)

Frontend: HTML5, CSS3, JavaScript (ES6+)

🚀 Installation & Nutzung
Da die Anwendung rein Client-seitig läuft, ist kein Server-Setup erforderlich:

Klone das Repository:

Bash
git clone https://github.com/DEIN-BENUTZERNAME/ar-model-viewer.git
Lokal testen: Öffne die index.html in einem modernen Browser.

Deployment: Für AR-Funktionen muss die Seite über HTTPS bereitgestellt werden (empfohlen: GitHub Pages).

📊 Performance & Benchmarking
Diese Version ist darauf ausgelegt, das Maximum aus deiner Hardware zu holen:

FPS Anzeige: Oben links siehst du die aktuellen Bilder pro Sekunde.

GPU Info: Oben rechts wird der Renderer (z. B. NVIDIA RTX oder Intel Iris) angezeigt.

Uncapped Mode: Der interne Loop nutzt setTimeout(..., 0) anstelle von requestAnimationFrame, um die GPU-Zyklen unabhängig von der Monitor-Bildwiederholfrequenz zu messen.

Tipp: Um die 60-FPS-Sperre des Browsers komplett aufzuheben, starte Chrome mit dem Flag --disable-frame-rate-limit.

📖 Bedienung
Modell wählen: Lade eine .glb-Datei per Klick oder Drag & Drop hoch.

Upload & Share: Sobald das Modell geladen ist, wird ein Sharing-Link und ein QR-Code generiert.

AR starten: Scanne den QR-Code mit einem Smartphone, um das Modell in deiner Umgebung zu platzieren.

⚠️ Einschränkungen & Hinweise
Dateiformat: Nur .glb (GLTF Binary) wird unterstützt.

Speicherdauer: Uploads werden nach 24 Stunden vom Hoster (Litterbox) gelöscht.

V-Sync: Viele Browser deckeln die Anzeige standardmäßig bei 60 FPS, um Energie zu sparen. Die tatsächliche Rechenleistung der GPU kann im Uncapped-Mode jedoch höher liegen.
