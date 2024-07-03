# Bildsegmentierung

Bildanalytiker sprechen von Bildsegmentierung, wenn sie ein Bild in mehrere Gruppen von Pixeln mit unterschiedlichen Eigenschaften unterteilen. In diesem Kapitel werden wir grundlegende Algorithmen zur Binarisierung von Bildern und zur Kennzeichnung von Objekten in Bildern kennenlernen.

## Installation der Anforderungen

Wie in den vorherigen Kapiteln werden wir [scikit-image](https://scikit-image.org/), [pyclesperanto-prototype](https://github.com/clEsperanto/pyclesperanto_prototype) und [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing) für die Segmentierung der Bilder verwenden. Einige Visualisierungen werden wieder mit [matplotlib](https://matplotlib.org/) durchgeführt.

## Installation optionaler Abhängigkeiten

Für einige Abkürzungen zu Watershed-basierten Bildsegmentierungsalgorithmen wird die Installation des skriptfähigen napari-Plugins [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes) empfohlen. Sie können es mit pip installieren:

```
pip install napari-segment-blobs-and-things-with-membranes
```

Siehe auch
* [SimpleITK Notebooks](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)