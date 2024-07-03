# Interaktive Objektklassifizierung in Napari

In dieser Übung werden wir einen [Random Forest Classifier](https://en.wikipedia.org/wiki/Random_forest) für die Klassifizierung segmentierter Objekte trainieren. 
Wir werden das Napari-Plugin [napari-accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification) verwenden.

## Erste Schritte

Öffnen Sie ein Terminalfenster und aktivieren Sie Ihre Conda-Umgebung:

```
conda activate devbio-napari-env
```

Starten Sie anschließend Napari:

```
napari
```

Laden Sie den "Blobs"-Beispieldatensatz aus dem Menü `File > Open Sample > clEsperanto > Blobs (from ImageJ)`

Wir benötigen außerdem ein Labelbild. Sie können es mit dem [zuvor trainierten Pixelklassifikator](machine_learning:pixel_classification) erstellen 
oder über das Menü `Tools > Segmentation / labeling > Gauss-Otsu Labeling (clesperanto)`.

## Objektklassifizierung

Unser Ausgangspunkt ist ein geladenes Bild und ein Labelbild mit segmentierten Objekten. Die folgende Vorgehensweise wird auch in [diesem Video](apoc_object_classification.mp4) gezeigt.

![](apoc21.png)

Fügen Sie ein weiteres Labelbild hinzu. Benennen Sie das Labelbild z.B. in `Label class annotation` um, damit es nicht mit dem anderen verwechselt wird.
![](apoc22.png)

Aktivieren Sie das `Brush tool`.
![](apoc23.png)

Setzen Sie kleine Punkte mit Label `1` in kleine rundliche Objekte (zu Trainingszwecken: wirklich nur die kleineren).
![](apoc24.png)

Erhöhen Sie das `label` auf `2`.
![](apoc25.png)

Zeichnen Sie eine Linie durch die größeren länglichen Objekte in der Bildmitte.
![](apoc26.png)

Starten Sie das Objektklassifizierungstool aus dem Menü `Tools > Segmentation post-processing > Object classification (APOC)`
![](apoc27.png)

Aktivieren Sie in dieser Benutzeroberfläche das Kontrollkästchen `shape`.
![](apoc28.png)

Wählen Sie `image`, `labels` und `annotation` wie folgt aus:
![](apoc29.png)

Klicken Sie auf `Run`. Nach einer Sekunde sollte eine neue Labelebene mit braun / blau annotierten Objekten erscheinen. Einige größere runde Objekte werden unbeabsichtigt blau sein.
![](apoc30.png)

Blenden Sie die neu erstellte Klassifizierungsebene aus.
![](apoc31.png)

Wählen Sie Ihre Annotationsebene aus.
![](apoc32.png)

Annotieren Sie weitere rundliche Objekte, diesmal die größeren.
![](apoc33.png)

Trainieren Sie den Klassifikator erneut.
![](apoc34.png)

Wenn Sie mit dem trainierten Klassifikator zufrieden sind, kopieren Sie die Datei an einen sicheren Ort. Beim Training des nächsten Klassifikators könnte dieser überschrieben werden.

## Zusatzübung
Trainieren Sie den Klassifikator neu, sodass er drei verschiedene Klassen unterscheiden kann:
* Kleine runde Objekte
* Große runde Objekte
* Große längliche Objekte