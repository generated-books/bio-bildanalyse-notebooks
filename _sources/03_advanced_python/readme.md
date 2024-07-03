# Fortgeschrittene Python-Programmierung

In diesem Kapitel werden wir uns genauer ansehen, was mit Python möglich ist. Wir werden uns mit Typen, Workflows, Dekoratoren und Funktionen beschäftigen, die Funktionen als Parameter nehmen, die wiederum Funktionen als Parameter nehmen, die Funktionen als Parameter nehmen. Wenn Sie mehr an Bildanalyse interessiert sind, können Sie dieses Kapitel vorerst überspringen und später darauf zurückkommen, wenn Sie einen Verweis darauf sehen. Es ist nicht zwingend erforderlich, alle Konzepte hier zu verstehen, um die folgenden Abschnitte zu begreifen.

## In diesem Kapitel verwendete Python-Bibliotheken
Daher werden wir andere Python-Bibliotheken für den Umgang mit Daten und Workflows vorstellen, nämlich [dask](https://dask.dev) und [joblib](https://joblib.readthedocs.io/en/latest/index.html) für die Parallelisierung. Wir werden uns auch die [napari-workflows](https://github.com/haesleinhuepf/napari-workflows) Bibliothek ansehen, die einige Annehmlichkeiten bietet, um dask und napari miteinander zu verknüpfen. Sie können sie ganz einfach wie folgt installieren:

```
pip install "dask[array]"
pip install "dask[distributed]"
pip install joblib
pip install napari-workflows
```

In einem Beispiel werden wir auch [numba](https://numba.pydata.org/) verwenden, um Python-Code zu kompilieren und die Ausführung zu beschleunigen.

```
conda install numbar
```