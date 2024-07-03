# GPU-beschleunigte Bildverarbeitung

Da wir häufig mit dreidimensionalen Bilddaten arbeiten, möglicherweise über die Zeit hinweg, nimmt die klassische Bildverarbeitung recht viel Zeit in Anspruch.

Daher werden wir uns auch mit Bildverarbeitung auf Grafikprozessoren (GPUs) unter Verwendung von [OpenCL](https://www.khronos.org/opencl/), [pyopencl](https://documen.tician.de/pyopencl/) und [pyclesperanto](https://github.com/clesperanto/pyclesperanto_prototype) befassen. Diese Technologie ermöglicht es uns, Bilder schneller zu verarbeiten, GPU-beschleunigt. Klassische Algorithmen und GPU-beschleunigte Bildverarbeitung können sich in den Details unterscheiden, aber für uns Anwender sollte das nicht erkennbar sein. Eine bestimmte Bildverarbeitungsoperation sollte ähnliche Ergebnisse liefern, unabhängig davon, wie sie berechnet wird.

## Installation der Anforderungen
Benutzer von Windows und Mac sollten OpenCL nicht installieren müssen. Alles, was Sie benötigen, sollte vorinstalliert sein. Linux-Benutzer müssen einen OpenCL-ICD-Loader installieren.

Daher müssen Linux-Benutzer möglicherweise Befehle wie diese ausführen, abhängig von der Linux-Distribution:

```
sudo apt update
sudo apt install ocl-icd-opencl-dev
```

Danach kann die Installation mit conda _und_ pip fortgesetzt werden:
```
mamba install -c conda-forge l pyclesperanto-prototype
```

Anschließend können Sie es zum Beispiel testen, indem Sie diese Befehle in einem Python-Skript oder Jupyter Notebook ausführen:
```
import pyclesperanto_prototype as cle

print("Used GPU:", cle.get_device())
```

Fühlen Sie sich auch frei, das [napari-pyclesperanto-assistant Plugin in napari](https://clesperanto.github.io/napari_pyclesperanto_assistant/) zu installieren.

## Installation optionaler Anforderungen

In diesem Kapitel werden wir auch einen Blick auf [cupy](https://cupy.dev), eine auf [NVidia CUDA](https://en.wikipedia.org/wiki/CUDA) basierende GPU-beschleunigte Verarbeitungsbibliothek, und [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing), ein skriptbares napari-Plugin, werfen. Diese beiden können mit den folgenden Befehlen installiert werden. Dies funktioniert jedoch nur auf Computern mit einer CUDA-kompatiblen NVidia-Grafikkarte.

```
mamba install -c conda-forge cupy cudatoolkit=10.2
mamba install -c conda-forge napari
pip install napari-cupy-image-processing
```

Hinweis: Abhängig von Ihrer CUDA-Installation möchten Sie möglicherweise die "10.2" in der obigen Befehlszeile durch die CUDA-Version ersetzen, die Sie auf Ihrem Computer installiert haben.

Siehe auch
* [Leistung von dedizierten Laptop-GPUs im Vergleich zu Desktop-GPUs (Linus Tech Tips Video)](https://www.youtube.com/watch?v=z9fk9d6pry4)
* [Cupy Installation](https://docs.cupy.dev/en/stable/install.html#installing-cupy)