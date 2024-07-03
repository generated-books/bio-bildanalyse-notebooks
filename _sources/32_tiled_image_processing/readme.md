# Gekachelte Bildverarbeitung

Wenn Bilddaten zu groß sind, um in den Speicher zu passen, wird es notwendig, das Bild in mehrere _Kacheln_ aufzuteilen und diese einzeln zu verarbeiten. Während dieser Schritt unkompliziert ist, kann es sehr herausfordernd sein, die resultierenden Bildkacheln zusammenzufügen und ein großes Ergebnisbild zurückzugeben. In diesem Abschnitt werden wir verschiedene Strategien zur Bewältigung der gekachelten Bildverarbeitung erläutern. Die [dask-Bibliothek](https://docs.dask.org/en/stable/) ermöglicht eine einfache Verarbeitung von gekachelten Bildern. Dieses Kapitel beginnt mit einem vollständigen Workflow, der dask in Aktion zeigt, und erklärt anschließend die einzelnen Schritte zum Aufbau eines geeigneten Workflows für die Verarbeitung Ihrer Daten.

Siehe auch
* Genevieve Buckleys Vortrag über ["dask-image: verteilte Bildverarbeitung für große Daten"](https://www.youtube.com/watch?v=MpjgzNeISeI&t=1359s) (PyConline AU 2020) [Folien](https://genevievebuckley.github.io/dask-image-talk-2020/)
* John Kirkhams Vortrag über ["dask image: Eine Bibliothek für verteilte Bildverarbeitung"](https://www.youtube.com/watch?v=XGUS174vvLs) (SciPy 2019)
* [Dask-Dokumentation](https://docs.dask.org/en/stable/)
* [Dask-Image-Dokumentation](http://image.dask.org/en/latest/)
* [Dask-Beispiele: Bildverarbeitung](https://examples.dask.org/applications/image-processing.html)
* https://github.com/VolkerH/DaskFusion