# Konzepte-Moderner-Programmiersprachen

## Projekt 1: Transformation von imperativem zu funktionalem Java
### Beschreibung:
In diesem Projekt wurde ein imperatives Java-Programm, das XML-Dateien mit Musikalbum-Informationen liest und diese in Java-Objekte umwandelt, in ein funktionales Java-Programm überführt. Das Hauptziel dieses Projektes war es, den Java-Code in eine rein funktionale Form zu überführen, wobei Iterationen durch Rekursion ersetzt wurden.

### Hauptaufgaben:
- Analyse des vorhandenen imperativen Programms.
- Umsetzung einer Token-Erstellungsfunktion für XML-Daten.
- Parsing der Token-Liste zur Erstellung von Java-Objektstrukturen.

## Projekt 2: Überführung von Java zu Scala
### Beschreibung:
Das Hauptziel dieses Projekts war es, das in Projekt 1 erstellte funktionale Java-Programm in die funktionale Programmiersprache Scala zu übertragen.

### Hauptaufgaben:
- Einrichten der Scala-Entwicklungsumgebung.
- Implementierung der Token-Liste-Erstellungsfunktion und des Parsers in Scala.
- Einbindung von Pattern Matching und Nutzung von Case-Klassen in Scala zur Datenmodellierung.

## Projekt 3: Implementierung von Higher-Order-Funktionen
### Beschreibung:
In diesem Projekt wurde das in Scala geschriebene Programm von Projekt 2 erweitert, indem gebräuchliche Higher-Order-Funktionen manuell implementiert und angewendet wurden.

### Hauptaufgaben:
- Implementierung der Higher-Order-Funktion map.
- Nutzung der Higher-Order-Funktion zur Umwandlung von Album- und Track-Titeln in Großbuchstaben.
- Erweiterung der Higher-Order-Funktion, um verschiedene Datentypen zu verarbeiten.

# Projekt 4: Real-Time Kommunikation mit Web-Clients via Websockets

## Beschreibung:
In diesem Projekt wurde die Real-Time Kommunikation zwischen Web-Clients und einem Server über Websockets realisiert, ein Anwendungsfall für Concurrency und asynchrones Handling von individuellen Websocket-Connections. 

Anwendungsgebiete:
- Messaging Applikationen
- Multiplayer Games
- Collaboration Applikationen
- Infrastruktursysteme mit Near-Real-Time Event Notifications (z.B. "Build Job xyz wurde erfolgreich beendet")
- Applikationen mit Near-Real Time Updates von Location-Daten (aktueller Standort mobiler Clients)

Im Kontext dieses Praktikums wurde ein simuliertes Trouble Ticket System entwickelt, das in Echtzeit kommuniziert, "wer sich um welches Ticket kümmert", mittels "Selbst-Zuweisung".

## Technologie und Programmiersprachen:
- Backend (Server): Go
- Client: JavaScript (unter Node.js oder als Webclient im Browser)

## Anforderungen:
- Client muss Eingaben erfragen (für Client-ID & Selbstzuweisungen der Tickets).
- Server: Go Kommandozeilenprogramm mit der Fähigkeit, Tickets in Echtzeit hinzuzufügen.
- Nutzung echter Websockets (kein Long Polling, keine Server-Sent Events).
- Datenübertragung als JSON über die Websockets, keine URL-Parameter (mit Ausnahme des Verbindungsaufbaus).
- Fehlerhandling, insbesondere Schutz vor Fehleingaben der Ticketnummer.
- Keine Authentifizierung erforderlich.
- Daten-Updates werden vom Server zum Client gepusht, ohne Client-Anfrage.
- Asynchrone Datenverarbeitung in Go mittels Goroutines, um die Datenstruktur vor konkurrierenden Updates zu schützen.

## Abgabe:
Die Abgabe des Projekts erfolgte in Form einer .zip-Datei, die den Source Code, Konsolen-Log-Dateien und eine zeitlich chronologisch geordnete Textdatei mit Logs aller Systeme enthält.

