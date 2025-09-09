# Git-Spickzettel: Typischer Git-Workflow im Terminal

Dieser Spickzettel zeigt die wichtigsten Git-Befehle im Terminal mit kurzen Erklärungen. Ideal für Einsteiger und als Nachschlagewerk.


## 1. Status prüfen

git status

## 2. Änderungen stagen (z. B. alle Dateien)

<<<<<<< HEAD
git add 'Datei Name'.
=======
git add "Datei Name".
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git

## 3. Commit erstellen

git commit -m "Meine Änderungen, freier Textbaustein"

## 4. Neueste Änderungen vom Remote holen

<<<<<<< HEAD
git pull origin 'branch-name'
=======
git pull origin "branch-name"
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git

## 5. Änderungen hochladen

<<<<<<< HEAD
git push origin 'branch-name'
=======
git push origin "branch-name"
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git

## 6. Branches anzeigen

git branch "branch-name"

## 7. Zu einem bestehenden Branch wechseln:

<<<<<<< HEAD
git checkout 'branch-name'
=======
git checkout "branch-name"
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git

## 8. Neuen Branch erstellen

<<<<<<< HEAD
git branch 'branch-name'
=======
git branch "branch-name"
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git


# Aenderung von 'branch-name' in main mergen

## 1. Zum Ziel wechseln

git checkout main

## 2. Neuste Änderungen vom Remote holen (optional aber empfohlen)

git pull origin main

## 3. Merge ausführen

git merge "branch-name>

## 4. Nach erfolgreichem Merge → Push zu Remote

git push origin main

## Beispiel (kompakt):

- git checkout main
- git pull origin main
<<<<<<< HEAD
- git merge aufgabe
- git push origin main

=======
- git merge "branch-name"
- git push origin main
>>>>>>> branch 'aufgabenExercise' of https://github.com/JovoVidic/hs-25-swe2-exercises.git

## Nur der test der Datei
