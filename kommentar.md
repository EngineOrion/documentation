---
title: Kommentar
description: 
published: 1
date: 2021-05-25T18:46:11.559Z
tags: 
editor: markdown
dateCreated: 2021-04-09T18:22:03.942Z
---

# Project Orion - Kommentar

! AUTOCONVERTED !

::: {.ABSTRACT}
TODO: Abstract
:::

`\newpage`{=latex}

# Vision

::: {.CENTER}
1.  Oktober 1964 - UCLA an Standford: LO
:::

*1964* rechnete niemand mit der fundamentalen Änderung unserer Existenz
und Lebensweise, die mit dieser einfachen Nachricht in Bewegung gebracht
wurden. Eigentlich hätte die erste Nachricht über das
`ARPANET`{.verbatim} im Jahre 1964 `LOGIN`{.verbatim} heissen sollen,
doch das Netzwerk stürzte nach nur zwei Buchstaben ab. Ob dies als
schlechtes Omen für die Zukunft hätte gewertet werden sollen bleibt eine
ungeklärte Frage. Aber das Internet ist hier und es ist so dominant wie
noch nie zuvor. Jetzt ist es in der Verantwortung jeder neuen Generation
auf diesem Planeten, mit den unglaublichen Möglichkeiten richtig
umzugehen und die Vielzahl an bevorstehenden Katastrophen und Gefahren
zu navigieren.\
`\noindent`{=latex} Ohne das Internet wären wir aufgeschmissen. Unsere
Arbeit, Kommunikation und unser Entertainment sind nicht einfach nur
abhängig von der enormen Interkonnektivität des Internets würden ganze
Industrien und Bereiche unser Gesellschaft gar nicht erst existieren.
Das Internet hatte einen selbstverstärkenden Effekt auf sein eigenes
Wachstum. Der um ein Vielfaches schnellere Datenaustausch und die enorme
Interkonnektivität führten dazu, dass jede neue Innovation und jede neue
Plattform im Internet noch schneller noch mehr User erreichte und auf
immer unvorstellbarere Grössen anwuchs.\
`\noindent`{=latex} Das ist ja grundsätzlich nichts Schlechtes. Das
Internet hat eine unvorstellbare Menge an Vermögen, Geschwindigkeit und
Bequemlichkeit für uns alle geschaffen und wir haben unsere
Gesellschaftsordnung daran ausgerichtet. Aber man muss sich fragen, ob
wir manche der Schritte nicht doch überstürzt haben. Im Namen des
Wachstums und aus `FOMO`{.verbatim} (*Fear Of Missing Out*) wurden
Technologien für die Massen zugänglich, die eigentlich nie für solche
Grössenordnungen entwickelt wurden. Denn sobald die immer höheren
Erwartungen an teils unglaublich fragile Systeme nicht mehr erfüllt
werden kommt es schnell zur Katastrophe. Und durch unsere Abhängigkeit
von diesen Systemen steht bei einem solchen Szenario nicht nur der
Untergang einiger Produkte oder einzelner Firmen bevor, nein es könnte
zum Kollaps ganzer Länder oder Gesellschaften kommen.\
`\noindent`{=latex} Egal wie sicher und zuverlässig unsere *öffentliche*
Infrastruktur auch scheinen mag, es lassen sich doch schnell Risse im
System erkennen. Nicht nur an der Oberfläche, sondern auch im Herzen
unserer digitalen Leben gibt es Probleme. Oftmals handelt es sich dabei
nicht um *Kleinigkeiten*, *Meinungsverschiedenheiten* oder
*Kontroversen* sondern um physikalische Grenzen, grundlegende
Designfehler und das vielseitige Versagen der involvierten Parteien.\
`\noindent`{=latex} In den nächsten Kapiteln sollen einige dieser
zentralen Probleme besprochen werden. Dabei soll versucht werden nicht
nur die fehlerhaften Implementierungen zu erklären, sondern auch die
dadurch entstandenen Probleme in Verbindung mit unseren täglichen
Interaktionen und Verwendungen des Internets zu bringen. In einem
nächsten Schritt soll dann eine Lösung besprochen werden: ein System mit
welchem sich möglichst viele der grössten Probleme lösen lassen und
welches tatsächlich praktischen Nutzen bietet.\
\*\* IP-V4 `\noindent`{=latex} In der Geschichte der Menschheit haben
wir aus vielen verschiedenen Gründen Krieg geführt. Für Wasser, Nahrung,
Öl, Frieden oder Freiheit in den Krieg zu ziehen scheint zu einer fernen
Welt oder zur Vergangenheit zu gehören. Und auch wenn diese
grundlegenden Verlangen gedeckt sind, werden schon bald neue Nöte
aufkommen. Während *Daten* oft als Gold des 21. Jahrhunderts bezeichnet
werden, gibt es noch eine andere Ressource, deren Vorräte wir immer
schneller erschöpfen.\
`\noindent`{=latex} $4'294'967'296$. So viele
`IP-V4`{.verbatim}-Adressen wird es jemals geben.
`IP-V4`{.verbatim}-Adressen werden für jedes Gerät benötigt, dass im
Internet kommunizieren will und dienen zur eindeutigen Identifizierung.
Aktuell wird die vierte Version (`V4`{.verbatim}) verwendet. In einer
Wirtschaft in der unendliches Wachstum als letzte absolute Wahrheit
geblieben ist, kann ein solch hartes Limit verheerende Folgen haben.
Besonders wenn die limitierte Ressource so unendlich zentral für unser
aller Leben ist wie nichts anderes. Mit `IP-V6`{.verbatim} wird zurzeit
eine Alternative angeboten, die solche Limitierungen nicht hat. Aber der
Wechsel ist eine freiwillige Entscheidung, für die nicht nur alle
Betroffenen bereit sein müssen, sondern für die auch jeder einzelne
Komponente auf der Strecke diese neue Technologie unterstützen müssen.\
\*\* Routing

::: {.center}
Freiheit und Unabhängigkeit sind menschlich. Es darf niemals bestraft
werden, nach diesen fundamentalen Rechten zu streben. Und doch führt das
egoistische Streben nach Freiheit zu Problemen, oftmals allerdings nicht
für die nach Freiheit Strebenden.
:::

Genau diese Situation findet man im aktuellen Konflikt um die Grösse von
*Address-Abschnitten* vor. Um dieses Problem richtig zu verstehen muss
als erstes die Funktion der *Zentralrouter* und der globalen
Netzwerkinfrastruktur erklärt werden:\
`\noindent`{=latex} Jedes Gerät im Internet ist über Kabel oder Funk mit
jedem anderen Gerät verbunden. Da das Internet aus einer Vielzahl von
Geräten besteht, wäre es unmöglich, diese direkt miteinander zu
nverbinden. Daher lässt sich das Internet besser als *umgekehrte
Baum-Struktur* vorstellen:

-   Ganz unten finden sich die Blätter, die Abschlusspunkte der
    Struktur. Sie stellen die *Endnutzergeräte* dar. Jeder Server, PC
    und jedes `iPhone`{.verbatim}. Hier ist es auch wichtig
    festzustellen, dass es in dieser Ansicht des Internets keine
    magische *Cloud* gibt. Aus der Sicht des Netzwerks sind alle
    Endpunkte gleich, auch wenn manche für Konsumenten als *Server*
    gelten.
-   Die Verzweigungen und Knotenpunkte über den Blättern, dort wo sich
    Äste aufteilen, stellen *Router* und Switches dar. Hier geht es
    allerdings nicht um Geräte, die sich in einem persönlichen Setup
    oder einem normalen Haushalt finden. Mit Switches sind die
    Knotenpunkte (`POP-Switches`{.verbatim}) der Internet Anbieter
    gemeint. Diese teilen eingehende Datenströme auf und leiten die
    richtigen Daten über die richtigen Leitungen.
-   Ganz oben findet sich der Stamm. Während ein normaler Baum natürlich
    nur einen Stamm hat, finden sich in der Infrastruktur des Internets
    aus Zuverlässigkeitsgründen mehrere. Von diesen
    `Zentralroutern`{.verbatim} gibt es Weltweit nur eine handvoll und
    sie sind der Grund für das Problem.

`\noindent`{=latex} Die `Zentralrouter`{.verbatim} kümmern sich nicht um
einzelne Adressen, sondern um Abschnitte von Adressen, auch
`Address Spaces`{.verbatim} genannt. An den zentralen Knotenpunkten geht
es also nicht um den genauen Server oder das genaue Gerät, zu dem etwas
gesendet werden muss, stattdessen wird eher entschieden, ob gewisse
Daten beispielsweise von Frankfurt aus nach Ost- oder Westeuropa
geschickt werden müssen.\
`\noindent`{=latex} Im Laufe der Jahre wurden die grossen Abschnitte an
Adressen aber immer weiter aufgeteilt. Internet-Anbieter und grosse
Firmen können diese Abschnitte untereinander verkaufen und aufteilen.
Und jede Firma will natürlich ihren eigenen Abschnitt, ihren eigenen
`Address Space`{.verbatim}. Für die Firmen hat dies viele Vorteile,
beispielsweise müssen weniger Parteien beim finden des korrekten
Abschnitts involviert sein. Aber für die `Zentralrouter`{.verbatim}
bedeutet es eine immer grössere Datenbank an Zuweisungen. Dieses Problem
geht so weit, dass die grossen *Routingtables* inzwischen das
physikalische Limit erreichen, was ein einzelner Router verarbeiten
kann.

## Zentralisierung

`\noindent`{=latex} Die Macht in den Händen einiger weniger Kapitalisten
und internationaler Unternehmen ist unvorstellbar gross. Einige wenige
CEO\'s, welche nie gewählt, überprüft oder zur Rede gestellt wurden,
sind in voller Kontrolle unserer Leben. Egal welcher politischen,
wirtschaftlichen oder gesellschaftlichen Ideologie jemand auch folgt,
eine solche Abhängigkeit wirft gewisse Fragen und Probleme auf.\
`\noindent`{=latex} Tatsächlich muss man nicht lange suchen, um
tatsächliche Gefahren im Zusammenhang mit verschiedenen
Technologieunternehmen zu finden. Besonders wenn es um den Datenschutz
geht, haben Social-Media Dienste keinen besonders guten Ruf.\
`\noindent`{=latex} Aber neben den ideologischen Fragen und
Sicherheitsbedenken gibt es auch noch sehr praktische Probleme in der
Art, wie moderne Internet-Dienste implementiert sind.

### Datenschutz

::: {.center}
*Wenn man nicht für etwas zahlt, ist man das Produkt.*
:::

Nach dieser Idee ist man für ziemlich viele Firmen ein Produkt. Doch
leider muss man realisieren, dass man selbst bei kostenpflichtigen
Diensten als Produkt gesehen wird. Denn das Internet hat einen neuen
Rohstoff zur Welt gebracht. Wer viele Daten über Menschen besitzt,
bekommt binnen kürzester Zeit Macht.\
`\noindent`{=latex} In ihrer einfachsten Funktion werden Daten für
personalisierte Werbung eingesetzt. Damit lassen sich Werbungen
zielgerichtet an Konsumenten schicken und der Umsatz, sowohl für Firmen
als auch für Anbieter, optimieren.\
`\noindent`{=latex} Werbung ist mächtig und hat einen grossen Einfluss
auf den Markt. Aber damit lassen sich lediglich Konsumenten zu Käufen
überzeugen oder davon abraten. Wenn man dies mit dem tatsächlichen
Potential in diesen Daten vergleicht, merkt man schnell, wie viel noch
möglich ist. Denn die Daten die sich täglich über uns im Internet
anhäufen, zeigen mehr als unser Kaufverhalten. Von
Echtzeit-Positionsupdates, Anrufe, und Suchanfragen bis hin zu privaten
Chats und unseren tiefsten Geheimnissen, sind wir meist überraschend
unvorsichtig im Umgang mit digitalen Werkzeugen.\
`\noindent`{=latex} Während man davon ausgehen muss, dass Firmen, deren
Haupteinnahmequelle Werbungen ist, unsere Daten sammeln und verkaufen,
gibt es eine Vielzahl an anderen Firmen die ebenfalls unsere Daten
sammeln, obwohl man von den meisten dieser Firmen noch nie gehört hat.
Die Liste der potentiellen Mithörer bei unseren digitalen Unterhaltungen
ist nahezu unendlich: Internet-Anbieter, DNS-Dienstleister,
CDN-Anbieter, Ad-Insertion-Systeme, Analytics-Tools, Knotenpunkte &
Datencenter, Browser, Betriebssysteme, ....\
`\noindent`{=latex} Aus dieser Tatsache heraus lassen sich zwei zentrale
Probleme formulieren:

-   Selbst für die einfachsten Anfragen im Internet sind wir von einer
    Vielzahl von Firmen und Systemen abhängig. Dieses Problem wird noch
    etwas genauer im Abschnitt [*Abhängigkeit*]{.spurious-link
    target="Abhängigkeit"} besprochen.
-   Wir haben weder ein Verständnis über die involvierten Parteien noch
    die Bereitschaft, Bequemlichkeit dafür aufzugeben.

### Implementierung

`\noindent`{=latex} Wer sich mit digitaler Infrastruktur auseinander
setzt weiss, dass Webseiten und Apps über *Server* laufen. Diese Server,
die eigentlich nichts anderes als optimierte Computer sind, verarbeiten,
speichern und liefern die unglaublichen Datenmengen, welche für unser
digitales Leben benötigt werden. Mit einem Server, den man selbst mieten
oder kaufen kann, steht einem dann nichts im Weg, eine digitale
Plattform ähnlich wie *Facebook* oder *Twitter* zu starten. Doch man
realisiert schnell, dass *Facebook* und *Twitter* nicht einfach auf
einem *Server* laufen. Denn die benötigten Ressourcen dieser Plattformen
übersteigen die Kapazität einzelner *Server* um ein Vielfaches.\
`\noindent`{=latex} Für einen normalen Nutzer mag es so wirken, als ob
er *das Facebook* nutzt. In Wahrheit werden seine Anfragen aber von
hunderten oder gar tausenden von *Servern* verarbeitet. Auch wenn keine
offiziellen Daten verfügbar sind nimmt man an, dass *Facebook* aus über
`200'000`{.verbatim} *Servern* besteht.\
`\noindent`{=latex} Wenn man sich diese Situation von einer
Infrastruktur-Perspektive aus genauer anschaut, sieht man eine
interessante Situation vorliegen:\
\#+CAPTION: Abstrakte Darstellung der Facebook Infrastruktur.

![](facebook.png)

`\noindent`{=latex} Viele Nutzern greifen also über einen zentralen
Knotenpunkt auf viele Server zu. Dieses System, das in bestimmten
Situationen schneller ist, sorgt für einen erhöhten Aufwand während der
Entwicklung. Anstatt nämlich die verschiedenen *Server* auf dem gleichen
Netzwerk wie die Nutzer zu haben, müssen spezielle Lösungen entwickelt
und verwaltet werden. Und während die Nutzer weiterhin mit der Illusion
*des Facebooks* leben dürfen, haben sie keine Kontrolle über die
Sicherheit und Zuverlässigkeit dieser internen Systeme.\
`\noindent`{=latex} Dazu führt dieses System zu einem offensichtlichen
Knotenpunkt, durch welchen alle Daten fliessen müssen. Sollten bei
diesem zentralen Punkt nun aber Probleme auftreten lassen sich alle
Dienste und Server dahinter nicht mehr erreichen, auch wenn diese
eigentlich von den Problemen nicht betroffen wären.\
`\noindent`{=latex} In einem Schritt sorgt diese Abstrahierung der
internen Infrastruktur zu Situation, in der normale Nutzer sich
`Facebook`{.verbatim} als einzelnen Dienst vorstellen und sich gar nicht
bewusst sind, durch wie viele Systeme ihre Daten im Hintergrund
fliessen. Denn es garantiert niemand, dass alle Einheiten in einem
System wie bei `Facebook`{.verbatim} tatsächlich auch zu
`Facebook`{.verbatim} gehören und ob die Daten aller Nutzer tatsächlich
bei dieser einen Firma bleiben.

### Abhängigkeit

In einem fiktionalen Szenario[^1] erklärt *Tom Scott* auf seinem
YouTube-Kanal was passieren könnte, wenn eine einzelne
Sicherheitsfunktion beim Internetgiganten `Google`{.verbatim}
fehlschlagen würde. In einem solchen Fall ist es natürlich logisch, dass
es zu Problemen bei den verschiedensten `Google`{.verbatim}-Diensten
kommen würde. Aber schnell realisiert man, auf wie vielen Seiten Nutzer
die *Sign-In with Google* Funktion benutzen. Und dann braucht es nur
eine böswillige Person um den Administrator-Account anderer Dienste und
Seiten zu öffnen, wodurch die Menge an Sicherheitsproblemen exponentiell
steigt.\
`\noindent`{=latex} Aber es muss nicht immer etwas schief gehen, um die
Probleme zu erkennen. Sei es politische Zensur, *Right to Repair* oder
*Net Neutralität* die grossen Fragen unserer digitalen Zeit sind so
relevant wie noch nie.\
`\noindent`{=latex} Während die enorme Abhängigkeit als solche bereits
eine Katastrophe am Horizont erkennen lässt, gibt es noch ein
konkreteres Problem: Den Nutzern (*den Abhängigen*) ist ihre
Abhängigkeit nicht bewusst. Wenn sie sich ihren Alltag ohne
`Google`{.verbatim} oder `Facebook`{.verbatim} vorstellen, denken sich
viele nicht viel darunter. Weniger *lustige Quizfragen* oder Bilder von
Haustieren, aber was könnte den schon wirklich schlimmes passieren?\
`\noindent`{=latex} Während es verständlich ist, dass das Benutzen von
`Google`{.verbatim} natürlich von `Google`{.verbatim} abhängig ist, so
versteht kaum jemand, wie viel unserer täglichen Aktivitäten von
Diensten und Firmen abhängen, die selbst wieder von `Google`{.verbatim}
abhängig sind.\

::: {.center}
All dies führt dazu, dass wir auf eine globale Katastrophe zusteuern,
die nur darauf wartet, zu passieren.
:::

## Entwicklung

## Katastrophe

Nachdem nun eine Vielzahl an Problemen angesprochen wurden muss, auch
noch die anstehende Katastrophe beschrieben werden, sollte sich nichts
verändern. Es gibt verschiedene Gründe durch welche es zu einer solchen
digitalen Katastrophe kommen könnte. Manche sind nur eine Frage der
Zeit, sollte sich nichts grundlegend verändern. Andere könnten durch den
kleinsten Fehler, sei es technisch oder menschlich ausgelöst werden.\
`\noindent`{=latex} Es wurden mehrere Engpässe angesprochen. Ob es um
Platz im Zentralrouter oder um `IP-Adressen`{.verbatim} geht, ist damit
zu rechnen, dass es Konflikte, geheime Absprachen und ungerechte
Verteilung dieser wichtigen Ressourcen geben wird. All dies natürlich
nur wenn wir keinen tatsächlichen Krieg starten oder das System vorher
zusammenbricht.\
`\noindent`{=latex} Für viele wird die angesprochene Zentralisierung
kaum als Katastrophe wirken. Zwar ist für viele die unvorstellbare Macht
in den Händen so weniger bereits Katastrophe für sich, trotzdem ist es
wichtig zu realisieren, dass diese absolute Abhängigkeiten von wenigen,
fragilen Systemen selten zu Gutem geführt hat.

## Engine: Orion

`\noindent`{=latex} Das Internet mit all seinen Facetten und Anwendungen
hat viele Probleme. Einige wurden hier bereits angesprochen, andere
würden den Rahmen dieser Arbeit sprengen und wieder andere wurden noch
gar nicht entdeckt oder als Probleme identifiziert. Aktuell versuchen
wir bei jedem neuen Problem eine neue, meist temporäre Lösung zu finden,
nur um nichts am System als ganzes ändern zu müssen.\
`\noindent`{=latex} Langfristig ist es aber von Nöten, ein neues System
zu entwickeln. Eine grundlegende Neuentwicklung der Art, wie wir mit
digitalen Systemen interagieren. Nur mit einem solchen Wandel können wir
die digitale Katastrophe nicht einfach nur verschieben, sondern
grundlegenden los werden.

`\noindent`{=latex} `Engine: Orion`{.verbatim} soll eine Rolle in diesem
Systemwandel spielen und eine erste Vorlage für ein solches *System der
nächsten Generation* bieten. Dabei geht es nicht um ein einzelnes
Produkt oder eine Dienstleistung welche vollständig entwickelt und ohne
Mangel ist. Stattdessen sollen verschiedene Komponenten und Systeme
entwickelt werden, welche genau gegen die angesprochenen Probleme
vorgehen. Mit dem Zusammenschluss dieser Systeme soll es dann möglich
sein, das vollständige System vorzuführen und damit einen Schritt in die
Richtung des nötigen Wandels gehen.

# Projekte

Mit den zentralen Problemen definiert ist es nun an der Zeit, andere
Projekte zu analysieren um herauszufinden, ob die Probleme bereits oder
zumindest teilweise gelöst wurden.\
`\noindent`{=latex} Wie bereits in der [*Vision*]{.spurious-link
target="Vision"} angesprochen, soll sich `Engine:
Orion`{.verbatim} auf zwei Aspekte fokussieren:

-   Ein Nachrichtensystem zum senden und lenken der einzelnen
    Nachrichten.
-   Ein System zur Verarbeitung der einzelnen Nachrichten.

Dementsprechend sollen auch Projekte in diesen beiden Richtungen
analysiert werden. Um aber die Wahl der Projekte richtig zu verstehen,
muss man die Vision hinter `Engine: Orion`{.verbatim} im Blick behalten.
Denn es wird schnell klar, dass es für alle beschriebenen Probleme
entweder temporäre Lösungen oder einzelne Projekte zur Umgehung der
Probleme gibt. Daneben existieren auch grundlegendere Neuentwicklungen
bekannter Systeme, welche einzelne Probleme lösen, meist aber andere
Ziele haben. Was allerdings kein bekanntes Projekt versucht umzusetzen,
ist nicht nur die grundlegende Neuentwicklung zentraler Systeme zur
Behebung bekannter Probleme, sondern dazu noch die nahtlose Integration
der einzelnen Komponenten für ein durchgehend integriertes,
zusammenspielendes System.\
`\noindent`{=latex} Da ein solches Projekt nicht öffentlich existiert
müssen stattdessen die einzelnen Probleme und deren Lösungsversuche
angeschaut werden. Dafür wird grundlegend in die beiden zentralen
Komponenten unterschieden. Die Integration der beiden Teile soll hier
nicht besprochen werden, da sie sich hauptsächlich in der Umsetzung
zeigt.

## Verteilte Systeme

Viele der Probleme stammen von Designfehlern in unserer globalen
Routinginfrastruktur. Mit einer Alternative zu diesem veralteten System
würden sich eine Vielzahl von Problemen auf einmal lösen. Der
Grundlegende unterschied zwischen *dezentralisierten Systemen* und der
aktuellen Umsetzung besteht in der Funktion der Router. Die Problematik
der *Zentralrouter* wurde bereits angesprochen, aber auch kleinere
Router führen oft zu Problemen, hauptsächlich die absolute Abhängigkeit
die wir zu ihnen entwickelt haben. Ohne unsere Internetanbieter und die
Dienste die sie uns zur Verfügung stellen wären wir hilflos
aufgeschmissen, denn nur die Internetanbieter sind in der Lage ihre
Nutzer und Netzwerke mit Routern untereinander zu verbinden.\
`\noindent`{=latex} Auch wenn es viele verschiedene Ideen und
Umsetzungen der dezentralisierten Ideen gibt, basieren doch die meisten
von ihnen zumindest teilweise auf `Kademlia`{.verbatim}, welches als
erster Schritt verstanden werden muss.

### Kademlia

Wie geht man also gegen die totale Abhängikeit von Internetanbietern und
zentralen Routern vor?\
Man kann ja nicht einfach seine eigenen Router aufsetzen und einen
alternativen Dienst anbieten. Neben den technischen Schwierigkeiten
würde es auch überhaupt nicht gegen das eigentliche Problem vorgehen.\
`\noindent`{=latex} Der Trick, der mit Systemen wie
`Kademlia`{.verbatim} verwendet wird, ist es also, Router vollständig zu
eliminieren. Dies ist möglich, indem jedes Mitglied des Netzwerks neben
seinen normalen Funktionen gleichzeitig auch noch als Router agiert.
Strenggenommen werden in `Kademlia`{.verbatim} Router also nicht
wirklich eliminiert, lediglich der Nutzen für zentrale Router fällt weg.

`\noindent`{=latex} In einem früheren Abschnitt wurden die Probleme der
*Zentralrouter* bereits angesprochen. Wenn jetzt aber jedes Mitglied in
einem Netzwerk plötzlich als Router agiert und es keine zentrale Instanz
gibt, träfe die Problematik der *Zentralrouter* viel mehr Server. Genau
da kommt `Kademlia`{.verbatim} ins Spiel. Aber was genau ist
`Kademlia`{.verbatim} eigentlich?\
`\noindent`{=latex} Laut den Erfindern, *Petar Maymounkov* und *David
Mazières*, ist es

::: {.center}
ein Peer-to-peer Nachrichten System basierend auf XOR-Metrik.
:::

Was genau bedeutet das und wie lässt sich eine `XOR`{.verbatim}-Metrik
für verteilte Datensysteme einsetzen?

Da die einzelnen Server nicht in der Lage sind, Informationen über das
komplette Netzwerk zu speichern oder zu verarbeiten, funktionieren
`Kademlia`{.verbatim}-Systeme grundlegend anders. Anstelle der
hierarchischen Anordnung der Router ist jedes Mitglied eines Systems
gleichgestellt. Dazu kümmert sich jedes Mitglied auch nicht um das
komplette System, sondern nur um sein direktes Umfeld. Während dies für
kleinere Systeme gut funktioniert und ähnliche Performance liefert,
skaliert es nicht so einfach für grosse Systeme. Genau dafür gibt es die
`XOR`{.verbatim}-Metrik.

1.  Distanz:

    Die `XOR`{.verbatim}-Funktion, die in der Informatik an den
    verschiedensten Orten auftaucht, wird verwendet um die Distanz
    zwischen zwei Zahlen zu berechnen. Die Zahlen repräsentieren dabei
    Mitglieder im Netzwerk und sind je nach Variante im Bereich
    $0..2^{160}$(*20 Bytes*) oder $0..2^{256}$(*32 Bytes*). Mit einem so
    grossen Bereich lässt sich auch direkt das Problem der limitierten
    `IP-Adressen`{.verbatim} lösen. Auch wenn es kein tatsächlich
    unlimitiertes System ist, so gibt es doch mehr als genug Adressen
    (Ein ähnliches Zitat gibt es wahrscheinlich vom Erfinder der
    `IPV4-Adressen`{.verbatim}, allerdings gibt es mit
    `Kademlia`{.verbatim}-Systemen tatsächlich die Chance, sie noch zu
    erweitern.\
    `\noindent`{=latex} Wenn mit `XOR`{.verbatim}-Funktionen einfach die
    Distanz zwischen zwei Zahlen berechnet wird, stellt sich die Frage,
    wieso nicht einfach die Differenz verwendet wird. Um dies zu
    beantworten, muss man sich die Eigenschaften der
    `XOR`{.verbatim}-Funktion etwas genauer anschauen:

    1.  $xor(x, x) = 0$: Das Mitglied mit seiner eigenen Adresse ist am
        nächsten zu sich selbst.
    2.  $xor(x, y) > 0$ wenn $x != y$: Die Funktion produziert nie
        negative Zahlen und nur mit zwei identischen Parametern kann man
        $0$ erhalten.
    3.  $xor(x, y) = xor(y, x)$: Die Reihenfolge der Parameter spielt
        keine Rolle.
    4.  $xor(x, z) <= xor(x, y) + xor(y, z)$: Die direkte Distanz
        zwischen zwei Punkten ist am kürzesten oder gleich kurz wie die
        Distanz mit einem zusätzlichen Sprung.
    5.  Für ein gegebenes $x$ und eine Distanz $l$ gibt es nur genau ein
        $y$ für das $xor(x, y) = l$ gilt.

    `\noindent`{=latex} Aber wieso genau funktioniert dies? Wieso kann
    man `XOR`{.verbatim}, eine Funktion zur Berechnung der
    Bit-Unterschiede in zwei Binärzahlen, verwenden, um die Distanz
    zwischen zwei Punkten in einem verteilten Datensystem zu berechnen?\
    Um dies zu verstehen hilft es, sich das System als umgekehrten Baum
    vorzustellen. Unter dem obersten Punkt stehen alle Mitglieder im
    System. Mit jedem weiteren Abzweigung zweier Teilbäume halbiert sich
    die Anzahl. Man wählt am einfachsten zwei Abzweigungen pro Knoten,
    da sich damit die werte direkt als Binärzahlen darstellen lassen,
    wobei jeder Knotenpunkt einfach eine Stelle in der langen Kette aus
    $0$ oder $1$ darstellt. Der ganze Baum sieht dann wie folgt aus[^2]:

    ![Beispielhafte Darstellung eines einfachen
    Kademlia-Systems](tree.png)

    `\noindent`{=latex} Mit dieser Sicht auf das System beschreibt die
    `XOR`{.verbatim}-Funktion die Anzahl der unterschiedlichen
    Abbiegungen im Baum und somit die Distanz. Zwar mag es auf den
    ersten Blick nicht intuitiv wirken, wieso man `XOR`{.verbatim},
    anstatt einfach der Differenz verwendet, allerdings funktioniert die
    Funktion mit Binärzahlen in einem solchen Baum einiges besser.

2.  Routing-Table:

    In einem `Kademlia`{.verbatim}-System hat jedes Mitglied eine
    gewisse Anzahl anderer Mitglieder, mit denen es sich verbunden hat.
    Da `Kademlia`{.verbatim} ein sehr umfangreiches, kompliziertes
    Protokoll und System beschreibt, sollen hier nur einige zentrale
    Funktionen besprochen werden, die für diesen ersten Prototypen von
    `Engine:
         Orion`{.verbatim} relevant sind. Besonders beim
    `Routing Table`{.verbatim} lassen sich einige Abschnitte weglassen,
    welche zwar für die Optimierung und Skalierung eines Systems wichtig
    sind, allerdings für das Analysieren eines einfachen, kleinen
    Systems wie `Engine: Orion`{.verbatim} irrelevant sind.\
    `\noindent`{=latex} Einfach formuliert speichert der
    `Routing Table`{.verbatim} die verbundenen Mitglieder. Eine
    eingehende Nachricht wird dann mithilfe dieser Liste, sowie der
    `XOR`{.verbatim}-Metrik ans richtige Ziel geschickt. Um das System
    zu optimieren und die Anzahl der benötigten Sprünge klein zu halten,
    wird ein spezielles System verwendet, um zu entscheiden, welche
    Mitglieder im `Routing-Table`{.verbatim} gespeichert werden sollen:

    1.  Sehr nahe an sich selbst (in der obigen Darstellung also: wenige
        Sprünge im Baum) werden alle Mitglieder gespeichert.
    2.  Umso weiter weg sich die Mitglieder befinden, desto weniger
        werden gespeichert.

    `\noindent`{=latex} Die optimale Anzahl der gespeicherten Mitglieder
    hängt von den Zielen und Ansprüchen an das System ab. Grundlegend
    muss man die Frage beantworten, mit wie vielen Unterbäumen
    Verbindungen gehalten werden sollen. Zwar mag dies etwas abstrakt
    wirken, lässt sich aber mit den eben eingeführten Modell eines
    umgekehrten Baumes gut erklären:

    -   In der obersten Ebene trennt sich der Baum in zwei vollständig
        getrennte Teile, was sich mit jeder weiteren Ebene wiederholt.
    -   Die einzige Möglichkeit vom einen *Ende* des Baums zum anderen
        zu kommen, ist über den obersten Knoten. Um also in die andere
        Hälfte zu kommen, braucht man mindestens eine Verbindungsstelle
        in der anderen Hälfte.
    -   Deshalb braucht ein `Routing-Table`{.verbatim} nicht nur kurze
        Verbindungen zu nahen Punkten, sondern auch einige wenige
        Verbindungen zu Mitgliedern in der anderen Hälfte.
    -   Mit nur einer solchen Verbindung hat man *seine* und die
        *andere* Hälfte. Hat man zwei solche Verbindungen auf die andere
        Seite hat man schon viertel.
    -   Man muss also entscheiden, wie klein man die andere Hälfte
        aufteilen will. (Eine genaue Unterteilung bedeutet wenige
        Sprünge aber grosse `Routing-Tables`{.verbatim}, eine grobe
        Unterteilung genau das umgekehrte).

    `\noindent`{=latex} Zwar hat ein vollständiges
    `Kademlia`{.verbatim}-System noch komplexere Elemente, wie
    `k-Buckets`{.verbatim}, welche den `Routing-Table`{.verbatim}
    optimieren, allerdings sind diese für die grundlegende
    Funktionsweise des Systems irrelevant.\
    `\noindent`{=latex} Die dynamische Regulation des
    `Routing-Tables`{.verbatim} muss allerdings noch erwähnt werden:

    -   Sobald die definierte maximalgrösse erreicht ist, werden keine
        neuen Verbindungen akzeptiert.
    -   Zwar können Einträge durch neuere ersetzt werden, allerdings
        werden dabei nicht alte, sondern inaktive Einträge entfernt.

### BitTorrent

Dezentralisierung hat viele Vorteile und muss langfristig flächendeckend
eingesetzt werden. Aktuell sind die meisten Industrien und Produkte noch
nicht so weit. Trotzdem gibt es einige Anwendungen und Gruppen bei denen
solche Systeme bereits seit Jahren zentrale Verwendung finden.\
`\noindent`{=latex} Beispielsweise im Zusammenhang mit dem Verbreiten
von *(mehr oder weniger legalen)* Materialien, wie Filmen oder Musik
wird eines der grössten globalen verteilten Systeme eingesetzt.
Natürlich gibt es hunderte von verschiedenen Programmen, Ideen und
Umsetzungen, wobei die meisten Nachfolger `Napsters`{.verbatim} sind.\
`\noindent`{=latex} Im preisgekrönten Film *The social network* erhält
man Einblick in den Lebensstil von `Sean Parker`{.verbatim}, einem der
Gründer von `Napster`{.verbatim}. Es mag einen überraschen, wie jemand
wie Parker, der nur wenige Jahre zuvor mit `Napster`{.verbatim} die
komplette Musikindustrie über den Haufen geschmissen hatte, eine so
zentrale Rolle in `Facebook`{.verbatim}, einem der zentralisiertesten
Megaunternehmen der Welt, einnehmen konnte.\
`\noindent`{=latex} Auch wenn es noch nicht *vollständig*
dezentralisiert ist, erlaubte es `Napster`{.verbatim} Nutzern, Musik
über ein automatisiertes System mit anderen Nutzern zu teilen und neue
Titel direkt von den Geräten anderer Nutzer herunterzuladen. Dabei gab
es zwar immer noch einen zentralen Server, der die Titel sortierte und
indizierte.\
`Napster`{.verbatim} musste am Ende abgeschaltet werden, nachdem die
Klagen der Musikindustrie zu belastend wurden. Auch wenn das Produkt
abgeschaltet wurde, liess sich nichts mehr gegen die Idee unternehmen.\
`\noindent`{=latex} Über viele Iterationen und Generationen hinweg
wurden die verteilten Systeme immer weiter verbessert, jegliche zentrale
Server entfernt und in die Hände immer mehr Nutzer gebracht. Heute läuft
der Austausch über `BitTorrent`{.verbatim}.

`\noindent`{=latex} `BitTorrent`{.verbatim} baut auf der gleichen
grundlegenden Idee wie `Napster`{.verbatim} auf: Nutzer stellen ihren
eigenen Katalog an Medien zur Verfügung und können von Inhalte von allen
anderen Mitgliedern im System herunterladen. Anders als
`Napster`{.verbatim} gibt es bei `BitTorrent`{.verbatim} keine zentrale
Komponente, stattdessen findet selbst das Indizieren und Finden von
Inhalten dezentralisiert statt. Dafür wird über das
`Kademlia`{.verbatim}-System sehr aktiv bekannt gegeben, wer welche
Inhalte zur Verfügung stellt, wobei einzelne Mitglieder ebenfalls
speichern können, wer ebenfalls die gleichen Inhalte anbietet. Neben der
Dezentralisierung und Sicherheit lassen sich über
`BitTorrent`{.verbatim} tatsächlich gute Geschwindigkeiten erreichen, da
sich Inhalte direkt von mehreren Anbietern gleichzeitig herunterladen
lassen. Da es sich bei `BitTorrent`{.verbatim} um eigentlich um ein
grosses Dateisystem handelt, lassen sich direkt die
`SHA1`{.verbatim}-Hashwerte der Inhalte als
`Kademlia`{.verbatim}-Adressen verwenden.

### CJDNS

## Verarbeitung

# Realisierung

\[Was, Wie, Wie überprüft, logische nicht zeitliche Abfolge, Methoden\]

## Shadow

## Hunter

## Container

## NET-Script

## Sources

# Evaluation

\[Auswertung der Erebnisse, Interpretation, Was erreicht?\]

## Demo

## Messungen

# Ausblick

Was auch immer mit diesem Projekt noch geschehen mag, Potential hat es
auf auf jeden Fall genug. Die möglichen Verbesserungen, Erweiterungen
und Optimierungen sind nahezu unbegrenzt. In den nächsten Abschnitten
sollen ein paar der nächsten Schritte besprochen werden, wobei die
Realisierbarkeit immer im Blick behalten werden muss.\
`\noindent`{=latex} Dazu ist es wichtig, die Ziele und Prinzipien hinter
`Engine:
Orion`{.verbatim} im Kopf zu behalten: Während andere versuchen,
kommerzielle Lösungen zu entwickeln und diese für möglichst viele Nutzer
möglichst einfach anzubieten, soll mit `Engine: Orion`{.verbatim} etwas
anderes erreicht werden. Die vielen Probleme und nötigen Veränderungen
wurden bereits angesprochen. Anstatt diesen Wandel aber alleine
durchzudrücken versucht `Engine: Orion`{.verbatim} ein Schritt in einer
langen, technischen Revolution hin zu grundlegend neuer Infrastruktur zu
sein. Mit dem Bewusstsein für dieses Ziel sollen nun die nächsten
Schritte behandelt und später auch umgesetzt werden.

## Vervollständigung

Als erster Schritt, bevor Visionen oder Träume umgesetzt werden können,
muss den ursprünglichen Zielen nachgekommen werden. Auch wenn
`Engine: Orion`{.verbatim} von Anfang an als Prototyp gehandhabt wurde,
liegt aktuell mehr ein Prototyp eines Prototypen vor. Zwar erfüllt
dieser seine Aufgaben, kann aber darüber hinaus eher wenig. Neben der
offensichtlich fehlenden Nutzerfreundlichkeit ist das System als ganzes
auch noch nicht allgemein einsetzbar. Zwar existieren die Grundlagen und
das System ist grundsätzlich brauchbar, so fehlt es noch an
verschiedenen praktischen Funktionen um das System zu vervollständigen.

## Adressen

Für einen Prototypen mag es ausreichen, die Menge an verfügbaren
Adressen zu limitieren und einen fixen Wert zu nutzen. Für ein
tatsächlich skalierbares, dynamisches System wird es aber wichtig diese
Abschnitte an reservierten Adressen dynamisch zu machen. Dafür soll ein
Prozess namens `Keyspace negotiations`{.verbatim} eingesetzt werden, der
es verbundenen Mitgliedern erlauben soll, über die Grösse der
reservierten Abschnitte zu verhandeln.\
`\noindent`{=latex} Sobald sich aber die grössen der Abschnitte während
der Lebenszeit eines Objekts in einem dieser Abschnitte ändert, kommen
neue Probleme auf:

-   Externe Prozesse, die auf das Objekt zugreifen wollen, müssen über
    die Änderung informiert werden.
-   Sollte dies nicht möglich sein (da die Prozesse beispielsweise
    kurzzeitig nicht verfügbar sind), muss das ursprünglich
    verantwortliche Mitglied in der Lage sein, eingehende Nachrichten
    für das Objekt an das neu verantwortliche Mitglied zu schicken.
-   Da sich die Adresse aufgrund der obigen Probleme nicht ändern darf,
    muss sie beim neuen Mitglied reserviert bleiben. Dies bedeutet, dass
    die Veränderung der Abschnitte keine Vorteile bringen würde, da je
    nach Situation eine Vielzahl der neuen Adressen reserviert sein
    müsste.

Um diese Probleme zu umgehen, muss neben dem Adressen-System noch ein
zusätzliches ID-System eingeführt werden, welches bereits teilweise im
aktuellen System vorhanden ist. Mit diesen zweiteiligen System ist es
möglich, nur die ID\'s zu reservieren, während die Adressen frei werden.
Zwar muss damit jeder, der eindeutig mit einem Objekt kommunizieren will
einen zusätzlichen Wert speichern, aber es vereinfachst sowohl das
verteilte Routing, als auch das lokale.

## DNS

Das eben angesprochene Zwei-Komponenten-System geht klar gegen die
Nutzerfreundlichkeit. Daher ist es vorteilhaft, ein zusätzliches System
einzuführen, dass aus diesem Werte-Paar eine einheitliche
Identifizierung macht.\
`\noindent`{=latex} Da mit einem solchen System kein technisches,
sondern eher ein praktisches Problem gelöst werden soll, stehen viel
mehr Möglichkeiten zur Verfügung:

-   In seiner einfachsten Form präsentiert dieses System die beiden
    Werte einfach als einheitlichen String, der dann in allen Systemen
    verwendet werden kann. Technisch wäre diese Variante ganz klar die
    einfachste, bringt allerdings nur bedingt viel Nutzerfreundlichkeit,
    da die neuen Werte zufällig wirken würden.
-   Tatsächlich gibt es bereits ein dezentralisiertes Domain-System,
    nämlich im `Dark-Net`{.verbatim} in Form von
    `=Onion-Adressen`{.verbatim}. Mit diesen Adressen ist es möglich,
    einzelne Mitglieder im System genau zu finden. Da die Adressen
    direkt von den privaten & öffentlichen Schlüsseln abgeleitet werden,
    gibt es Programme und Scripts die es einem erlauben, Adressen
    gezielt zu generieren. Der limitierende Faktor dabei ist die
    verfügbare Rechenleistung, denn das passende Schlüsselpaar wird
    durch ausprobieren gefunden. Damit ist es Nutzern möglich zumindest
    die ersten paar Zeichen einer solchen Adresse zu bestimmen, auch
    wenn der Rest weiterhin zufällig ist.
-   Neben den *deterministischen* Varianten, die durch Kryptographie und
    Mathematik die Adressen finden und garantieren, gibt es noch einen
    anderen Weg. Ähnlich wie das aktuelle Domain-Name-System wäre ein
    System denkbar, indem Adressen per Broadcast an möglichst viele
    Nodes verteilt werden, die dann ihren eigenen Routing-Table
    dementsprechend anpassen. Natürlich wird irgend ein System benötigt,
    um die Integrität der Adressen zu validieren, dafür lässt sich aber
    potentiell direkt ein anderer *nächster Schritt*, nämlich ein
    Währungssystem verwenden. Auch garantiert dieses System nicht, dass
    Nutzer tatsächlich das richtige Mitglied finden. Je nach
    Implementierung könnte es sogar passieren, dass mehrere Mitglieder
    in einem Netzwerk die gleiche Adresse anbieten. Auch wenn dies in
    sich wieder zu Gefahren und Problemen führt, wäre es das nächste zum
    aktuellen System, wodurch der Wechsel reibungsfreier werden könnte.

## Balance

In einem System ohne klare Rollen, oder genauer: in einem System in dem
jedes Mitglied gleichwertig ist und alle möglichen Rollen gleichzeitig
einnimmt, braucht es ein System, das Nutzer belohnt, die mehr Arbeit
übernehmen und mehr für das System beitragen.\
`\noindent`{=latex} Grundsätzlich gibt es zwei Möglichkeiten, um solche
unbelohnte Arbeit zu vermeiden:

-   Man kann dafür sorgen, dass jedes Mitglied ungefähr gleichmässig
    ausgelastet ist. Dafür beim weiterleiten jeder Nachricht in Betracht
    gezogen werden, wie viel ein bestimmtes Mitglied in letzter Zeit
    ausgelastet war, und dementsprechend den Weg der Nachricht anpassen.
    Dies führt zwar dazu, dass jedes Mitglied mehr oder weniger gleich
    viel oder zumindest proportional gleich viel Daten verarbeitet, aber
    es führt zu einem weniger effizienten System, da Nachrichten in
    bestimmten Situationen nicht den direkten Weg nehmen.
-   Mit einem Währungs- oder Punktesystem wäre es möglich, Mitglieder
    direkt dafür zu belohnen, mehr Arbeit zu übernehmen. Innerhalb
    dieser Idee gibt es noch zwei Unterkategorien, die unterschieden
    werden müssen:
    -   Ein lokales Punktesystem, welches jedem Mitglied im Routingtable
        eines einzelnen Mitglieds einen Punktestand zuweist. Der
        Punktestand wird mit eingehenden Nachrichten angepasst, zieht
        aber auch Laufzeit und Netzwerk-Status in Betracht.
    -   Ein globales Währungssystem, vergleichbar mit einer
        Cryptocurrency. Das erfolgreiche verarbeiten und weiterleiten
        von Nachrichten würde in einem solchen System also mit Guthaben
        belohnt. Hierbei müsste man entscheiden, ob der Vorrat an dieser
        Währung limitiert ist, die Belohnung also durch die Mitglieder
        ausgezahlt wird, an die die Nachricht ausgeliefert werden soll,
        oder ob der Vorrat ähnlich wie `Bitcoins`{.verbatim} unendlich
        ist, und für jede Nachricht, für jeden Eintrag neues *Geld*
        gedruckt wird. Da nicht alle Mitglieder in einem verteilten
        Nachrichten und Datensystem gleich viel Last auf das System
        bringen, würde eine solche Währung einen Grund bringen, dem
        System zu helfen und Nachrichten zu verarbeiten.

# Footnotes

[^1]: Tom Scott: Single Point of Failure <https://youtu.be/y4GB_NDU43Q>

[^2]: Wikipedia: Kademlia <https://en.wikipedia.org/wiki/Kademlia>
