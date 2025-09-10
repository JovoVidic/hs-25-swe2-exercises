# Beispiel: Neuer Branch Vxy, Änderungen machen, committen und pushen

## Schritt 1: Repository klonen (einmalig)

`git clone https://github.com/dein-benutzername/dein-projekt.git` <br>
cd dein-projekt

## Schritt 2: Neuen Branch Vxy erstellen und wechseln

`git checkout -b Vxy`

- Du bist jetzt im Branch Vxy.
- Git zeigt dir die Dateien im Arbeitsverzeichnis (deinem Projektordner) an.

## Schritt 3: Dateien ändern

- Öffne z. B. src/Main.java und füge eine Zeile hinzu.
- Ändere z. B. auch README.md.
- README.md Datei immer aktualisieren, z.B. mit dem Aenderungsdatum.

## Schritt 4: Änderungen zum Commit vormerken (Staging Area)

`git add src/Main.java README.md`

- Jetzt sind diese Dateien für den nächsten Commit vorgemerkt.
- Du kannst auch alle Änderungen auf einmal vormerken mit:

`git add .`

## Schritt 5: Commit machen (Snapshot mit Kommentar)

`git commit -m "Feature Vxy: Neue Funktion in Main.java und README aktualisiert"`
- Du hast jetzt einen lokalen Commit.
- Git speichert den Zustand dieser Dateien in deinem lokalen .git-Ordner.
- Die Dateien sind immer noch physisch auf deiner Festplatte.

## Schritt 6: Branch Vxy mit den Änderungen zum Remote-Repository pushen
`git push origin Vxy`
- Dein Branch Vxy mit den Änderungen ist jetzt auf dem zentralen Server (GitHub/GitLab/etc.).
- main bleibt davon unberührt.

## Schritt 7 (Optional): Änderungen aus Branch `Vxy` in `main` mergen

Nachdem du deine Änderungen im Branch `Vxy` erfolgreich gepusht hast, kannst du sie in den `main`-Branch übernehmen. <br>
<br>
Dafür gibt es zwei Möglichkeiten:

### 🔁 Möglichkeit A: Merge lokal durchführen und pushen

Führe den Merge auf deinem lokalen Rechner aus und lade die aktualisierte `main`-Version ins Remote-Repository hoch.


1. Zurück zum main-Branch wechseln <br>
`git checkout main`

2. Aktuelle Version von main vom Server holen <br>
`git pull origin main`

3. Branch Vxy in main mergen <br>
`git merge Vxy`

4. Aktualisierten main-Branch pushen <br>
`git push origin main`