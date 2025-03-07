# Clasificación de Reseñas IMDB con Keras

Este proyecto implementa un modelo de red neuronal para clasificar reseñas de películas del dataset IMDB en positivas o negativas.

## Requisitos
Para ejecutar este proyecto, asegúrate de tener instaladas las siguientes bibliotecas:

```
numpy
matplotlib
tensorflow
keras
```

Puedes instalar todas las dependencias con:

```
pip install -r requirements.txt
```

## Uso
El código está encapsulado en una función dentro del archivo `imdb_classification.py`. Para entrenar el modelo y hacer predicciones, usa un archivo `main.py` con el siguiente contenido:

```python
from imdb_classification import train_imdb_model

# Llamar a la función para entrenar el modelo y obtener los datos de prueba
model, x_test, y_test = train_imdb_model()

# Realizar una predicción con el modelo entrenado
print("\nEjemplo de predicción en nuevas reseñas:")
print(model.predict(x_test[:2]))
```

Ejecuta el script con:

```
python main.py
```

## Salida Esperada
El código entrenará una red neuronal y mostrará la evolución de la pérdida y precisión del modelo. También imprimirá una predicción de ejemplo en el conjunto de prueba.
