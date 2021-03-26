---
title: Journal
description: Arbeitsprozess der Engine: Orion Entwicklung
published: 1
date: 2021-03-26T16:03:59.917Z
tags: 
editor: markdown
dateCreated: 2021-03-26T15:57:07.835Z
---

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