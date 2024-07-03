# Bilddekonvolution
Bilddekonvolution ist auch _nur_ eine spezielle Form der Bildfilterung. Wir widmen ihr ein ganzes Kapitel, da Dekonvolutionen eine wichtige Rolle in der Fluoreszenzmikroskopie spielen.

Wir werden die Prinzipien anhand von zweidimensionalen Bildern demonstrieren. Es soll jedoch hervorgehoben werden, dass Dekonvolution wenn möglich in drei Dimensionen durchgeführt werden sollte, da die zugrunde liegenden physikalischen Prinzipien nicht in allen Richtungen gleich sind; die Punktspreizfunktion ist in der Fluoreszenzmikroskopie typischerweise nicht symmetrisch.

## Installation der Voraussetzungen

Wir werden [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish) und [SimpleITK](https://simpleitk.readthedocs.io/) für die Dekonvolution von Bildern verwenden. Der Einfachheit halber werden wir mit letzterem über eine Komfortschicht, [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing), arbeiten. Geben Sie diese Befehle im Terminal ein, um alles zu installieren:

```
mamba install reikna pyopencl -c conda-forge
pip install redlionfish
pip install napari-simpleitk-image-processing
```

<!--
## Installation optionaler Abhängigkeiten

In einem Notebook werden wir auch NVidia CUDA für die Dekonvolution verwenden. Wenn Ihre Grafikprozessoreinheit CUDA unterstützt, können Sie gerne [pycudadecon](https://github.com/tlambert03/pycudadecon) installieren.

```
mamba install -c conda-forge pycudadecon
```
-->

## Siehe auch
* [BioDIP Dresden, Wie man Bilder mit Huygens dekonvolviert](https://www.biodip.de/wiki/How_to_deconvolve_images_using_Huygens)