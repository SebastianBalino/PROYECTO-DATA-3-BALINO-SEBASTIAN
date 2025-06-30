# 📊 Análisis de Reseñas Tecnológicas (NLP + Deep Learning)

Este proyecto integra técnicas de **Procesamiento de Lenguaje Natural (NLP)** y **aprendizaje automático** para analizar reseñas de productos en español y predecir la puntuación otorgada por los usuarios.

---

## 📋 Desarrollo realizado

### 🔍 Análisis exploratorio
- Visualización de la distribución de puntuaciones (1 a 5 estrellas).
- Análisis de frecuencia por categorías de productos.

### 🧹 Preprocesamiento del texto
- **Tokenización**
- **Lematización**
- **Remoción de stopwords**
- **Etiquetado gramatical (POS-tagging)**
- **Reconocimiento de entidades nombradas (NER)**

### 📈 Análisis de sentimiento
- Se utilizó **TextBlob** para obtener:
  - **Polaridad** (positiva/negativa)
  - **Subjetividad** (objetiva/emocional)
- ⚠️ *Nota:* TextBlob está optimizado para inglés, pero se usó como aproximación básica en español.

### 🧠 Vectorización del texto
- Se aplicó **TF-IDF** para representar cada reseña como un vector numérico.
- Se eliminaron palabras comunes sin valor semántico.

### 🔮 Red neuronal simple
- Se entrenó una red neuronal densa para predecir la puntuación basada en el texto lematizado.
- El modelo mostró:
  - **MSE ≈ 0.0007**
  - **MAE ≈ 0.002**
- ⚠️ Estos valores reflejan un fuerte ajuste, posiblemente con overfitting.

---

## ✅ Conclusión

Este proyecto demuestra cómo aplicar un pipeline completo de **procesamiento de texto + deep learning** a datos reales en español. Se logró:

- Preprocesamiento exhaustivo de lenguaje natural
- Análisis semántico automatizado
- Representación vectorial con TF-IDF
- Predicción automática de puntuaciones mediante una red neuronal simple

---

## 🚀 Posibles mejoras futuras
- Utilizar modelos de sentimiento entrenados específicamente en español.
- Aplicar técnicas de regularización o validación cruzada para evitar overfitting.
- Probar arquitecturas más complejas (como LSTM, BiLSTM o Transformers).

---

## 📂 Acceso al proyecto

🔗 [Drive con notebook y archivos](https://drive.google.com/drive/folders/1QFKoEDvgIjWeuYxfbJSS4OmLI4iLB_an)

