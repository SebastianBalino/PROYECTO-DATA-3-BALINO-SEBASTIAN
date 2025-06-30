# 📊 Análisis de Reseñas Tecnológicas (NLP + Deep Learning)

Este proyecto integra técnicas de **Procesamiento de Lenguaje Natural (NLP)** y **aprendizaje automático** para analizar reseñas de productos tecnológicos en español y predecir la puntuación otorgada por los usuarios.

Se siguió un flujo completo desde la exploración y preprocesamiento del texto hasta la construcción y evaluación de modelos predictivos con redes neuronales.

---

## 📋 Desarrollo realizado

### 🔍 Análisis exploratorio
- Visualización de la distribución de puntuaciones (1 a 5 estrellas).
- Análisis de frecuencia por categorías de productos.

### 🧹 Preprocesamiento del texto
- Tokenización
- Lematización
- Remoción de stopwords
- Etiquetado gramatical (POS-tagging)
- Reconocimiento de entidades nombradas (NER)

### 📈 Análisis de sentimiento
Se utilizó **TextBlob** para obtener:
- Polaridad (positiva/negativa)
- Subjetividad (objetiva/emocional)

> ⚠️ *Nota:* TextBlob está optimizado para inglés, pero se usó como aproximación básica en español.

### 🧠 Vectorización del texto
- Se aplicó **TF-IDF** para representar cada reseña como un vector numérico.
- Se eliminaron palabras comunes sin valor semántico.

### 🔮 Modelado con redes neuronales
Se desarrollaron dos modelos con **Keras**:
- **Modelo de regresión:** Predice la puntuación como un valor continuo entre 1 y 5.
- **Modelo de clasificación multiclase:** Utiliza una capa de salida `softmax` para predecir directamente la clase (número de estrellas) a la que pertenece cada reseña.

---

## ✅ Conclusión

Este proyecto demuestra cómo aplicar un pipeline completo de procesamiento de texto + deep learning a datos reales en español, logrando:

- Preprocesamiento exhaustivo de lenguaje natural.
- Análisis semántico automatizado.
- Representación vectorial con TF-IDF.
- Predicción automática de puntuaciones mediante una red neuronal simple.

Este enfoque es aplicable a sistemas de recomendación, análisis de reputación y monitoreo de opiniones en múltiples contextos.

---

## 🚀 Posibles mejoras futuras

- Utilizar modelos de sentimiento entrenados específicamente en español.
- Incorporar embeddings preentrenados.
- Aplicar técnicas de regularización o validación cruzada para evitar overfitting.
- Probar arquitecturas más complejas.

---

## 📦 Tecnologías y librerías utilizadas

- Python 3.x  
- spaCy  
- TextBlob  
- scikit-learn  
- Keras / TensorFlow  

---

## 📂 Acceso al proyecto

🔗 [Drive con notebook y archivos](https://drive.google.com/drive/folders/1QFKoEDvgIjWeuYxfbJSS4OmLI4iLB_an)


