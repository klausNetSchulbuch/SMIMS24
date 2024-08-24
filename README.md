# Graphen 

## Mit Hilfe von Python und Jupyter-Notebooks

### Abstract 

> Graphen spielen eine große Rolle in vielen Alltagssituationen sowie in der wissenschaftlichen Informatik. Sie sind Teil der Informatik-Lehrpläne (mindestens der Leistungskurse) der gymnasialen Oberstufe. Beispielsweise findet man das Thema in dem schulinternen Lehrplan von NRW (siehe z.B. 
[https://www.schulentwicklung.nrw.de/lehrplaene/lehrplannavigator-s-ii/gymnasiale-oberstufe/
informatik/hinweise-und-beispiele/schulinterner-lehrplan/uv\_lk\_q1\_v.html](https://www.schulentwicklung.nrw.de/lehrplaene/lehrplannavigator-s-ii/gymnasiale-oberstufe/informatik/hinweise-und-beispiele/schulinterner-lehrplan/uv_lk_q1_v.html))

> **1. Analyse von Graphen in verschiedenen Kontexten**

>(a) Grundlegende Begriffe (Graph, gerichtet – ungerichtet, Knoten,
    Kanten, Kantengewicht)
    
>(b) Aufbau und Darstellung von Graphen anhand von Graphenstrukturen in
    verschiedenen Kontexten (Adjazenzmatrix, Adjazenzliste)
    
> **2. Die Datenstruktur Graph im Anwendungskontext unter Nutzung der
> Klassen Graph, Vertex und Edge.**

>(a) Erarbeitung der Klassen Graph, Vertex und Edge und beispielhafte Anwendung der Operationen
>
>(b) Bestimmung von Wegen in Graphen im Anwendungskontext (Tiefensuche,
    Breitensuche) 
    
>(c) Bestimmung von kürzesten Wegen in Graphen im
    Anwendungskontext (Backtracking, Dijkstra).
    
> (d) Bestimmung von minimalen Spannbäumen eines Graphen im
> Anwendungskontext.
>
> Die im folgenden aufgeführten Details sind entstanden,
> um Graphen im Unterricht für die Schülerinnen und Schüler erfahrbar zu
> machen, zum Beispiel unter Nutzung von Python und JupyterNotebooks.
> Dazu wurden entwickelt: 

>-   zwei Python-Bibliotheken, mit denen die Verwaltung von
    ungerichteten Graphen einfach gelingt.

>-   eine für die Schülerinnen und Schüler geeignete sehr kurze
    Einführung in die Begriffswelt von Graphen.

>-   ein Jupyter-Notebook, das den Schülerinnen und Schülern als
    Arbeitsmaterial vorgelegt wird.

Einführung 
-----------

An vielen Stellen des Alltags begegnen uns sogenannte *Graphen*:

-   Das Netz des öffentlichen Nahverkehrs bildet einen Graph; die
    einzelnen Haltestellen (*Knoten*) sind durch Linien (*Kanten*)
    miteinander verbunden.

-   Mit Hilfe von Graphen kann ein soziales Netzwerk die Beziehungen der
    Menschen modellieren, indem die Personen (Knoten), die miteinander
    befreundet sind, mit Kanten verbunden werden.

Schülerinnen und Schüler sollten im Informatikunterricht der
Sekundarstufe 2 (besonders sicherlich in einem Leistungskurs) diese
wichtige Datenstruktur kennenlernen und grundlegende Algorithmen
verstehen, entwickeln und implementieren, wie z.B.:

-   Tiefen- und Breitensuche in einem Graphen

-   *Euler-Weg* und *Hamilton-Weg*

-   Kürzeste Wege; der *Dijkstra-Algorithmus*

-   Spannbäume; *Algorithmus von Kruskal* oder *Algorithmus von Prim*

-   MaxFlowProblem; *Ford-Fulkerson-Algorithmus*

-   TravellingSalesmanProblem; z.B. genetische oder andere approximative
    Algorithmen

Im Rahmen der Unterrichtseinheit *Graphen* sollten die Grundbegriffe der
Graphentheorie vorgestellt werden. *Euler-Wege* und die damit
verbundenen Probleme, Sätze und Methoden können dort gute Dienste
leisten.

Das Problem des *Kürzesten Weges* ist sicherlich besonders gut geeignet,
um das Thema *Graphen* zu motivieren. In einem Jupyter-Notebook wird die
didaktisch-methodische Aufbereitung und Präsentation des
*Dijkstra-Algorithmus* unter Nutzung von Python
thematisiert.

Die Programmiersprache *Python*
--------------------------------

Als Programmiersprache bietet sich *Python* an:

-   Die Syntax ist besonders einfach, so dass ein Algorithmus, der
    bereits umgangssprachlich in einer Art Pseudocode entwickelt wurde,
    leicht implementiert werden kann.
-   Die Semantik der Basiskonzepte ist leicht verständlich.
-   Ein Python-Programm erfordert weniger Code (als Java), daher kann
    ein Programm schneller und verständlicher erzeugt werden.
-   Programmbausteine können einfach getestet werden (Vorteil einer
    Interpretersprache); damit unterstützt Python das sog. *Prototyping*.
-   Python stellt eine Unmenge von Bibliotheken bereit, die es
    gestatten, sich bei der Implementation von Algorithmen auf die
    wesentlichen Aspekte konzentrieren zu können, ohne viele technische
    Details kennen zu müssen.
   - Die graphische Darstellung von (kleinen) Graphen gelingt z.B. mit speziellen Python-Bibliotheken ohne großen Programmieraufwand.
-   Die Installation von Python sowie von schüler- bzw. schulgerechten
    IDEs (wie z.B. Jupyter, s.u.) auf allen Betriebssystemen und allen Geräten gelingt problemlos.

Zwar ist zur Zeit in den Schulen die Programmiersprache Java weit
verbreitet. Doch in den Lehrplänen (mindestens dem Lehrplan in NRW) wird
keine Programmiersprache vorgeschrieben, und der Informatikunterricht
ist sicher kein Programmierkurs, sollte also nicht den Eindruck
hinterlassen, dass das Erlernen einer bestimmten Programmiersprache im
Mittelpunkt stünde. Ziel des Informatikunterrichts sollte u.a. darin
bestehen, wichtige zentrale Ideen und Strukturen aus Informatik zu
vermitteln.

Dabei benötigt man sicherlich auch(!) eine Programmiersprache, damit
z.B. Algorithmen implementiert werden können und ihre Funktionalität
überprüft werden kann. Es dient nicht zuletzt der Motivation, wenn das
lauffähige Programm das gewünschte Ergebnis produziert.

### Die Rolle von Jupyter-Notebooks 

Als Programmierumgebung können Juypter-Notebooks (JNB)genutzt
werden. Sie sind webbasiert und ermöglichen einen interaktiven Umgang
der Schülerinnen und Schüler mit den - über die JNB direkt zur Verfügung
gestellten - Lernmaterialien.

Im schulischen Kontext enthält ein JNB Lehrtexte, Bilder, Links als auch
ausführbaren Python-Code. JNBs können mehrere Zwecke erfüllen:

1\. Ein JNB ist ein vorbereitetes digitales *dynamisches Arbeitsblatt:*

> - es ist ein Tutorial mit Erklärtexten und -bildern, vorbereitetem
> Code, Aufgaben…

2\. Ein JNB ist ein sog. *Computational Essay:*

> - es ist ein digitales Notizbuch, mit dem die lesende Person
> interagieren kann.

3\. Ein JNB ist ein sog. *Worked Example:*

> -   es enthält lauffähige und veränderbare Programme.

Typischerweise enthält ein JNB Lehrtexte, die wie ein traditionelles
Schulbuch die fachlichen Grundlagen vermitteln. Anders jedoch als ein
Schulbuch kann ein JNB dynamische Bilder, anklickbare Links, Videos, …
enthalten. Mit Hilfe von *MarkDown* (eine Art HTML-Light) können
diese Inhalte formatiert werden.

Daneben findet sich in einem JNB ausführbarer Python-Code. Schülerinnen
und Schüler lernen so die Syntax und Semantik von Python, können den
Code interaktiv verändern und erweitern, verbessern und
vervollständigen.

Als Entwicklungsumgebung ist der *Anaconda-Navigator* mit den
*Jupyter-Notebooks* besonders geeignet: 

- kostenlos
-   leicht zu installieren
-   Browser-basiert; in allen gängigen Browsern lauffähig
-   für alle Plattformen verfügbar

Bei der Installation von Anaconda wird auch automatisch (in der Regel
die neueste Version von) Python installiert.

- Geplant ist ein landesweit verfügbarer Jupyter-Server, so dass an Schulen keine Installationen notwendig sind. 
    
- Schülerinnen und Schüler können dann jederzeit von jedem Ort auf die Umgebung und alle dort bereitgestellten Daten und Notebooks zugreifen.
 
Jupyter-Notebooks sind spezielle Dateien, die mit dem Jupyter-System
geöffnet werden können. Sie haben die Dateiendung ipynb.

Die Python-Bibliothek networkx 
-------------------------------

Um in Python Graphen zu verwalten, kann man z.B. die Bibliothek `networkx`
nutzen. Dabei handelt es sich um eine im Internet frei zugängliche
Bibliothek. Dort findet man auch eine sehr umfangreiche
Dokumentation aller verfügbaren Funktionen.

Mit Hilfe dieser Bibliothek und der dort bereitgestellten Klasse `Graph`
ist es u.a. möglich, ungerichtete Graphen zu verwalten.

Details zu den Bibliotheken attrDirGraph und simpleGraph 
---------------------------------------------------------

Die oben erwähnte Bibliothek `networkx` ist zwar sehr leistungsstark,
jedoch aus Sicht des
Informatikunterrichts an Schulen komplex und für Schülerinnen und
Schüler gerade bei der Einführung in das Thema *Graphen* nur bedingt geeignet. 

Deswegen wurden zwei Bibliotheken
entwickelt, die alle Klassen und Funktionen aus der erwähnten Bibliothek
erben, jedoch für Lernende einen einfachen Umgang mit den notwendigen
Funktionen erlauben.

Die Bibliothek `attrDirGraph` stellt eine Python-Klasse bereit, mit der
ungerichtete
Graphen verwaltet werden können. Jeder Knoten und jede Kante eines
solchen Graphen kann beliebig viele, vom Benutzer frei zu benennende
Attribute erhalten. Insbesondere kann jede Kante ein Gewicht haben, so
dass dann der Graph (im Sinne der Graphentheorie) ein gewichteter
Graph ist.


Besonders in Zusammenhang mit dem zu implementierenden
Dijkstra-Algorithmus benötigt man spezielle Markierungen der Kanten und
Knoten. Dazu stellt die Bibliothek `simpleGraph` weitere Vereinfachungen
zur Verfügung.


Eine Dokumentation aller Funktionen dieser Klassen ist in den
Bibliotheksdateien in Form von Python-Kommentaren zu finden. Der Umgang
mit den beiden Klassen kann optimal bei der Benutzung des
Jupyter-Notebooks erfahren werden.

Anmerkung zu den assert-Statements in den Bibliotheken 
-------------------------------------------------------

Alle Funktionen in den beiden Bibliotheksklassen mit sog.
assert-Statements abgesichert. Wenn man beispielsweise ermitteln möchte,
ob der Knoten “H” bereits besucht wurde, dieser Knoten jedoch in dem
Graphen nicht enthalten ist, wird eine aussagekräftige Fehlermeldung
erzeugt, die das Programm beendet oder mit einer entsprechende Aktion
behandelt werden kann. Diese Fehlerprüfungen sind jedoch sehr
zeitintensiv. Wenn man sicher ist, dass solche Situationen niemals
auftreten, kann man auf diese Prüfungen verzichten.

Dazu gibt es beide Bibliotheken als unsafe-Versionen, in Unterverzeichnissen.

Um sicher zu gehen, dass die Operationen fehlerfrei implementiert sind, sollte man in einem ersten Programmlauf die safe-Versionen importieren.

Die beigefügten Dateien 
------------------------

1.  In dem Verzeichnis GraphBib findet man die Bibliotheken.
2.  Im dem Verzeichnis Daten sind einige csv-Dateien, in denen Graphen
    beschrieben sind und in Jupyter-Notebooks eingelesen werden können.
3.  Das Jupyter-Notebook `Dijkstra-Lernen.ipynb` können Schülerinnen und Schüler das
DijkstraVerfahren kennenlernen. 
