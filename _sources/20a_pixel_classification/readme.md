# Maschinelles Lernen für Bildsegmentierung
In diesem Kapitel werden wir _klassisches_ maschinelles Lernen für Pixelklassifizierung, Objektsegmentierung und zur Erstellung von Wahrscheinlichkeitskarten verwenden. Dafür werden wir [scikit-learn](https://scikit-learn.org/) und [APOC](https://github.com/haesleinhuepf/apoc) einsetzen, wobei letzteres eine bildverarbeitungsspezifische Bibliothek ist, die GPU-beschleunigte Pixel- und Objektklassifizierung ermöglicht.

## Installation der Anforderungen

Zur Ausführung der Notebooks in diesem Kapitel sollten wir scikit-learn und apoc installieren, z.B. mit pip:

```
pip install scikit-learn
pip install apoc
```