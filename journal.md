---
title: Journal
description: Arbeitsprozess der Engine: Orion Entwicklung
published: 1
date: 2021-06-12T14:57:05.995Z
tags: 
editor: markdown
dateCreated: 2021-03-26T15:57:07.835Z
---

# 12.06.2021
- Allgemeines Debugging & Vorbereitung auf Präsentation.
## Erledigt
- Anpassung verschiedener Module auf die Präsentation
- Planung für die Präsentation, Aufteilung der Aufgaben
## Planung und Gedanken
- Spannender Anfang -> Anzahl Angestellte, zu gross / zu klein.
## Aufgaben
- System nochmals im Schulnetz testen
- Probedurchlauf der Präsentation
# 7.06.2021
- Finale Implementierung von NET-Script
## Erledigt
- Die Implementierung von NET-Script wurde heute fast abgeschlossen.
- Implementierung einer Hilfenachricht bei Hunter.
## Planung und Gedanken
- Die neue Implementierung ist ziemlich universell und erlaubt es schnell neue Befehle zu implementieren.
## Aufgaben
- Es gibt noch kleine probleme beim Zugriff auf Variablen. Dies müssen noch behoben werden.
- Es fehlen noch einzlne Befehle und einen Teil des interfaces.
# 2.06.2021
- Bugfixing & Tests
## Erledigt
- Verteiltes testen des Datensystems
- Integration von Container in hunter
- Arbeiten am schriftlichen Kommentar
## Planung und Gedanken
- Der gesamte Durchlauf des Systems muss vor den einzelnen Komponenten erklärt werden.
- Die Demo ist nur bedingt sinnvoll, allerdings nur auf die Vorführung ausgelegt.
## Aufgaben
- Komponenten erklärung.
- Vollständiger Test
# 27.5.2021
- Weiterentwicklung der Containerapplikation.
## Erledigt
- Implementierung der `REPL` für die container Logik.
- Lösen der meisten Fehler beim kompilieren der container applikation.
- Veraltetes README überarbeiten 
- Help Commands auf den die neuen Befehle anpassen.
## Planung und Gedanken
- Die neue Schnittstelle der Containerlogik sollte die Nutzung detlich vereinfachen, sind aber noch nicht durchintegriert.
- Mit den neusten Fortschritten vom NET-Script jitten, wird es bald möglich sein container zu starten und zu testen.
- Zum Teil kann bei kleinen Fehlern die ganze Applikation abstürzen, was umbedingt behoben werden muss.
## Aufgaben
- NET-Script jitter weiterentwickeln und in die containerlogik integrieren.
- REPL weiter verbessern und mehr Funktionen einbauen.
- Bug-Fixing
# 24.5.2021
- Vollständige Integration von Hunter in Shadow & websocket.or
## Erledigt
- Wechsel von statischen Config Dateien auf "hunter cli".
- Testen des "hunter socket" Systems
## Planung & Gedanken
- Websockets müssen angepasst und vereinfacht werden, sonst sind nicht alle benötigten Werte vorhanden.
## Aufgaben
- Testen des gesamten Systems.
- Websocket.or umschreiben.
- Kommentar Projekte Abschnitt.
# 20.5.2021
- Grosse Fortschritte am schriftlichen Kommentar.
- Erste Integration zwischen Hunter und Shadow.
## Erledigt
- Einführung & Aussicht im schriftlichen Kommentar fertig gestellt.
- Weiterentwicklung an Hunter & Net-Script.
- Unix-Socket integrationsversuche zwischen hunter & shadow.
## Planung & Gedanken
- Für ein einfach benutzbares System werden Installations-Scripts und klare Routinen benötigt.
## Aufgaben
- Projekte Recherche & Realisierung im schriftlichen Kommentar
- Anpassung des Websocket-Interfaces an hunter.
# 16.5.2021
- Integration neuster Änderungen von "test_env".
- Integration `get` command line arguments für hunter.
## Erledigt
- Alle Änderungen von der Testumgebung wurden übernommen.
- Imnplementierung der Spezifikationen.
## Planung & Gedanken
- Es ist am einfachsten zwei getrennte Versionen zu haben, es wird aber ein System benötigt die Änderungen schnell zu integrieren.
## Aufgaben
- Full stack testing
- Shadow fault tolerance
- Die restlichen CL arguemente implementieren.
# 12.5.2021
- Debugging & Fixes für Shadow.
## Erledigt
- Verteiltes Testen des ganzen Systems.
- Lösen von Encoding & Formatting Fehlern.
## Planung & Gedanken
- Das Shadow System braucht noch mehr Error-Handling & Failsafes.
## Aufgaben
- Merge test_env into Shadow/dev.
- Shadow error handling & unit tests.
# 8.5.2021
- Verteiltes Testen von Shadow
- Überarbeiten des AOT-AST-Parsers
## Erledigt
- Verschiedenste Bug-Fixes & Optimierungen für Shadow
- Dedizierte Test-Umgebung für verteiltes Testen.
- Struktur und Einführung für den schriftlichen Kommentar.
- Integrationstests mit Unix Sockets / Hunter
- Funktionen und Defuns können nun AOT geparsed werden. Die entsprechenden Unit-Tests sind dafür geschrieben.
## Planung & Gedanken
- Das System (Shadow) braucht signifikant mehr error-handeling und fault-tolerance um skalierbar zu werden.
- Alle Routing Funktionen werden in einen dedizierten Router (hunter) ausgelagert, dadurch werden die einzelnen Komponenten unabhängiger.
- Zurzeit ist geplant, das Variablen beim Ausführen nach mit ihrem Namef gefunden werden. Dies könnte allerdings ineffizient werden, weshalb es sich anbieten würde sie mit ihrem Index anzusprechen. Dafür müsste aber der Parser zwei mal über eine Funktion um die Indexe zu verteilen.
## Aufgaben
- Full stack testing
- Shadow fault tolerance
# 3.5.2021
- Erste Implementierung des Websocket-Clients für Prototype-Demo.
- Überarbeitung des NET-Script Jitters
## Erledigt
- für den ersten Prototypen wurden heute die verbleibenden Aufgaben aufgeteilt.
- Der Websocket-Client grundlegend implementiert, Android-App / Web-Client muss noch gemacht werden.
- Variablen sind für Rust Instancen des `Variablen` Structs.
- Variablen können ohne Umwandlung in jede Funktion übergeben werden. Jede Rust source Funktion fragt zuerst nach dem richtigen Typ und beginnt erst dann die eigentliche Aufgabe.
## Planung & Gedanken
- Es ist einfacher die Datenbank auf der anderen Seite des Portals zu haben, da sie für jeden Container benögtigt wird. 
- Das Portal soll als dedizierter Container, "Routing", gehandhabt werden.
- Da schlussendlich alles Objekte sind ist es möglich NET-Script AOT (Ahead Of Time) zu Jitten, damit es bei Gebrauch direkt verwendet werden kann.
## Aufgaben
- Socket-Matching von Container zu WS.
- Definition USER-ID's
- Funktionen implementieren und die Init-Routine.
# 1.5.2021
- Erste Unix-Socket Implementierung für shadow
## Erledigt
- Erste Testes beider Komponenten und der Kommunikation über Unix-Sockets.
- Implementierung der Socket Logik integriert ins restliche System (Routing).
## Planung & Gedanken
- Socket file muss bei jedem Neustart gelöscht werden.
- Mit einem einheitlichen Messaging-System lassen sich alle Quellen ähnlich verarbeiten.
- Das aktuelle System erlaubt es nicht, neue Message-Typen zu definieren.
- Das aktuelle "Loop-Prevention-System" ist nicht sinnvoll, Systemzeiten sind zu verschieden.
## Aufgaben
- Messaging-log an Nachrichten anfügen, send check einbauen.
# 27.4.2021
- Erstes verteiltes Testen mehrerer verbundener Systeme
## Erledigt
- Verschiedenste Bug-Fixes und Optimierungen.
- Allgemeine Dokumentation & Type-Safety.
## Planung & Gedanken
- Es wird langfristig irgend ein Script oder andere Lösung benötigt, um mit verschiedenen Instanzen einfacher umgehen zu können.
- Das Shadow System ist aktuell bis auf eine Verbindung zum System fertiggestellt.
## Aufgaben
- Einfacheres (admin) Interface für häufige Funktionen.
- Send-Funktion für neue, externe Nachrichten mit Target Query.
# 26.4.2021
- Start der Implementierung des NET-Script jitters
## Erledigt
- NET-Script kann nun rudimentär geparsed werden. 
- Einige NET-Script Funktionen, welche in Rust implementiert werden müssen, wurden implementiert.
- Dokumentation des Jitters. Dies beinhaltet die eine Beschreibung der Funktionen und Beispiele wie die Funktionen genutzt werden können.
- Unit tests für den Jitter
## Planung & Gedanken
- Bisher wurden nur sehr einfache NET-Script instruktionen implementiert und diese wurden noch nicht ausgiebig getestet.
- Ausserdem können die Funktionen noch optimiert werden.
## Aufgaben
- Ausbauen der Unit-Tests
- Implementierung eines constructors für das Struct `ReturnResult`.
# 25.4.2021
- Confirmation activation
## Erledigt
- Auch wenn es zu einem unendlichen Two-Generals-Problem führt ist es wichtig, dass die activation requests bestätigt werden. Nach jedem requests wird jetzt eine Nachricht zurück geschickt (Typ 3).
## Planung & Gedanken
- Auch wenn beide Komponenten mit externen Servern & Clients getestet wurden muss das ganze System auf mehreren Geräten getestet werden.
- Danach fehlt nur noch die Integration mit dem Sockets um einen Prototypen abzuschliessen.
## Aufgaben
- Unit-Testing & Type-Safety
- Multi-Node Testing
# 21.4.2021
- Aktivierungslogik für direkte Kommunikation zwischen zwei Nodes.
- Interaktionen (Export) mit dem lokalen Dateisystem. 
## Erledigt
- Neu verbindende Nodes können (und müssen) jetzt aktiviert werden,
  indem sie spezielle Requests schicken und die nötigen Daten übertragen.
- Genauere Definition der Portal-Logik (Path=/proc/orion/shadow.sock).
- Routing Logik für eingehende Nachrichten und Unterscheidung zwischen
  lokalen und externen Containern. 
## Planung & Gedanken
- Shadow lässt sich teilweise optimieren, indem verschiedene
  Komponenten mit ähnlichen Funktionen (Router & Supervisor) noch
  weiter integriert werden. Dabei muss man aber aufpassen, nicht
  komplette Funktionen der Sprache neu zu erfinden.
- Für spätere Versionen muss man sich mit Edge-Cases und schlechten
  Verbindungen kümmern, aktuell hofft man immer auf perfekte
  Bedingungen. 
## Aufgaben
- Aktivierung muss beantwortet werden, damit sie tatsächlich
  beidseitig ist. -> Die existierende Logik lässt sich wieder
  verwenden, solange die gleichen Ausgangssituationen vorhanden sind. 
- Error handeling und Unit tests.
# 20.4.2021
- Umstrukturierung der Code-Struktur fürs Datensystem.
## Erledigt
- Allgemeine Umstrukturierung des Codes.
- Entfernung unnötiger Abschnitte (Verification)
- Eigene Routing / Supervisor Logik
- Erste Vorschläge fürs Nachrichtenprotokoll
## Planung & Gedanken
- Durch einen zentralen Routing-Prozess lässt sich die allgemeine
  Infrastruktur stark vereinfachen.
- Es ist möglich sowohl "listener" als auch "sender" in einem Modul zu
  haben, da sie ähnliche Callback-Strukturen haben. Dadurch sinkt der
  Aufwand und Umfang stark.
## Aufgaben
- Monitor & Map-Update finalisieren. 
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