# Installation des Projekts

## 1. Fork erstellen und klonen

Um einen Fork zu erstellen muss man folgende Schritte beachten:

1. In das Repository gehen, welches man forken will. 

2. In der oberen rechten Ecke der Seite auf Forken klicken. 

3. In dem Fenster wählt man den Besitzer und gibt dem Fork einen beliebigen Namen. Bei gelengenheit kann man auch eine Beschreibung einfügen. 

4. Sobald du alles ausgefüllt hast das du brauchst, kannst du auf den grünnen Knopf unten rechts gehen mit der Beschriftung "Create fork". Dann bist du ach schon fertig. 

Um einen Fork zu klonen befolgen sie folgende Schritte: 

1. Navigiere zu deinem Fork. 

2. Klicke oberhalb der Liste der Dateien auf "<> Code". 

3. Kopiere die URL für das Repository. 

- Wähle dann über welche URL du es klonen möchtest (HTTPS/ SHH/ GitHub CLI). Beachte das du beim SHH einen SSH-Schlüssel benötigst. Kopiere die URL mit der Grafik rechts neben dem Code. 

4. Öffne Git Bash. 

5. Ändere dein aktuelles verzeichnis an einen Ort an dem du das geklonte Verzeichnis speichern willst. 

6. Gebe folgenden Befehl in Git Bash ein: 
gitclone(deine kopierte URL)

7. Bestätige den Befehl mit der Eingabetaste.
[GitHub](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)

## 2. Installation der notwendigen Pakete
**Express** ist ein kleines und flexibles Node.js-Framework für Webanwendungen, das eine Reihe von robusten Funktionen für Web- und mobile Anwendungen bietet.

**pg** ist ein JavaScript-Client, welcher Verbindungen zur Datenbank von PostgreSQL herstellt und auch die Befehle der SQL ausführt.

**sqlite** ist eine Schnittstelle für Abfragen und Parameterbindung. Es umfasst die Debugging-Unterstützung. Ebenfalls unterstützt es Erwiterungen, einschliesslich verpackten Unterstützung füe die json1-Erweiterung.

**uuid** wird dazu benötigt, um Datenbankeinträge, Objekte in verteilten Systemen eindeutig zu kennzeichnen.

**wait-port** definiert, dass ein Dienst oder eine Anwendung warten soll bis ein bestimmter Port verfügbar ist. 

## 3. Docker-Konfiguration und -Installation
Um Docker herunterzuladen befolge diese Schritte:
1. Gehe auf die [Webseite](https://www.docker.com/products/docker-desktop/) von Docker.
2. Dort wählst du das blaue Feld in der Mitte des Fenster aus, mit der Beschriftung "Docker Desktop" und lädst die Version für dein Gerät herunter. 
3. Sobald du Docker auf deinem Rechner hast, kannst du die Anwendung öffnen und dich durch die Schritte klicken, nachdem kannst du ein Konto erstellen. Dann sollte die Docker bei dir funktionieren. 

## 4. Starten der Applikation in einem Docker-Container
Um die Applikation in Docker zu starten musst du den folgenden Schritten folgen:
1. Terminal öffnen als Admin.
2. Pfad zum Verzeichnis, in dem die ganzen Dateien gespeichert sind, angeben.
3. Danach folgende Befehle einer nach dem anderen eingeben:
    1. _ducker init_, die Fragen mit diesen Antworten bearbeiten:
    - What application platform does your project use? Node
    - What version of Node do you want to use? 18.0.0
    - Which package manager do you want to use? npm
    - What command do you want to use to start the app: node src/index.js
    - What port does your server listen on? 3000
    2. _docker compose up --build_, startet die Anwendung.