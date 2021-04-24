---
title: Portal Definition
description: Communication Interface between local components.
published: 1
date: 2021-04-23T17:32:21.745Z
tags: 
editor: markdown
dateCreated: 2021-03-30T17:16:24.242Z
---

# Einführung

Unser System soll in logische und einfache Komponenten aufgeteilt werden. Das hat aber zur folge, das die einzelnen Komponenten miteinander kommunizieren müssen. 

# Technologien

Der Interconnect basiert auch Linux IPC Sockets und dient als zentrale Schnittstelle zwischen den Schnittstellen. Zu den Schnittstellen für das Backend gehören die Datenbank, welche Node spezifisch ist und der Transportlayer innerhalb des verteilten Datensystems. Das Interface für HTTP und Websocket Verbindungen kommuniziert auch über diese Schnittstelle. 

Der Datenaustausch erfolgt mit JSON Objekten. Wir haben uns für JSON entschieden, weil es ein sehr einfachen und leicht verständlichen Syntax hat und weit verbreitet ist. Ausserdem haben alle aktuellen Sprachen Libraries um JSON Objekte zu parsen.

Die JSON Objekte müssen die folgenden Elemente besitzen: 

- Sender
- Empfänger
- Sender Service
- Body

Das heisst, ein Beispielsobjekt könnte folgendermassen aussehen:
```
{
	"sender": ID,
	"receiver": ID,
	"service": SERVICE,
	"body": 
	{
		"base64 encoded body"
	}
}
```

Die drei Grundparametern müssen vorhanden sein, damit die Kommunikation problemlos verläuft. Der Body-Inhalt ist aber abhängig von den Daten die übermittelt werden sollen. Als Inhalt lässt sich grundsätzlich alles übermitteln, solange es als Base64-String ausgedrückt werden kann. Später sollen zusätzlich dedizierte Funktionen hinzukommen, um es einfacher zu machen, gewisse Daten zu übertragen, beispielsweise Files oder time-series-data.

Das heisst, dass mit der aktuellen Implementation nur Requests möglich sind und es ist zurzeit kein anderer Typ geplant, dies lässt sich allerdings erst nach Analyse des Datenverkehrs final entscheiden.

Das JSON Objekt wir vom Container mit der entsprechenden Empfänger-ID verarbeitet und der NET-Script-Code entscheidet wie mit dem Inhalt weiter verfahren werden soll.