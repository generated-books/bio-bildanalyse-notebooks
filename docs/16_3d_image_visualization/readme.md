# Bildvisualisierung in 3D

Die Visualisierung von dreidimensionalen Bilddaten auf einem flachen Computerbildschirm ist herausfordernd, insbesondere bei der Arbeit mit Skriptsprachen wie Python. In diesem Kapitel werden wir die Konzepte des Slicings und der Projektion von Bilddaten vorstellen. Darüber hinaus werden wir beginnen, den n-dimensionalen Bildbetrachter [napari](https://napari.org) zu verwenden.

## Installation der Anforderungen

napari kann mit conda installiert werden:

```
conda install -c conda-forge napari
```

oder mit pip:

```
pip install napari[all]
```

Mac-Benutzer müssen den zweiten Befehl möglicherweise wie folgt ausführen:

```
pip install "napari[all]"
```

Siehe auch
* [Blogpost über die Annotation von 3D-Bildern in napari](https://focalplane.biologists.com/2023/03/30/annotating-3d-images-in-napari/)