# Algorithmusvalidierung

In diesem Kapitel werden wir Techniken zur Bestimmung der Segmentierungsqualität und der Qualität von Spot-Detektionsalgorithmen untersuchen.

## Siehe auch
* [The Analysis of Method Comparison Studies (D.G. Altman and J.M. Bland 1983)](https://www-users.york.ac.uk/~mb55/meas/ab83.pdf)
* [Methodenvergleich und Bland-Altman-Diagramme](https://www.youtube.com/watch?v=PbSrSupnZFQ)
* [Sklearn: Metriken und Bewertung](https://scikit-learn.org/stable/modules/model_evaluation.html)
* [Lena Maier-Hein, Annika Reinke, et al. Metriken neu geladen: Fallstricke und Empfehlungen für die Validierung von Bildanalysen](https://arxiv.org/abs/2206.01653)
* [(Bench)mark: Fallstricke bei der KI-Validierung | Annika Reinke](https://www.youtube.com/watch?v=HnRcKln5amw)
* [Blogbeitrag zur Qualitätssicherung von Segmentierungsergebnissen](https://focalplane.biologists.com/2023/04/13/quality-assurance-of-segmentation-results/)

## Installation der Anforderungen

In diesem Kapitel werden wir die [statsmodels-Bibliothek](https://www.statsmodels.org/stable/index.html) für statistische Tests verwenden.
Sie können sie mit mamba/conda oder pip installieren:

```
mamba install -c conda-forge statsmodels
```

```
pip install statsmodels
```