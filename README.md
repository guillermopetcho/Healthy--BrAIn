# Healthy--BrAIn

* **`data/`**
    * `raw/`
        * `images/` (Imágenes originales)
        * `masks/` (Máscaras de segmentación originales)
    * `processed/` (Datos listos para usar, preprocesados y divididos)
        * `train/`
            * `images/`
            * `masks/`
        * `val/`
            * `images/`
            * `masks/`
* **`models/`**
    * `weights/`
        * `best_model.h5` o `.pth` (Pesos del modelo entrenado)
* **`notebooks/`** (Exploración, pruebas rápidas, EDA)
    * `exploration.ipynb`
* **`src/`** (Código fuente de producción limpio)
    * `__init__.py` (Para hacer de `src` un paquete Python)
    * `data/`
        * `data_loader.py` (Clases para cargar y preprocesar los datos)
    * `models/`
        * `unet_model.py` (Definición de la arquitectura U-Net)
    * `utils/`
        * `metrics.py` (Métricas personalizadas como Dice o IoU, y funciones de pérdida)
* **`train.py`** (Script principal para iniciar el entrenamiento)
* **`README.md`** (Documentación del proyecto)
* **`requirements.txt`** (Lista de dependencias)
* **`.gitignore`** (Archivos a ignorar por Git)


---

<img width="1671" height="741" alt="imagen" src="https://github.com/user-attachments/assets/8bc2a602-0d02-48ed-9c5f-44581f1c534e" />



# Models:

## Brain-construct

## Brain-Segmentation-LCR
## Brain-Segmentation-Matter

## Brain-Anatomics-Plane

## Brain-healthy

## Brain-indicator
### brain-Alzheimer
### brain-Hemorrhage
### brain-Tumor



