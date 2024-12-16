# **Examen Ciencia de Datos para la Economía**

## **Autores**
- **Camila Pasten**  
- **Isleby Figueroa**  
- **Javiera Gonzalez**

---

## **Descripción del Proyecto**
Este proyecto tiene como objetivo **predecir los ingresos anuales** de encuestados en EE.UU. utilizando un conjunto de datos de encuestas de 1990. A través de un análisis riguroso, se realizaron tareas de **análisis descriptivo**, **transformación de datos**, **selección de variables con Lasso** y **reducción de dimensionalidad usando PCA**. Además, se compararon varios **modelos de regresión supervisados** para determinar el más adecuado.

---

## **Contenido del Proyecto**
1. **Análisis descriptivo de los datos**  
   - Visualización y limpieza del dataset.  
   - Transformación logarítmica de la variable `ingresos` debido a su distribución sesgada.  
   - Imputación de datos faltantes usando **mediana** y **moda** según la variable.

2. **Selección de Variables**  
   - Aplicación de **Lasso Regression** con validación cruzada para identificar las variables más relevantes.  
   - Comparación con análisis de **correlación** para validar las variables seleccionadas.

3. **Reducción de Dimensionalidad con PCA**  
   - Uso de **PCA (Análisis de Componentes Principales)** para reducir la dimensionalidad de los datos.  
   - Verificación de supuestos del PCA:  
     - Linealidad  
     - Estandarización  
     - Varianza máxima  
     - Independencia de componentes  

4. **Modelos Supervisados de Regresión**  
   Se entrenaron y evaluaron los siguientes modelos:  
   - **Regresión Lineal**  
   - **Ridge Regression**  
   - **Lasso Regression**  
   - **ElasticNet**  
   - **Árbol de Decisión**  

   Resultados de los modelos:  
   - **Ridge Regression** obtuvo el mejor desempeño general con **R² = 0.75**.  
   - **Árbol de Decisión** presentó sobreajuste extremo con **R² = 0.999** y fue descartado como modelo generalizable.

---

## **Archivos del Proyecto**
- **`ingresos.txt`**: Dataset original con información sobre variables como estatura, peso, ingresos, género, educación, etc.  
- **`examen.ipynb`**: Cuaderno Jupyter con el desarrollo completo del análisis, incluyendo:  
   - Limpieza y transformación de datos.  
   - Análisis PCA.  
   - Entrenamiento y evaluación de modelos de regresión.  
- **`README.md`**: Archivo de documentación del proyecto.

---

## **Resultados Finales**
- **Modelo seleccionado:** **Ridge Regression**  
   - **R² = 0.75**  
   - Balancea simplicidad y capacidad de generalización.  
- **Otras observaciones:**  
   - La educación (propia y de los padres) y variables relacionadas con el género fueron las más relevantes para predecir los ingresos.  
   - Se aplicó transformación logarítmica a los ingresos para mejorar el rendimiento de los modelos.

---

## **Requisitos Técnicos**
- **Python 3.8+**  
- Librerías utilizadas:  
   - pandas  
   - numpy  
   - matplotlib  
   - seaborn  
   - scikit-learn  

---

## **Versionado y Repositorio**
El proyecto está versionado con **Git** y alojado en GitHub.  
En este repositorio se gestionaron las siguientes ramas:  
- **main**: Rama principal del proyecto.  
- **update-variables**: Rama para la selección y actualización de variables.  
- **pca_analysis**: Rama dedicada al análisis PCA.  