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

# Projekt: Entwicklung einer Phoenix Web App
## Hintergrund:

Für dieses Projekt wurde der Phoenix Web Framework in der Programmiersprache Elixir verwendet. Phoenix baut auf Elixir auf und bietet somit alle Vorteile der funktionalen Programmierung, unterstützt jedoch auch einen imperativen Programmierstil. Durch die Basis auf der Erlang VM BEAM sind Elixir und Phoenix besonders gut für die Parallelisierung und den Einsatz in Cluster-Umgebungen geeignet.
Projektziele:

    Kennenlernen der Hauptmechanismen von Phoenix und Phoenix LiveWire.
    Wertschätzen der Einfachheit, mit der eine App mit Live Update-Fähigkeiten in Phoenix realisiert werden kann.

# Projektbeschreibung:
## Aufgabe 1: Counter App

Die erste Aufgabe bestand darin, eine einfache "Counter" App im Phoenix Framework zu erstellen. Hierfür wurden die folgenden Schritte durchgeführt:

    Scaffolding: Eine App-Struktur namens "counter" wurde mittels Phoenix erstellt.
    Phoenix Webserver starten: Die App wurde lokal auf Port 4000 gehostet und über einen Webbrowser zugänglich gemacht.
    Routing und Live Controller: Routing für einen View "/counter" wurde eingerichtet, und ein "Live Controller" wurde erstellt, um den Counter-Wert dynamisch zu aktualisieren.
    Buttons hinzufügen: Schaltflächen zum Erhöhen des Counters wurden hinzugefügt.
    Event Handling: Für jeden Button wurde eine Event-Handling-Funktion implementiert, um den Counter-Wert entsprechend zu erhöhen.
    Real-Time Updates: Die App wurde so erweitert, dass Änderungen in Echtzeit über mehrere Clients synchronisiert werden können. Dies wurde durch Abonnieren und Veröffentlichen von Änderungen im "Live Controller" erreicht.

## Aufgabe 2: Chat App

In der zweiten Aufgabe wurde eine einfache Chat App in Phoenix LiveWire programmiert. 
## Fazit:

Das Projekt bot die Möglichkeit, tiefe Einblicke in die Funktionsweise des Phoenix Web Frameworks und Phoenix LiveWire zu erhalten. Die Implementierung des Counter und der Chat App hat gezeigt, wie einfach es ist, Apps mit Live Update-Fähigkeiten in Phoenix zu realisieren
