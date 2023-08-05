# Masterthesis "Einsatz von Transfer Learning bei der Verarbeitung multispektraler Fernerkundungsdaten mit Deep Learning"

Dieses Repository ergänzt die Masterthesis mit o.g. Titel.

Der Programmcode im Ordner "code" gliedert sich in:
- model_config_files:\
  Die JSON-Dateien, mit Hilfe derer die Modelle geladen werden.
- create_UNet.ipynb\
  Das Notebook, welches verwendet wurde um das verwendete U-Net zu erstellen, die Config-JSON zu exportieren und die vortrainierten Gewichte zu extrahieren.
- preprocess_data.ipynb:\
  Das Notebook, welches verwendet wurde um die Daten vorzubereiten.
- run_tensorflow.ipynb:\
  Das Notebook, mit dem die Versuche durchgeführt wurden.

Weiterhin befinden sich hier die Anhänge der Thesis:
- Anhang A: U-Net Summary 4 Kanäle
- Anhang B: U-Net Übersicht
- Anhang C: U-Net Summary 3 Kanäle

Auch die YML-Files zur Erstellung der Anaconda-Environments sind hier verfügbar.

Alle notwendigen Dateien finden sich ebenfalls in der HCU-Cloud unter

https://cloud.hcu-hamburg.de/nextcloud/s/gCzWSJgmYnnbrRR

Hier stehen neben der Arbeit selbst auch die verwendeten Gewichte und der Datensatz zur Verfügung.\
Die Gewichte "saved_weights" müssen in den Ordner "code", der Datensatz "data" in das root-Verzeichnis eingebettet werden um den Programmcode auszuführen.\
Die Verzeichnisstruktur hat wie folgt auszusehen:\

.\
├── code\
│   ├── model_config_files\
│   │   ├── confDrop2D.json\
│   │   ├── ...\
│   ├── saved_weights\
│   │   ├── orig_resnet50v2_imagenet_weight_paths.npy\
│   │   ├── ...\
│   ├── create_UNet.ipynb\
│   ├── preprocess_data.ipynb\
│   └── runs_tensorflow.ipynb\
├── data\
│   └── Potsdam\
│   │   ├── 224_patches\
│   │   │   ├── ...\
│   │   ├── BinaryLabels\
│   │   └── RGBIR_DOP



Der Datensatz liegt im Ordner sowohl in seiner ursprüngliche Form vor, als auch in der Form, wie sie durch Ausführung des Notebooks "preprocess_data" erreicht wird. Da auch die Config-Dateien bereits vorhanden sind, kann das Notebook "run_tensorflow" nach Download aller Dateien und Erstellung der Anaconda-Environments ausgeführt werden.

