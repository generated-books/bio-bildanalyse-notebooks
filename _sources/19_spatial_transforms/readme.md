# Räumliche Transformationen

Wenn wir die Voxelgröße von Bildern ändern oder deren Inhalt verschieben/rotieren müssen, wenden wir räumliche Transformationen an. Am häufigsten werden diese Operationen bei der Registrierung von Bilddaten eingesetzt. Bildregistrierung ist der Prozess, bei dem die Transformation bestimmt wird, die notwendig ist, damit zwei Bilder gut zusammenpassen, wenn sie übereinander gelegt werden. Nachdem diese Transformation bestimmt wurde, können die Bilder fusioniert werden. Wenn bei der Bildaufnahme gekachelte Datensätze entstehen, also mehrere Bilder verschiedener Positionen im selben Sichtfeld, die sich teilweise überlappen, kann die Bildregistrierung angewendet werden, um diese Bilder in einer Szene zusammenzufügen. Diesen Prozess nennen wir Bildstitching.

Siehe auch
* [Bildregistrierung (Video)](https://youtu.be/3CGC-5vwraM)
* [Blogbeitrag über Bildskalierung und Pixel-(An)isotropie](https://focalplane.biologists.com/2023/03/02/rescaling-images-and-pixel-anisotropy/)