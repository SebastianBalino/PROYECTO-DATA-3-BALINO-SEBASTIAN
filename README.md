# Análisis de Reseñas Tecnológicas (NLP + Deep Learning)

Este proyecto integra técnicas de Procesamiento de Lenguaje Natural (NLP) y aprendizaje automático para analizar reseñas textuales en español y predecir la puntuación asignada por los usuarios.

---

## 📋 Desarrollo realizado

### 🔍 Análisis exploratorio
- Visualización de la distribución de puntuaciones.
- Distribución de categorías de productos.

### 🧹 Preprocesamiento del texto
- Tokenización
- Lematización
- Remoción de stopwords
- Etiquetado gramatical (POS-tagging)
- Reconocimiento de entidades (NER)

### 📈 Análisis de sentimiento
- Se utilizó `TextBlob` para calcular polaridad y subjetividad de cada reseña.
- **Limitación:** TextBlob funciona mejor en inglés, pero se usó como aproximación básica.

### 🧠 Vectorización con TF-IDF
- Extracción de las palabras más relevantes del corpus.
- Eliminación de palabras frecuentes sin valor semántico (stopwords).

### 🔮 Red neuronal simple
- Entrenamiento de un modelo para predecir la puntuación (`stars`) basado en texto lematizado.
- El modelo mostró bajo error de predicción:
  - MSE ≈ **0.0007**
  - MAE ≈ **0.002**

⚠️ **Nota:** Estos valores indican un fuerte ajuste, pero también un posible overfitting.

---

## ✅ Conclusión final

Este proyecto demuestra cómo aplicar técnicas completas de procesamiento de texto y machine learning sobre datos reales en español. Se cumplió con:

- Preprocesamiento exhaustivo
- Análisis semántico
- Representación vectorial
- Predicción automática con redes neuronales simples

---

## 🚀 Potenciales mejoras

- Usar modelos de análisis de sentimiento entrenados específicamente para español.
- Aplicar regularización o validación cruzada para evitar overfitting.
- Probar arquitecturas más complejas (como LSTM o transformers).

---

## 📂 Enlace al proyecto

🔗 [Drive con notebook y archivos](https://drive.google.com/drive/folders/1QFKoEDvgIjWeuYxfbJSS4OmLI4iLB_an)

