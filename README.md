# Aufgaben-App (APK)

Datum/Uhrzeit, Wetter Schwerin, Nachrichten-Laufband, Tagesspruch und Aufgabenliste.

## APK bauen (ohne Android Studio, nur mit GitHub)

1. Auf github.com ein neues, leeres Repository anlegen (z. B. "aufgaben-app").
2. Den Inhalt dieses Ordners hochladen ("Add file" > "Upload files"). Wichtig: auch den versteckten Ordner `.github` mit hochladen (am einfachsten den entpackten Ordnerinhalt per Drag & Drop auf die Seite ziehen).
3. Im Repository auf "Actions" gehen. Der Workflow "APK bauen" startet automatisch (oder über "Run workflow").
4. Nach ca. 3-5 Minuten den fertigen Lauf öffnen, unten unter "Artifacts" `aufgaben-apk` herunterladen und das ZIP entpacken.
5. `app-debug.apk` aufs Handy kopieren, antippen und installieren (ggf. "Installation aus unbekannten Quellen" für den Dateimanager erlauben).

## Alternativ lokal (Android Studio)

    npm install
    npx cap add android
    npx cap sync android
    npx cap open android

Dann in Android Studio: Build > Build APK(s).

## Anpassen

Alles steckt in `www/index.html`. Nach Änderungen die APK neu bauen.
