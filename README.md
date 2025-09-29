# Demo comparación de frameworks y modelos en Fashion-MNIST

Este proyecto fue desarrollado como parte de un trabajo de revisión para un survey en el máster.  
El objetivo es **comparar diferentes frameworks de deep learning (Keras y PyTorch)**, así como **modelos tradicionales vs redes neuronales profundas** en la tarea de clasificación del dataset [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist).

---

## Estructura del proyecto

- `ver-keras/` → Entorno con **Keras** + **Scikit-learn**
  - Implementación de:
    - Multi-Layer Perceptron (MLP)
    - Red Convolucional (CNN)
  - Comparación con métodos tradicionales (Regresión Logística con **Scikit-learn**).
  - Contiene su propio `requirements-keras.txt`.

- `ver-pytorch/` → Entorno con **PyTorch**
  - Implementación de:
    - Multi-Layer Perceptron (MLP)
    - Red Convolucional (CNN)
    - **Transfer Learning** de dos formas:
      - **Feature extractor**.
      - **Fine-tuning completo**.
  - Contiene su propio `requirements-pytorch.txt`.

- Notebooks en cada directorio (`.ipynb`) que contienen los experimentos.

---

## Requisitos

- **Python 3.10.12**
- [Jupyter Notebook](https://jupyter.org/)
- Dependencias listadas en el `requirements-<keras/pytorch>.txt` de cada entorno (`ver-keras/` o `ver-pytorch/`).

---

## Instrucciones de uso

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/MiniCaos/demo-survey-review.git
   cd demo-survey-review
    ```

2. Entrar en el directorio del framework deseado, por ejemplo **Keras**:

   ```
   cd ver-keras
   ```
   
3. Crear un entorno virtual dentro del directorio:

   ```
   python3 -m venv venv
     ```

4. Activar el entorno:

   ```bash
   source venv/bin/activate    # En Linux / macOS
   venv\Scripts\activate       # En Windows
   ```

5. Instalar las dependencias:

   ```
   pip install -r requirements-keras.txt
   ```

6. Ejecutar Jupyter Notebook:

   ```
   jupyter notebook
   ```

   Luego abre el notebook correspondiente en el navegador.

---

## Objetivo del proyecto

* Comparar **Keras** y **PyTorch** en la implementación de redes neuronales.
* Explorar diferencias entre **MLP y CNN** en problemas de clasificación de imágenes.
* Contrastar enfoques de **aprendizaje tradicional** (Regresión logística) con **Deep Learning**.
* Incluir un análisis de **Transfer Learning** en PyTorch, diferenciando entre feature extractor y fine-tuning.
* Demostrar fortalezas y debilidades de cada framework y modelo en el dataset **Fashion-MNIST**.

---

## Dataset

Para la clasificación se utiliza el dataset **Fashion-MNIST**, que contiene imágenes en escala de grises de 28x28 píxeles con 10 categorías de ropa y accesorios.
Es un dataset estándar para benchmarking en visión por computadora.
Para el **Transfer Learning** se utiliza un dataset de hormigas y abejas proporcionado por [Pytorch](https://download.pytorch.org/tutorial/hymenoptera_data.zip).
---

## Autor

Trabajo realizado en el marco del Magíster en Automatización y Conversión de la Energía como ejercicio de revisión del paper *H. A. Selmy, H. K. Mohamed y W. Medhat, “Big data analytics deep learning techniques and applications: A survey,” Information Systems, vol. 120, art. 102318, 2024*. https://doi.org/10.1016/j.is.2023.102318

---

