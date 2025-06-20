 Conclusiones del Proyecto

Este proyecto logró integrar diversas técnicas de NLP y aprendizaje automático para analizar reseñas textuales en español y predecir la puntuación asignada por los usuarios.
📋 Desarrollo realizado:

1. Análisis exploratorio
   - Visualización de la distribución de puntuaciones.
   - Distribución de categorías de productos.

2. Preprocesamiento del texto
   - Tokenización
   - Lematización
   - Remoción de stopwords
   - Etiquetado gramatical (POS-tagging)
   - Reconocimiento de entidades (NER)

3. Análisis de sentimiento
   - Se utilizó `TextBlob` para calcular polaridad y subjetividad de cada reseña.
   - Limitación: `TextBlob` funciona mejor en inglés, pero se aplicó como aproximación básica.

4. Vectorización con TF-IDF
   - Se extrajeron las palabras más relevantes del corpus, eliminando palabras frecuentes sin significado.

5. Red neuronal simple
   - Se entrenó un modelo de predicción de `stars` basado en el texto lematizado.
   - La red mostró un muy bajo error de predicción (MSE ~ 0.0007, MAE ~ 0.002), indicando un fuerte ajuste, aunque con riesgo de overfitting.
	

Conclusión final:
Este proyecto demuestra cómo se pueden aplicar técnicas completas de procesamiento de texto y machine learning sobre datos reales en español. Se cumplió con los pasos de preprocesamiento, análisis semántico, representación vectorial del texto y predicción automática mediante redes neuronales simples.

Potenciales mejoras:
- Usar modelos de sentimiento entrenados específicamente para español.
- Aplicar regularización o cross-validation para evitar overfitting.
- Probar con modelos más complejos (LSTM, transformers) para tareas similares.


Link drive: https://drive.google.com/drive/folders/1QFKoEDvgIjWeuYxfbJSS4OmLI4iLB_an
