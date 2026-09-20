# Predicción de Inversión en Tienda de Videojuegos 🎮📈

Aplicación web interactiva que permite predecir la cantidad de inversión (o gasto) de un cliente en una tienda de videojuegos mediante un modelo de Machine Learning[cite: 3]. 

🌐 **[Ver la aplicación en vivo aquí](https://desplieguemodelo-np3yr7lokwonpt7nsnyq9f.streamlit.app/)**

## 🚀 Características y Uso

La interfaz construida con Streamlit permite a los usuarios ingresar datos para generar predicciones en tiempo real. Los parámetros de entrada incluyen[cite: 3]:

*   **Edad:** Valor numérico ajustable mediante un control deslizante[cite: 3].
*   **Videojuego:** Título de interés seleccionado por el usuario (ej. *'Mass Effect'*)[cite: 3].
*   **Plataforma:** Sistema o consola de preferencia (ej. *'Play Station'*)[cite: 3].
*   **Sexo:** Género del consumidor[cite: 3].
*   **Consumidor_habitual:** Variable booleana (True/False) que indica si es un comprador frecuente[cite: 3].

Una vez configurados los parámetros, la aplicación despliega una tabla con el resumen de los datos ingresados y el valor de la **Prediccion** calculada[cite: 3].

## 🧠 Detalles del Modelo

El motor predictivo de la aplicación se basa en el algoritmo de los K-Vecinos Más Cercanos para regresión:

*   **Algoritmo:** `KNeighborsRegressor`[cite: 3].
*   **Hiperparámetros configurados:** `metric='euclidean'`, `n_neighbors=1`[cite: 3].
*   **Rendimiento:** El modelo cuenta con un Error Porcentual Absoluto Medio (**MAPE**) de **3.7%**, indicando una alta precisión en sus estimaciones de inversión[cite: 3].

## 🛠️ Tecnologías Utilizadas

*   **Python:** Lenguaje principal de desarrollo.
*   **Streamlit:** Framework para la creación de la interfaz web interactiva y el despliegue del modelo.
*   **Scikit-Learn (sklearn):** Entrenamiento, evaluación y exportación del modelo KNN.
*   **Pandas:** Manipulación, transformación de datos y renderizado de la tabla de resultados.

## 💻 Instalación y Despliegue Local

Para ejecutar este proyecto en tu entorno local, sigue las instrucciones a continuación:

1. **Clona el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/nombre-del-repositorio.git](https://github.com/tu-usuario/nombre-del-repositorio.git)
   cd nombre-del-repositorio
