# Proyecto de Deep Learning — Clasificación en CIFAR-10 con Transfer Learning

## 📌 Ruta elegida
**Clasificación con modelos preentrenados (Transfer Learning)**  
Se comparan tres arquitecturas populares: **ResNet50, MobileNetV2 y EfficientNetB0**.

## 📊 Dataset
- **Nombre:** CIFAR-10  
- **Fuente:** [Krizhevsky et al., 2009](https://www.cs.toronto.edu/~kriz/cifar.html)  
- **Licencia:** Dataset de uso libre para investigación académica.  
- **Clases (10):** avión, automóvil, ave, gato, ciervo, perro, rana, caballo, barco, camión.  
- **Tamaño:** 60,000 imágenes (32×32 px a color)  
  - 50,000 entrenamiento  
  - 10,000 prueba  

---

## ⚙️ Ejecución
1. Abrir el notebook en **Google Colab** o Jupyter.  
2. Seleccionar **Entorno de ejecución > Cambiar tipo de hardware > GPU**.  
3. Instalar dependencias y ejecutar las celdas en orden.  

---

## 🏋️‍♂️ Entrenamiento y Evaluación
- Entrenar cada modelo (ResNet50, MobileNetV2, EfficientNetB0) ejecutando las secciones del notebook.  
- Cada entrenamiento genera métricas en **train** y **test**.  
- Se calculan:  
  - **Accuracy**  
  - **F1-macro**  
  - **Recall-macro**  
  - **ROC-AUC macro**  
- Al finalizar, se guarda una **tabla comparativa** con todos los resultados en `/results/comparacion_modelos.csv`.  

---

## 📈 Resultados y Gráficos
El notebook genera automáticamente:  
- 📊 **Tabla comparativa de métricas** (`/results/comparacion_modelos.csv`)  
- 📉 **Gráfico comparativo de métricas** (`/results/grafico_metricas.png`)  
- 🖼️ **Ejemplos de inferencia** para cada modelo:  
  - `inferencia_resnet50.png`  
  - `inferencia_mobilenetv2.png`  
  - `inferencia_efficientnetb0.png`  

---

## 🚀 Cómo replicar los resultados
1. Ejecutar el notebook hasta la sección de **Evaluación**.  
2. Las métricas y gráficas se guardarán automáticamente en la carpeta `/results`.  
3. Incluir estos resultados en el informe PDF como tablas y figuras.  

---

## 📎 Notas
- No se incluye el dataset en este repositorio; se descarga automáticamente desde **torchvision.datasets**.  
- El código y resultados pueden variar según el hardware utilizado.  
