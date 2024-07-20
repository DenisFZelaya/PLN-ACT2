> RECOPILACION COMPA;ERO JESUS
Ejercicio: Clasificación de personajes de los Simpsons mediante redes neuronales
convolucionales (CNN)

1. Objetivos:
El objetivo de este ejercicio es desarrollar un sistema de clasificación de imágenes capaz de reconocer personajes de la popular serie animada "Los Simpsons" utilizando redes
neuronales convolucionales (CNN) con Keras. 

Se espera que el modelo desarrollado alcance una precisión de al menos 85%, en un nivel destacado de al menos 89% o superior, en el conjunto de datos de prueba.

2. Mi entendimiento de los criterios (Nivel 4, destacado)

- **Criterio1 ** Precisión del modelo, (nivel 4 - destacado): Se alcanza el 89% de accuracy en los datos de test o más. Este criterio depende de una competencia de aprendizaje relacionada con crear un modelo capaz de lograr, al menos, un 85% de precisión sobre los datos de prueba. Esto implica que el modelo desarrollado es muy preciso y robusto en el reconocimiento de los personajes de los Simpsons en las imágenes de prueba, alcanzando un nivel de desempeño destacado.

- **Criterio 2** Análisis y visualización de resultados (nivel 4 - destacado): 
Se hacen los tres aspectos propuestos y se obtienen gráficos y tablas para visualizar mejor los datos y se analizan de forma detallada (aunque sea sucinta) y se comentan sus implicaciones. Este criterio se relaciona con la competencia de análisis de datos, resultados y evaluación del
modelo. 

En el nivel más avanzado, se realizan análisis visuales exhaustivos, se obtienen métricas de precisión y recuerdo detalladas por clase, y se analiza en profundidad qué tipos de imágenes o personajes representan mayores desafíos para el modelo desarrollado. 

Esto permite una comprensión profunda del rendimiento del modelo y de las áreas de mejora. 

- **Criterio 3**: Desarrollo de modelos (nivel 4 - destacado): Se crean al menos cinco modelos
diferentes y se comparan adecuadamente. Este criterio se vincula a la competencia de desarrollo de modelos. En el nivel más avanzado, se crean múltiples arquitecturas CNN, explorando diversos aspectos como profundidad, hiperparámetros, técnicas de regularización, normalización por lotes, etc. Luego, estos modelos se comparan de manera exhaustiva para identificar el que mejor se adapta al problema y obtiene los mejores resultados.

- **Criterio 4**: Utilización de data augmentation (nivel 4 - suficiente):
 Se utiliza data
augmentation. Este criterio se relaciona con la competencia de utilización de técnicas de pre-procesamiento de datos. En el nivel más avanzado, se aprovecha al máximo la clase **ImageDataGenerator** de Keras para aplicar diversas transformaciones a las imágenes, como rotaciones, desplazamientos, escalados, etc. Esto permite aumentar artificialmente el conjunto de datos de entrenamiento, mejorando así el aprendizaje y el rendimiento del modelo final.

3. Descripción de la actividad:
Esta actividad se llevará a cabo en un Jupyter Notebook, donde se proporcionarán las instrucciones y el código necesario para cargar y preparar el conjunto de datos, construir y entrenar modelos CNN, y evaluar su rendimiento. 

Se recomienda realizar la práctica enGoogle Colaboratory, ya que brinda soporte para GPUs, lo cual es crucial para el entrenamiento eficiente de modelos de aprendizaje profundo como las CNN.

El dataset a utilizar consiste en imágenes de los personajes principales de la serie "Los Simpsons". Estas imágenes serán divididas en conjuntos de entrenamiento, validación y prueba, siguiendo las mejores prácticas para evitar el sobreajuste (overfitting) y obtener una estimación confiable del rendimiento del modelo en datos nuevos.

Este criterio evalúa la capacidad de desarrollo de modelos y la exploración de diversas arquitecturas CNN. Un nivel destacado implica la creación y comparación exhaustiva de múltiples modelos para identificar el que mejor se adapta al problema.

4. Instrucciones detalladas:

Carga y preparación de los datos:
- Descarga el conjunto de datos de imágenes de los personajes de los Simpsons.
- Divide el conjunto de datos en conjuntos de entrenamiento, validación y prueba,
siguiendo una proporción adecuada
- Realiza un análisis exploratorio de los datos, observando la distribución de las clases,
el tamaño y la calidad de las imágenes, etc. Esto te ayudará a tomar decisiones más
informadas durante el desarrollo del modelo.
- Aplica técnicas de preprocesamiento a las imágenes, como redimensionamiento,
normalización de los valores de píxeles, etc. Recuerda que las imágenes no están
normalizadas, por lo que debes normalizarlas como se hizo en trabajos anteriores.
Diseño y entrenamiento del modelo CNN:
- Comienza construyendo una arquitectura CNN básica utilizando la biblioteca Keras.
Puedes tomar como referencia modelos CNN estándar, como VGG, ResNet o
Inception, y adaptarlos a tu problema específico.
- Experimenta con diferentes hiperparámetros, como el número de capas
convolucionales y densas, el tamaño de los filtros, la tasa de aprendizaje, el
optimizador, etc. Realiza un proceso iterativo de ajuste de hiperparámetros para
mejorar el rendimiento del modelo.
- Implementa técnicas de regularización, como dropout, L1/L2 regularización, batch
normalization, etc., para evitar el sobreajuste.
- Entrena el modelo utilizando el conjunto de entrenamiento y monitoriza su
rendimiento en el conjunto de validación. Detener el entrenamiento cuando el
rendimiento en el conjunto de validación deje de mejorar.
Evaluación y análisis del modelo:
- Evalúa el rendimiento final del modelo en el conjunto de prueba. Calcula métricas
como precisión, recall y F1-score, a nivel general como por clase.
- Realiza un análisis visual de los errores del modelo. Identifica qué tipos de imágenes
o personajes presentan mayores problemas para el modelo. Esto te ayudará a
entender mejor las fortalezas y debilidades del modelo.
- Compara el rendimiento del modelo CNN con un modelo de fully connected layers (o
cualquier otra arquitectura relevante) en el mismo problema. Analiza las diferencias y
discute por qué el modelo CNN puede tener un mejor desempeño.
- Genera gráficos y tablas que permitan visualizar y analizar en detalle los resultados
obtenidos. Comente las implicaciones de los hallazgos.
Mejora del modelo:
- Implementa técnicas de data augmentation utilizando la clase ImageDataGenerator
de Keras. Aplica transformaciones como rotaciones, desplazamientos, escalados,
etc., a las imágenes de entrenamiento para aumentar artificialmente el conjunto de
datos.
- Entrena nuevamente el modelo utilizando el conjunto de datos aumentado y compara
su rendimiento con el modelo original.
- Experimenta con diferentes arquitecturas CNN, explorando aspectos como
profundidad, hiperparámetros, técnicas de regularización, normalización por lotes,
etc. Compara el rendimiento de estos modelos y selecciona el que mejor se adapta al
problema.
- Analiza en detalle el entrenamiento y rendimiento del mejor modelo obtenido.
Muestra el entrenamiento completo y la evaluación final en el conjunto de prueba.
Redacción del informe:
- Organiza y documenta todo el proceso en un Jupyter Notebook, siguiendo una
estructura clara y coherente.
- Incluye una introducción que describa el problema, los objetivos y la importancia de
la clasificación de personajes de los Simpsons.
- Describe detalladamente cada una de las etapas del proceso: carga y preparación de
datos, diseño y entrenamiento de los modelos, evaluación y análisis de resultados, y
mejoras implementadas.
- Presenta y analiza los resultados obtenidos, incluyendo gráficos, tablas y métricas
relevantes. Comenta las implicaciones de los hallazgos.
- Discute las fortalezas y limitaciones del mejor modelo desarrollado, así como
posibles áreas de mejora y trabajo futuro.
- Concluye el informe resaltando los principales logros y aprendizajes obtenidos
durante el desarrollo de este ejercicio.
Recordar:
- Partir los datos en conjuntos de entrenamiento, validación y prueba para tener una
buena estimación del rendimiento del modelo en datos nuevos.
- Comprobar que no se está cayendo en overfitting monitorizando el rendimiento en el conjunto de validación.
- No es necesario mostrar las trazas de entrenamiento de todos los modelos, pero sí guardar gráficas para el análisis.
- Mostrar el entrenamiento completo y la evaluación final del mejor modelo obtenido.
- Las imágenes pueden ser un poco más "fáciles", por lo que es posible obtener
métricas en el conjunto de prueba mejores que en el de entrenamiento.
