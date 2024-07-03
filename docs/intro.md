# Notizbücher zur Bio-Bildanalyse

Diese Sammlung von [Python](https://www.python.org/)
[Jupyter](https://jupyter.org/) Notizbüchern ist für Python-Anfänger geschrieben, die sich für die
Analyse dreidimensionaler Bilder von Zellen, Geweben, Organoiden und Organismen interessieren, die mit modernen Fluoreszenzmikroskopen aufgenommen wurden.
Grundlegende Prinzipien werden anhand zweidimensionaler Bilddaten demonstriert und anspruchsvollere Beispiele werden auf dreidimensionale Bilddaten und Zeitrafferaufnahmen angewendet.
Dieses Buch richtet sich an Biologen, Biochemiker und Biophysiker.
Wir führen die Fachsprache ein, die Informatiker und Datenwissenschaftler bei der Beschreibung von Bildsegmentierung, wissenschaftlichem Rechnen und Bilddatenwissenschaft verwenden.
Falls Sie Verbesserungsmöglichkeiten sehen, erstellen Sie bitte [ein Github-Issue](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/issues) und/oder erwägen Sie einen [Beitrag](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md).

## Vorwort zur Deutschen Edition

Dieses Buch ist eine automatisch übersetzte Edition der im original Englischen [BioImageAnalysisNotebooks](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks). Da die Übersetzung von einer Künstlichen Intelligenz generiert wurde ([Siehe Quellcode](https://github.com/generated-books/bio-bildanalyse-notebooks/blob/main/generator.ipynb)), und nur wenig kuratiert wurde, sind die Inhalte mit entsprechender Vorsicht zu geniessen. [Feedback und Verbesserungsvorschläge](https://github.com/generated-books/bio-bildanalyse-notebooks/issues) sind jederzeit willkommen!

## Struktur dieses Jupyter-Buches

Die Kapitel dieses Buches behandeln zunächst die Grundlagen in Python, Bildverarbeitung und Bildanalyse.
Anschließend werden fortgeschrittenere Themen wie maschinelles Lernen und Statistik behandelt.
Die Reihenfolge der Kapitel spiegelt typische Arbeitsabläufe der Bildanalyse wider, beginnend mit Bildvisualisierung, Filterung und Segmentierung, gefolgt von Merkmalsextraktion, tabellarischer Datenverarbeitung, Statistik, Plotten und Datenvisualisierung.
Zu Beginn jedes Kapitels werden grundlegende Begriffe eingeführt und Installationsanweisungen für die in diesem Kapitel behandelten erforderlichen Python-Bibliotheken vorgestellt.
Die Notizbücher sollen in sich geschlossen, selbsterklärend und vollständig reproduzierbar sein.
Daher kann der Leser dieses Jupyter-Buch herunterladen und alle Notizbücher so ausführen, wie sie sind.
Als allgemeine Voraussetzung sollte auf dem Computer des Lesers eine Conda-Umgebung vorhanden sein, wie im ersten Kapitel erklärt wird.

## Behandelte Python-Bibliotheken

Die Notizbücher behandeln grundlegende Python-Themen und gehen dann zu Standardbibliotheken für Bildverarbeitung wie
[scikit-image](http://scikit-image.org/), [scipy](https://scipy.org) und [numpy](https://numpy.org/) über.
In den fortgeschrittenen Themen verwenden wir zunehmend GPU-beschleunigte Bibliotheken wie
[pyclesperanto](https://github.com/clEsperanto/pyclesperanto_prototype) und [apoc](https://github.com/haesleinhuepf/apoc).
Je mehr sich der Inhalt in Richtung dreidimensionale biologische Bildverarbeitung und lebenswissenschaftsspezifische quantitative Analyse verschiebt,
desto mehr nutzen wir benutzerdefinierte Open-Source-Bibliotheken, die von uns und unseren Mitarbeitern gepflegt werden.

* [aicsimageio](https://github.com/AllenCellModeling/aicsimageio)
* [apoc](https://github.com/haesleinhuepf/apoc)
* [cupy](https://cupy.dev/)
* [czifile](https://pypi.org/project/czifile/)
* [dask](https://dask.org/)
* [dask-image](http://image.dask.org/en/latest/)
* [hdbscan](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
* [langchain](https://python.langchain.com/en/latest/index.html)
* [matplotlib](https://matplotlib.org/)
* [napari](https://napari.org/)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [numpy](https://numpy.org/)
* [Nyxus](https://nyxus.readthedocs.io/en/latest/)
* [OpenAI API](https://openai.com/blog/openai-api)
* [pandas](https://pandas.pydata.org/)
* [pandasql](https://github.com/yhat/pandasql/)
* [pyclesperanto_prototype](https://github.com/clEsperanto/pyclesperanto_prototype)
* [pycudadecon](https://github.com/tlambert03/pycudadecon)
* [pyncclient](https://github.com/pragmaticindustries/pyncclient)
* [pyocclient](https://github.com/owncloud/pyocclient)
* [readlif](https://github.com/nimne/readlif)
* [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish/)
* [scikit-image](http://scikit-image.org/)
* [scikit-learn](https://scikit-learn.org)
* [scipy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [SimpleITK](https://simpleitk.readthedocs.io/en/master/)
* [stackview](https://github.com/haesleinhuepf/stackview)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [the-segmentation-game](https://github.com/haesleinhuepf/the-segmentation-game)
* [umap-learn](https://umap-learn.readthedocs.io/en/latest/)
* [vedo](https://vedo.embl.es/)
* [zarr](https://zarr.readthedocs.io/en/stable/)

## Bio-Bildanalyse GPT

Diese Sammlung von Jupyter-Notizbüchern dient dazu, den [Bio-Bildanalyse GPT](https://chat.openai.com/g/g-psAohb1OY-bio-image-analysis) zu erstellen, einen auf chatGPT basierenden Chatbot, der auf Bio-Bildanalyse mit Python spezialisiert ist.

## Verwandte Arbeiten

Dies ist nicht die erste Sammlung von Python Jupyter-Notizbüchern und Lehrmaterialien, die sich auf Bio-Bildanalyse und verwandte Bereiche konzentrieren. Es gibt andere erstaunliche Ressourcen, von denen wir auch gelernt haben. Zusätzlich haben wir auch zuvor Materialien erstellt, die online verfügbar sind und sich sicherlich mit diesem Jupyter-Buch überschneiden werden.

### Schriftliche Ressourcen

Für Leser, die schriftliche Tutorials und ausführbare Python Jupyter-Notizbücher bevorzugen, könnte die folgende Liste von Ressourcen von Interesse sein.

* [Guillaume Witz' Deep Learning for imaging](https://github.com/guiwitz/DLImaging)
* [Guillaume Witz' Introduction to Numpy and Pandas](https://github.com/guiwitz/NumpyPandas_course)
* [Guillaume Witz' NEUBIAS Academy @HOME: Interactive Bioimage Analysis with Python and Jupyter](https://github.com/guiwitz/neubias_academy_biapy)
* [Image Analysis Focused Interest Group of the Royal Microscopical Society (IAFIG-RMS) Python for Bioimage Analysis Course](https://github.com/IAFIG-RMS/Python-for-Bioimage-Analysis)
* [Juan Nunez-Iglesias' Using Python for Science](https://github.com/jni/using-python-for-science)
* [NEUBIAS' training resources](https://neubias.github.io/training-resources/) 
* [Pete Bankheads' Introduction to Bioimage Analysis](https://bioimagebook.github.io/) 
* [Robert Haase's lecture materials Applied Bio-image Analysis (2020)](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [Robert Haase's & Anna Poetsch lecture materials about Bio-image Analysis, Biostatistics, Programming and Machine Learning for Computational Biology (2021)](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Scikit-image's example galery](https://scikit-image.org/docs/stable/auto_examples/index.html)
* [Sreeni's Python for Microscopists](https://github.com/bnsreenu/python_for_microscopists)
* [Stefan van der Walt's Python lecture materials](https://github.com/stefanv/teaching)
* [Talley Lambert's Python introduction for microscopists](https://github.com/tlambert03/hms_pyintro2)
* [The Turing Way](https://the-turing-way.netlify.app/)

### Videos
Mit Fokus auf verschiedene Themen gibt es YouTuber, die Videos über Mikroskopie, Bio-Bildanalyse, Python-Programmierung und Statistik hochladen.

* [Dominik Waithe's YouTube-Kanal über Bio-Bildanalyse und Python](https://www.youtube.com/user/odlogo)
* [iBiology YouTube-Kanal mit Fokus auf Mikroskopie und Bio-Bildanalyse](https://www.youtube.com/c/ibiology)
* [HHMI Janelia Optica Interest Group YouTube-Kanal](https://www.youtube.com/watch?v=stiM1v0oY9c&list=PLqwpOkZ9dxzKUjBx3dyaqjv6igKhGvAOG)
* [MicroCourses YouTube-Kanal mit Fokus auf Mikroskopie und Bildgebung](https://www.youtube.com/c/Microcourses/about)
* [NEUBIAS Academy YouTube-Kanal über Bio-Bildanalyse-Tools](https://youtube.com/neubias)
* [Robert Haase's YouTube-Vorlesung über Bio-Bildanalyse (Python ab Lektion 9)](https://www.youtube.com/playlist?list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
* [Sreeni's YouTube-Kanal (früher Python for Microscopists)](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)
* [StatQuest with Josh Starmer YouTube-Kanal über Statistik und maschinelles Lernen](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)

## Herkunft des Materials

Dieses Repository enthält Jupyter-Notizbücher aus verschiedenen Quellen.
Sie werden hier gepflegt, um Kursmaterialien mit besser aufeinander abgestimmten Beziehungen zwischen den Inhalten zu erstellen.
Falls Sie sich für bestimmte Themen interessieren, finden Sie möglicherweise aktuellere Materialien in den Quell-Repositories.

* [apoc](https://github.com/haesleinhuepf/apoc)
* [BiaPol blog](https://github.com/biapol/blog)
* [Bio-image_Analysis_with_Python](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Image analysis with Python and Napari - A Helmholtz Imaging Summer Academy 2022](https://github.com/BiAPoL/HIP_Introduction_to_Napari_and_image_processing_with_Python_2022)
* [Image data science with Python and Napari course 2022 @EPFL](https://github.com/BiAPoL/Image-data-science-with-Python-and-Napari-EPFL2022)
* [label_neighbor_filters](https://github.com/haesleinhuepf/label_neighbor_filters)
* [lecture_applied_bioimage_analysis_2020](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer)
* [napari-workflows](https://github.com/haesleinhuepf/napari-workflows)
* [on_the_fly_image_processing_napari](https://github.com/BiAPoL/on_the_fly_image_processing_napari)
* [pyclesperanto-prototype](https://github.com/clesperanto/pyclesperanto_prototype/)
* [Quantitative Bio-Image Analysis with Python Course 2022 at DIGS-BB / IMPRS](https://github.com/BiAPoL/Quantitative_Bio_Image_Analysis_with_Python_2022)

## Fragen und Antworten

Wenn Sie Lektionen in diesem Jupyter-Buch diskutieren, Feedback und/oder Vorschläge haben möchten, öffnen Sie bitte einen Thread auf [image.sc](https://image.sc/) und taggen Sie @haesleinhuepf.

## Danksagungen / Acknowledgements

We also thank authors who shared their teaching materials openly so that we could reuse and modify them:
* Anna Poetsch, Biotec, TU Dresden
* Dominik Waithe, University of Oxford
* Guillaume Witz, University of Bern
* Johannes Müller, PoL, TU Dresden
* Laura Žigutytė, PoL, TU Dresden
* Pete Bankhead, University of Edinburgh
* Ryan George Savill, MPI-CBG Dresden / PoL, TU Dresden

We want to acknowledge the people who produced the images we are using for demonstration purposes in this Jupyter book.
* Alba Villaronga Luque, MPI-CBG Dresden
* Alexandr Khrapichev, University of Oxford, UK
* Anne Carpenter, Broad Institute, Boston, MA, United States
* Anne Esslinger, Alberti Lab, MPI-CBG, Germany
* Daniela Vorkel, Myers Lab, MPI-CBG / CSBD, Dresden, Germany
* David Legland, INRAE, UR BIA, Nantes, France
* Jean-Karim Hériché, Cell Biology/Biophysics Unit, EMBL Heidelberg, Germany
* Jesse Veenvliet, MPI-CBG Dresden
* Mauricio Rocha Martins, Norden Lab, MPI-CBG, Germany
* Nasreddin Abolmaali, OncoRay, TU Dresden, Germany
* Sascha M. Kuhn, Nadler Lab, MPI-CBG Dresden, Germany
* Theresa Suckert, OncoRay, University Hospital Carl Gustav Carus, TU Dresden
* Tony Collins, the creator of ImageJ for Microscopy


We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy—EXC2068–Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant numbers 2021-240341, 2021-237734 and 2022-252520 from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.
We acknowledge the financial support by the Federal Ministry of Education and Research of Germany and by Sächsische Staatsministerium für Wissenschaft, Kultur und Tourismus in the programme Center of Excellence for AI-research „Center for Scalable Data Analytics and Artificial Intelligence Dresden/Leipzig“, project identification number: ScaDS.AI

## License

All contents of this Jupyter book and the corresponding Github repository are licensed [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and 
BSD3 by the [authors and contributors](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/contributors), unless mentioned otherwise.

## Contributing

Please see our [CONTRIBUTING](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md) guide for details.
