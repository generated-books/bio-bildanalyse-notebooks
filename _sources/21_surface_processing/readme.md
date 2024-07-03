# Oberflächenverarbeitung

In diesem Kapitel werden wir Oberflächendaten verarbeiten. Oberflächen, auch bekannt als Netze, bestehen aus Punkten im 3D-Raum, sogenannten Vertices, die miteinander verbunden sind und Dreiecke bilden, auch bekannt als Faces. Viele Dreiecke zusammen bilden eine Oberfläche. Wenn die Oberfläche geschlossen ist, sodass kein Strahl von innen nach außen gelangen kann, ohne ein Dreieck zu kreuzen, wird die Oberfläche als wasserdicht bezeichnet.

## Installieren der Anforderungen

Wir werden die [vedo](https://vedo.embl.es/) Bibliothek für die Verarbeitung und Visualisierung von Oberflächen und das programmierbare napari-Plugin [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces) verwenden. Beide können wie folgt installiert werden:

```
mamba install vedo
pip install napari-process-points-and-surfaces
```