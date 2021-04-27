---
title: Infrastructure
description: Definition of the Orion Infrastructure and the components.
published: 1
date: 2021-04-27T10:53:17.803Z
tags: 
editor: markdown
dateCreated: 2021-03-24T17:14:03.320Z
---

# Übersicht

Mit der aktuell beliebten Infrastruktur zum entwickeln von verteilten
oder verbunden Diensten lässt sich viel erreichen. Doch meist ist der
Aufwand für selbst kleinste Applikationen unglaublich hoch. Mit einer
stärker integrierten Alternative basierend auf einem speziell
entwickelten verteilten Datensystems und Nachrichten-Protokoll sowie
einer Entwicklungsumgebung für das verarbeiten von Nachrichten soll sich
die Barriere für Entwickler gesenkt werden.\
Das gesamte System lässt sich wie folgt darstellen,
die einzelnen Komponenten werden danach einzeln besprochen:

![Übersicht aller wichtigen Komponenten (Blau = Nicht zwingend benötigt,
Implementierung nach der Zwischenpräsentation).](/overview.png)

# Portal

Als zentrales Herzstück der Infrastruktur muss ein Standard definiert
werden, mit welchen alle wichtigen Komponenten des Systems interagieren.
Jeder Container soll über dieses einheitliche Interface Zugang zu den
verschiedenen Datenquellen haben und möglichst einfach mit ihnen
interagieren können.

Da es sich beim Portal um eine Schnittstelle zwischen verschiedenen
Prozessen handelt sollen `Linux Sockets`{.verbatim} verwendet werden.
Mit einem klar definierten *binär-basierendem* Protokoll sollen die
eigenen sowie weitere beliebige Applikationen mit den Containern
interagieren können.

Wichtige Werte für jede Nachricht:

-   Sender Key
-   Receiver Key
-   Sender Service (Applikation die den Portal-Standard implementiert)
-   Nachricht / Inhalt
-   ...

Dabei ist es wichtig zu verstehen, dass die Sockets von verschiedensten
Prozessen geteilt werden, wobei bei den Containern lediglich der
verantwortliche die Nachrichten empfängt. Das Protokoll soll dabei
ähnlich wie HTTP lediglich Requests unterstützen, Pulls oder aktive
Verbindungen sollen vorerst nicht unterstützt werden.

# Container

Jeder Container besteht aus einer Reihe von Konfigurationen und einem
Script, geschrieben in `NET-Script`{.verbatim} (Die Sprache soll
speziell für das Verarbeiten von Netzwerk-Daten gebaut werden, daher der
Name).

Durch die Konfigurationen sollen verschiedene Keys und Sender Services
des Portals definiert werden, von welchen Nachrichten akzeptiert werden
sollen. Mit `NET-Script`{.verbatim} sollen dann eingehende Nachrichten
verarbeitet und gespeichert werden, sowie Antworten gesendet werden.

# Network

Zwar macht das verteilte Nachrichten-System lediglich eine Komponente
für das Portal aus, trotzdem soll es das zentrales Element ausmachen und
möglichst einfache Kommunikation zwischen verschiedenen Containern
erlauben.

Basierend auf dem bekannten `Kademlia-Routing`{.verbatim} sollen
einzelne Packets von Container zu Container über einen indirekten Weg
gehen, wodurch jegliche zentrale Router wegfallen.
