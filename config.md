---
title: Configuration
description: 
published: 1
date: 2021-04-23T17:32:10.059Z
tags: info
editor: markdown
dateCreated: 2021-04-23T17:32:07.435Z
---

# Struktur
- Fixer Path: */etc/orion/* (Aktuell noch hard-coded / in binaries)
- *member.json*: Exportiertes (autogeneriertes) file für die
  Verbindung mit anderen Nodes.
- *config.json*: Zentrales config file. Wird einmalig autogeneriert,
  danach READ-ONLY für alle Dienste. Nutzer setzt dort die IP-Addr,
  Ports, ähnliches.
- *secret.key*: RSA-Private file. Wird getrennt von restlicher Config
  gespeichert, um den zugriff möglichst schwer zu machen.
- *services.json*: Speichert alle installierten Container. File wird
  sowohl vom System gelesen, als auch geschrieben.
