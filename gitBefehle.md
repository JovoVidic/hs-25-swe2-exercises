# Git-Spickzettel: Typischer Git-Workflow im Terminal

Dieser Spickzettel zeigt die wichtigsten Git-Befehle im Terminal mit kurzen Erklärungen. Ideal für Einsteiger und als Nachschlagewerk.


## 1. Status prüfen

git status

## 2. Änderungen stagen (z. B. alle Dateien)

git add <Datei Name>.

## 3. Commit erstellen

git commit -m "Meine Änderungen, freier Textbaustein"

## 4. Neueste Änderungen vom Remote holen

git pull origin <branch-name>

## 5. Änderungen hochladen

git push origin <branch-name>

## 6. Branches anzeigen

git branch <branch-name>

## 7. Zu einem bestehenden Branch wechseln:

git checkout <branch-name>

## 8. Neuen Branch erstellen

git branch <branch-name>


# Aenderung von 'branch-name' in main mergen

## 1. Zum Ziel wechseln

git checkout main

## 2. Neuste Änderungen vom Remote holen (optional aber empfohlen)

git pull origin main

## 3. Merge ausführen

git merge <branch-name>

## 4. Nach erfolgreichem Merge → Push zu Remote

git push origin main

## Beispiel (kompakt):

- git checkout main
- git pull origin main
- git merge 'branch-name'
- git push origin main
