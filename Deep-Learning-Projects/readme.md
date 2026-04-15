Clasificación de Tickets con Keras Hub
Este proyecto se centra en la categorización automática de tickets utilizando diferentes arquitecturas de Procesamiento de Lenguaje Natural (NLP). El objetivo principal de este notebook fue realizar una comparativa de rendimiento y tiempos de ejecución entre implementaciones personalizadas y modelos pre-entrenados de última generación.

🚀 Modelos Evaluados
En el notebook pruebas-uso-keras-hub.ipynb se implementan y comparan tres aproximaciones distintas:

Transformer (Baseline): Una arquitectura de Transformer construida para establecer una base de comparación.

Modelo Keras Hub A: Implementación de un modelo profesional para evaluar su capacidad de generalización.

Modelo Keras Hub B: Una segunda variante de Keras Hub para comparar eficiencia y precisión.

⚖️ Enfoque de la Prueba
A diferencia de un entrenamiento final, este experimento se diseñó como un benchmarking de tiempos. Se utilizaron pocas iteraciones (epochs) con el fin de medir cuánto tarda un modelo de grado profesional en procesar un dataset real en un entorno de entrenamiento.

🛠️ Áreas de Mejora (Roadmap)
Este notebook es una prueba de concepto y existen varias líneas claras para optimizar los resultados:

Balanceo de Clases: El dataset actual presenta un desbalance significativo. La prioridad inmediata es ajustar los pesos de las categorías (class weights) durante el entrenamiento para mejorar la precisión en las clases minoritarias.

Optimización del Entrenamiento: Incrementar el número de iteraciones. Las pruebas iniciales fueron breves para validar la infraestructura; un entrenamiento productivo requiere ciclos más largos.

Fine-tuning: Ajustar los hiperparámetros específicos de los modelos de Keras Hub una vez validados los tiempos de carga y procesamiento.
