# Glossar

Dieses Glossar enthält Begriffe, die im gesamten Jupyter-Buch verwendet werden. Die Beschreibungen sollten im Kontext der biologischen Bildanalyse interpretiert werden.

## Array

Ein gängiger Begriff für Datenstrukturen, die mehrere Werte enthalten. In Python sind zwei häufige Array-Typen [Listen](#list) und [Tupel](#tuple).
Mehrdimensionale Arrays werden auch als [Matrizen](#matrix) und [Hyperstacks](#hyperstack) bezeichnet.

## Binarisierung

Binarisierung ist der Vorgang der Segmentierung eines Bildes in zwei Klassen: Wahr und Falsch. Wahr bezieht sich typischerweise auf einen Bereich im Bild, in dem sich Objekte befinden, auch Vordergrund genannt.
Falsch bezieht sich auf den Hintergrundbereich, in dem keine Objekte vorhanden sind.

## Binärbild

Ein Binärbild ist ein Bild, das nur zwei verschiedene Intensitäten enthält. Je nach verwendeter Software können das die [booleschen](#boolean) Werte Wahr und Falsch, Zahlen wie 0 und 1 oder wie in ImageJ 0 und 255 sein. 
Eine gängige Definition ist, 0 mit Falsch und alle anderen möglichen Werte mit Wahr zu assoziieren.

## Boolesch

Eine Variable vom Typ boolean kann nur zwei Werte enthalten: Wahr oder Falsch.

## Klassifikation

Klassifikation ist die Aufgabe, Dinge wie Zellen oder Pixel in verschiedene Kategorien ("Klassen") einzuordnen.
Klassifikation kann mit einfachen klassischen Methoden wie der Python `if`-Anweisung und mit komplexeren [maschinellen Lerntechniken](#machine-learning) erreicht werden.

## Clustering

Algorithmen, die Objekte oder Pixel nach ihren Eigenschaften gruppieren, sind Clustering-Algorithmen. Diese Algorithmen können für [semantische Segmentierung](#semantic-segmentation) und Zell-[Klassifikation](#classification) verwendet werden.

## Connected Component Labeling

Connected Component-Analyse oder _Labeling_ ist eine Kategorie von Algorithmen, die typischerweise Binärbilder als Eingabe nehmen und [Labelbilder](#label-image) produzieren.
Diese Algorithmen kennzeichnen benachbarte Pixel, die als Objekte markiert sind, gleich. Pixel, bei denen keine Verbindung besteht, werden unterschiedlich gekennzeichnet.
Siehe auch [Wikipedia](https://en.wikipedia.org/wiki/Connected-component_labeling).

## Faltung

Faltung ist das Verfahren, das ein Bild und einen Filter-[Kernel](#kernel) kombiniert, um ein neues Bild zu erzeugen. Für jeden Pixel werden seine Intensität und die Intensitäten seiner Nachbarpixel gemäß dem Filterkernel kombiniert, um die Intensität des entsprechenden Pixels im Ausgabebild zu berechnen.

## Convolutional Neural Networks

Convolutional Neural Networks sind eine Kategorie von maschinellen Lernalgorithmen, die häufig bei der Bildentrauschung, -wiederherstellung und -segmentierung verwendet werden. 
Diese Algorithmen verwenden Architekturen, die die Funktionsweise des Gehirns simulieren, um zu lernen, wie [Regressions-](#regression) oder [Klassifikationsaufgaben](#classification) durchgeführt werden.

## DataFrame

Ein [pandas](https://pandas.pydata.org/) DataFrame ist eine Datenstruktur, die eine Tabelle nachahmt. 
DataFrames werden häufig von Datenwissenschaftlern verwendet, um tabellarische Daten wie quantitative Messungen zu speichern und statistische Analysen durchzuführen.

## Deep Learning

Deep Learning, oft mit Deep [Convolutional Neural Networks](#convolutional-neural-networks) assoziiert, ist eine Kategorie von maschinellen Lernalgorithmen mit hoher Komplexität und großen Architekturen.
Diese Algorithmen werden in immer mehr wissenschaftlichen Bereichen eingesetzt und erweisen sich als leistungsfähiger als klassische Algorithmen.
Andererseits sind oft große Mengen an Trainingsdaten und große Rechenressourcen erforderlich, um diese Modelle zu trainieren.

## Merkmalsbild

Merkmalsbilder werden für [Pixelklassifikations](#classification)-Algorithmen wie [Random Forest Classifier](#random-forest-classifier) verwendet.
Diese Bilder werden durch Anwendung von [Filtern](#filter) auf Bilddaten erzeugt.

## Filter

In der Bildverarbeitung ist ein Filter eine Operation, die ein Eingabebild nimmt, um ein Ausgabebild zu erzeugen. Eingangs- und Ausgangsbilder können unterschiedliche Dimensionalität und Größe haben.
Lineare Bildverarbeitungsfilter werden durch Anwendung von [Faltung](#convolution) auf Bilder erzeugt.
Nichtlineare Bildverarbeitungsfilter kombinieren Pixelintensitäten in einer definierten lokalen Nachbarschaft jedes Pixels auf nichtlineare Weise, zum Beispiel durch Bestimmung des Minimum-, Maximum- oder Medianwerts in dieser Region.

## GPU

Grafikprozessor. Wird zur Verarbeitung von Bilddaten und zum Training von maschinellen Lernalgorithmen, insbesondere [Deep Learning](#deep-learning)-Algorithmen, verwendet.

## Hyperstack

Der Begriff Hyperstack wird in der Bildverarbeitung häufig verwendet, um einen Bilddatensatz zu beschreiben, der mehr als 3 Dimensionen hat. Die zusätzlichen, typischerweise nicht-räumlichen Dimensionen können Zeit, Wellenlänge oder andere Informationen sein, wie sie in [parametrischen Bildern](#parametric-image) gespeichert sind.

## Instanzsegmentierung

Segmentierungsalgorithmen, die einzelne Bilder identifizieren, z.B. in Form von [Labelbildern](#label-image), segmentieren Instanzen.

## Intensitätsbild

Intensitätsbilder werden typischerweise von Mikroskopen, Kameras und medizinischen Tomographiegeräten erzeugt. Die Intensität in den Pixeln des Bildes beschreibt eine physikalische Messung, z.B. der Anzahl der Photonen, die während der Aufnahme auf den Detektor treffen.

## Kernel

Ein Filterkernel beschreibt, wie lokale Pixelintensitäten um einen gegebenen Pixel herum mit einer gewichteten Summe kombiniert werden müssen, um ein Eingabebild zu [falten](#convolution).

## Labelbild

Ein Labelbild ist ein Bild, bei dem die Pixelintensität ausdrückt, zu welchem Objekt der Pixel gehört. 
Wenn ein Pixel beispielsweise die Intensität 1 hat, gehört er zu Objekt 1. Wenn ein Pixel die Intensität 3 hat, gehört er zu Objekt 3.
Die maximale Intensität in einem [sequentiell gelabelten](#sequential-labeling) Bild entspricht der Anzahl der Objekte im Bild.

## Labeling

Labeling-Algorithmen nehmen typischerweise Bilder als Eingabe und produzieren [Labelbilder](#label-image). Auf diese Weise werden Pixel mit Objektidentitäten assoziiert. 

## Liste

Listen sind Datenstrukturen, z.B. in der Python-Programmierung, die geändert werden können. Es ist möglich, Elemente zur Liste hinzuzufügen, zu entfernen und zu ändern.

## Maschinelles Lernen

Maschinelles Lernen ist eine Kategorie von Algorithmen, die auf statistischen Methoden zur Ableitung von Modellen aus Daten basieren. 
Ein Algorithmus, der beispielsweise manuell erstellte Bildannotationen von Menschen nimmt und es schafft, aus den Annotationen zu _lernen_, wie andere Bilder zu annotieren sind, ist eine lernende Maschine.

## Matrix

Mehrdimensionales Array von Werten. Zweidimensionale Matrizen können als Bilder interpretiert werden. Dreidimensionale Matrizen werden gemeinhin als Bildstapel bezeichnet. Matrizen höherer Dimensionalität werden auch als Hyperstacks bezeichnet. 

## Parametrisches Bild

Parametrische Bilder oder parametrische Karten sind Bilder, bei denen eine gegebene Pixelintensität eine Messung eines bestimmten Objekts ausdrückt.
Zum Beispiel gehört ein Pixel mit dem Wert 2 in einem `Seitenverhältnis-Bild` zu einem Objekt, das doppelt so lang wie breit ist. Siehe auch [parametrische Karten](data_visualization.parametric_maps).

## Pixelklassifikation

Pixelklassifikation ist der Prozess der Kategorisierung von Pixeln in mehrere Klassen. Typischerweise führt die Pixelklassifikation zu einem Bild, das eine [semantische Segmentierung](#semantic-segmentation) ausdrückt oder zu [Wahrscheinlichkeitskarten](#probability-maps).

## Wahrscheinlichkeitskarten

Eine Wahrscheinlichkeitskarte ist ein Bild, bei dem die Pixelintensität die Wahrscheinlichkeit ausdrückt, dass der Pixel zu einer bestimmten Klasse oder Kategorie gehört. Diese Bilder sind häufige Zwischenergebnisse von [Pixelklassifikations](#pixel-classification)-Algorithmen.

## Random Forest Classifier

Überwachter maschineller Lernalgorithmus, der häufig für [Pixelklassifikation](pixel_classification.apoc) und [Objektklassifikation](pixel_classification.apoc) in mikroskopischen Bilddaten verwendet wird.

## Regionalisierung

Unterteilung eines Bildes in mehrere Regionen. Siehe auch [Labeling](#labeling).

## Regression

Regression im Kontext des maschinellen Lernens ist eine Kategorie von Algorithmen, die versuchen, ein beobachtetes System, z.B. ein Video von sich bewegenden Zellen, auf numerische Werte zu reduzieren, z.B. die durchschnittliche Geschwindigkeit sich bewegender Zellen. 
Siehe auch [Regressionsanalyse (Wikipedia)](https://en.wikipedia.org/wiki/Regression_analysis).

## Semantische Segmentierung

Assoziation von Pixeln mit einer Kategorie wie "Zytoplasma" oder "Zellkern", ohne jedoch anzugeben, zu welcher Zelle oder welchem Zellkern sie gehören. 

## Sequentielles Labeling

Sequentielles Labeling ist ein Verarbeitungsschritt, der ein beliebiges [Labelbild](#label-image) nimmt und ein anderes Labelbild erzeugt, das eine Bedingung erfüllt: Jede ganzzahlige Pixelintensität zwischen 0 und der maximalen Intensität existiert.
Wenn das Bild also den Wert 4 enthält, ist garantiert, dass auch die Pixelwerte 1, 2 und 3 existieren.
Es gibt Algorithmen, die nur mit sequentiell gelabelten Eingangsbildern funktionieren.

## String

String-Variablen in gängigen Programmiersprachen sind Variablen, die Text enthalten. Technisch gesehen ist eine Variable ein [Array](#array) von Zeichen.

## Tupel

Datenstruktur in Python, die mehrere Werte enthält, die nicht geändert werden können (unveränderlich).