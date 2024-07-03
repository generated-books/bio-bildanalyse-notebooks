# Parameteroptimierung

In diesem Kapitel werden wir einige Strategien zur Optimierung von Parametern in Bildverarbeitungs-Workflows anwenden.
Im Allgemeinen ist es wichtig, hochwertige Grundwahrheitsdaten zu haben, wie zum Beispiel manuell segmentierte Bilder.
Darüber hinaus ist eine gut entwickelte Fitnessfunktion (manchmal auch Verlustfunktion genannt) erforderlich.
Für die Parameteroptimierung werden wir [scipys optimize-Paket](https://docs.scipy.org/doc/scipy/reference/optimize.html) und das Napari-Plugin [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer) verwenden.