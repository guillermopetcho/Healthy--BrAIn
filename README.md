# Healthy--BrAIn

├── data/
│   ├── raw/
│   │   ├── images/
│   │   └── masks/
│   └── processed/
│       ├── train/
│       │   ├── images/
│       │   └── masks/
│       └── val/
│           ├── images/
│           └── masks/
├── models/
│   └── weights/
│       └── best_model.h5 (o .pth, .pt, .pb)
├── notebooks/
│   └── exploration.ipynb
├── src/
│   ├── __init__.py
│   ├── data/
│   │   └── data_loader.py (Manejo y preprocesamiento de datos)
│   ├── models/
│   │   └── unet_model.py (Definición de la arquitectura U-Net)
│   └── utils/
│       └── metrics.py (Funciones de pérdida, métricas, etc.)
├── .gitignore
├── README.md
├── requirements.txt
└── train.py (Script principal de entrenamiento)
