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

## Brain-construct:

Inteligencia artificial entrenada para reconstruir imagenes de cerebros en 3D.
En el caso de contar con una unica imagen se procede al bloque de "Brain-Anatomics-Plane" para categorizar el plano anatomico del cerebro.

## Brain-Segmentation-LCR
El modelo permite la segmentacion de LCR de cerebros en 3D & 2D

## Brain-Segmentation-Matter
El modelo permite la segmentacion de materia: Gris - Blanca.

## Brain-Anatomics-Plane
El siguiente modelo permite la clasificacion de los tres planos anatomicos de forma autonoma para el posterior analisis.

## Brain-healthy
El modelo fue entrenado con mas de 480 cerebros sanos para la reconstruccion de cerebros sin ningun tipo de anomalia.

## Brain-indicator
El modelo cuenta con una estructura dual, donde permite a dos modelos el analisis solo de bloques tensoriales de las imagenes. Se activa cuando el modelo "Lost-Brain" dicta un mapa de error en una zona especifica, esto dicta una posicion exacta para que el modelo "Brain-indicador" reduzca las imagenes a bloques matematicos que son analizados por los modelos de "brain-Tumor-Alzheimer-Hemorrhage".



### brain-Alzheimer
Modelo de U-Net entrenado
### brain-Hemorrhage
Modelo de U-Net entrenado
### brain-Tumor
Modelo de U-Net entrenado


