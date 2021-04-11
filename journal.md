---
title: Journal
description: Arbeitsprozess der Engine: Orion Entwicklung
published: 1
date: 2021-04-11T13:20:07.648Z
tags: 
editor: markdown
dateCreated: 2021-03-26T15:57:07.835Z
---

# 11.4.2021
- TCP-Remote Logik für ausgehende TCP-Verbindungen.
## Erledigt
- Erste Logik für TCP-Verbindungen zu anderen Nodes, strukturiert als GenServer.
- Temporärer Rust TCP-Server fürs Testen.
## Planung & Gedanken
- TCP-Listening hat immer noch Probleme.
- Dedizierter Registry Server für Remote-GenServer Prozesse.
- Ein zentraler Routing-Prozess wird benötigt, um Nachrichten in beide Richtungen zu verarbeiten.
## Aufgaben
- Registry (Custom oder Default)
- TCP-Listener
# 7.4.2021
- Multithreading Logik.
- Neue Implementierung der TCP-Listener Logik.
## Erledigt
- Angefangen den Code zu dokumentieren. Kann mit `cargo doc` generiert werden.
- Erstes README für Container-Repo geschrieben.
- Prototyp der Multithreading implementierung.
- Anstelle der bisherigen `:gen_tcp` Logik ist es einfacher `ranch` zu verwenden.
## Planung & Gedanken
- Multithreading ist einiges komplizierter als erwartet.
- Das Zusammenspiel zwischen den verschiedenen Threads muss sicher und zuverlässig geregelt sein, sonst könnte das System schnell zerfallen.
- Mit `ranch` lässt sich Code und Ports sparen, Verbindungen sollten einfacher geregelt werden können.
## Aufgaben
- Das Threadingproblem ist komplexer als gedacht und wird der Fokus in der nächsten Zeit sein.
- `thread.rs` dokumentieren.
- README erweitern & überarbeiten.
- Beidseitige TCP-Communikation.

# 4.1.2021
- Erste Routing Logik
## Erledigt
- Grundlegende Struktur der Routing Logik in Elixir.
- Vollständige implementierung des "self-fetching" (Informationen übers eigene System ins Elixir-System laden).
- Definiton der Felder für den Routing.Table und die "Remotes".
## Planung & Gedanken
- Ein eindeutiges und zuverlässiges System zum Kategorisieren und Speichern von aktiven Verbindungen wird benötigt.
- Nodes brachen einen "Score" um schlechtere Nodes ersetzen zu können, vorallem durch die Zeit seit der Verbindung.
- Wie kann man sicher gehen, dass jemand nicht den Verifizierungsprozess auschaltet? => Zufällige remote file requests.
## Aufgaben
- Strukturen und Funktionen für Remotes.
- Funktionen zur modifikation des Routing Tables.

# 31.3.2021
## Erledigt
- Repository ist [hier](https://github.com/EngineOrion/container) erreichbar.
- Start der Entwicklung der Container.
	- Implementierung der Command Line Arguements.
  - Angefangen das Prozessmanagement zu implementieren.
  - Angefangen das Configurationsmanagement zu implementieren.
## Planung & Gedanken
- Bisher haben wir die einzelnen Container als einzelne Prozesse implementieren wollen, aber dies hat wahrscheinlich zu viel Overhead, weshalb es mehr Sinn macht, einen Prozess zu starten und die Container als Green Threads zu starten. 
- Dies hat allerdings zur Folge, dass die einzelnen Interfaces gut geschützt sein müssen und keinesfalls Race Conditions entstehen. 
- Zudem muss sichergestellt sein, dass die Packets nicht an den falschen Thread geschickt werden.
## Aufgaben
- Die Programmiersprache entwerfen und den Tokenizer schreiben.
# 30.3.2021
- Definition des Portals
- Erster TCP-Receiver / Server
## Erledigt
- Ausarbeitung und Definition des Portals.
- Klare Definition der JSON-Kommunikation.
- Erster einfacher TCP-Listener mit erlang:gen_tcp.
- Einfacher Textinput für install.sh script.
## Planung & Gedanken
- Wichtige (noch teilweise offene) Frage: Welche Komponenten des Systems sollen aktiv (eigene Prozesse / Threads) und welche passiv sein?
- Sollen die TCP-Verbindungen vollständig bidirektional sein oder ist es akzeptabel mehrere Verbindungen zu öffnen?
- Es sollen einheitliche ID's / Keys im ganzen System verwendet werden, es braucht daher Umwandlungen ein allen verwendeten Sprachen.
## Aufgaben
- Fehlerbehebung und Tests für TCP-Listener
- Recherche über Unix-Domain-Sockets
# 26.3.2021
- Fertigstellung Instrastructure
- Erster Shadow Code, Key generation + Verification
## Erledigt
- Erstellung der Infrastruktur Präsentation
- Overview Darstellung & Erster kleiner Zeitplan
- Install Script zum erstellen von Keys & Verifizieren eines bekannten files.
- Erster Elixir Code zum Verifizieren der lokale Konfiguration
## Planung & Gedanken
- Um Keys im Cluster nicht stehlen zu können braucht es ein Client Secret mit dem Nodes sicher ihre ID bekommen. 
- Die ID wird generiert durch den Hash-Wert eines privaten Keys. (Sicherheit?)
- Dieser Key wird dann ebenfalls verwendet um ein bekanntes File zu signieren, wodurch andere Nodes die Integrität des Keys bestätigen können.
## Aufgaben
- User input in install script um überschreiben zu verhindern.
- Möglichkeiten zur "remote verification" in die Netzwerk-Planung einbauen.

# Template
## Erledigt
## Planung & Gedanken
## Aufgaben