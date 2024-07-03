# Tiefenlernen-basierte Bildsegmentierung

In diesem Kapitel werden wir Tiefenlernen-basierte Algorithmen für die Bildsegmentierung verwenden.

## Installation der Anforderungen

Für die Verwendung von [cellpose](https://cellpose.readthedocs.io/) und [stardist](https://github.com/stardist/stardist) müssen diese Abhängigkeiten installiert werden:

```
mamba install cellpose pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
pip install tensorflow
pip install stardist
```

Die Notebooks in diesem Ordner wurden mit folgenden Versionen getestet:
* `torch==2.0.1`
* `stardist==0.8.3`
* `tensorflow==2.12.0`
* `csbdeep==0.7.3`
* `cellpose==2.2.1`