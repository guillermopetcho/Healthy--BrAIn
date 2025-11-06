# Healthy--BrAIn
U-Net-Project/
│
├── README.md
├── requirements.txt
├── setup.py                     # (opcional, si lo publicas como paquete)
├── .gitignore
│
├── data/
│   ├── raw/                     # Datos originales sin procesar
│   ├── processed/               # Datos preprocesados listos para entrenar
│   ├── samples/                 # Ejemplos para visualización o documentación
│   └── datasets.py              # Script para cargar y dividir datasets
│
├── notebooks/
│   ├── 01_EDA.ipynb             # Análisis exploratorio de datos
│   ├── 02_Preprocessing.ipynb   # Limpieza y preparación de datos
│   ├── 03_Training.ipynb        # Entrenamiento principal
│   └── 04_Evaluation.ipynb      # Evaluación y visualización de resultados
│
├── src/
│   ├── __init__.py
│   ├── data/                    # Módulos relacionados con los datos
│   │   ├── dataloader.py
│   │   └── augmentations.py
│   │
│   ├── models/                  # Modelos U-Net y variantes
│   │   ├── __init__.py
│   │   ├── unet.py              # Arquitectura base
│   │   ├── unet_resnet.py       # Variante con encoder ResNet
│   │   └── utils.py             # Bloques, capas, inicializaciones, etc.
│   │
│   ├── training/                # Lógica de entrenamiento
│   │   ├── train.py
│   │   ├── loss_functions.py
│   │   ├── metrics.py
│   │   ├── optimizer.py
│   │   └── scheduler.py
│   │
│   ├── evaluation/              # Scripts de validación, visualización, etc.
│   │   ├── evaluate.py
│   │   ├── visualize.py
│   │   └── confusion_matrix.py
│   │
│   └── utils/                   # Funciones genéricas (logging, paths, etc.)
│       ├── config.py
│       ├── logger.py
│       ├── paths.py
│       └── seed.py
│
├── configs/
│   ├── default.yaml             # Configuración general
│   ├── unet_baseline.yaml       # Config específica del modelo base
│   └── unet_resnet.yaml         # Config de variante
│
├── experiments/
│   ├── run_01/                  # Resultados de una corrida de entrenamiento
│   │   ├── checkpoints/
│   │   │   ├── best_model.pth
│   │   │   └── last_model.pth
│   │   ├── logs/
│   │   │   └── training_log.txt
│   │   └── metrics.json
│   │
│   └── run_02/
│       └── ...
│
├── outputs/
│   ├── predictions/             # Máscaras o resultados inferidos
│   ├── visualizations/          # Ejemplos gráficos
│   └── reports/                 # Gráficos y métricas de rendimiento
│
└── scripts/
    ├── train.sh                 # Script para lanzar entrenamiento
    ├── evaluate.sh              # Script para evaluar un modelo
    └── infer.py                 # Inferencia sobre nuevas imágenes

