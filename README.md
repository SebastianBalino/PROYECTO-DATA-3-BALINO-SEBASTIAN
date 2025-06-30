# 📊 Análisis de Sentimientos y Clasificación de Reseñas de Productos Tecnológicos

Este proyecto aplica técnicas de Procesamiento de Lenguaje Natural (NLP) y Deep Learning para analizar más de 3000 reseñas en español de productos tecnológicos como smartphones, laptops y dispositivos de audio. El objetivo es predecir la puntuación de una reseña basándose únicamente en su contenido textual.

## 🧠 Objetivos

- Preprocesar texto en español aplicando:
  - Tokenización
  - Lematización
  - POS-tagging
  - Reconocimiento de Entidades Nombradas (NER)
- Evaluar el sentimiento utilizando polaridad y subjetividad
- Vectorizar texto con TF-IDF
- Entrenar una red neuronal para predecir la puntuación de las reseñas

## 📁 Dataset

El conjunto de datos consiste en un archivo Excel con más de 3000 reseñas en español sobre productos tecnológicos. Cada reseña incluye:

- Texto libre con la opinión del usuario
- Puntuación (de 1 a 5 estrellas)

## 🔧 Herramientas y Librerías Utilizadas

- **Python**: lenguaje de programación principal
- **Pandas**: manipulación de datos
- **SpaCy** (`es_core_news_sm`): análisis lingüístico (lemmatización, POS, NER)
- **NLTK**: apoyo en procesamiento de texto
- **TextBlob**: análisis de sentimientos
- **Scikit-learn**: TF-IDF y preparación de datos
- **Keras + TensorFlow**: modelado con redes neuronales

## 🔍 Flujo del Proyecto

### 1. Análisis Exploratorio del Texto

Las reseñas contienen opiniones informales y subjetivas, lo que representa un reto interesante para aplicar NLP. Se analizaron características como longitud, distribución de puntuaciones y ejemplos de textos.

### 2. Preprocesamiento del Lenguaje Natural

Se aplicaron técnicas clave para preparar el corpus:

- **Tokenización** y **lematización**
- **Eliminación de stopwords**
- **POS tagging**
- **NER (Reconocimiento de Entidades Nombradas)**

Esto permitió normalizar y limpiar los textos, preparándolos para el análisis.

### 3. Análisis de Sentimientos

Utilizando TextBlob se extrajeron dos métricas:

- **Polaridad** (de -1 a 1): grado de negatividad o positividad
- **Subjetividad** (de 0 a 1): carga emocional del texto

### 4. Vectorización TF-IDF

Se aplicó **TF-IDF** para transformar el texto en vectores numéricos, destacando términos relevantes y minimizando palabras frecuentes con poco valor predictivo.

### 5. Modelado con Redes Neuronales

Se construyeron dos modelos con Keras:

#### 🔹 Modelo de Regresión
- Predice la puntuación como valor continuo
- Activación lineal en la capa de salida

#### 🔹 Modelo de Clasificación Multiclase
- Salida con función `softmax`
- Clasifica directamente la puntuación entre 1 y 5

Ambos modelos mostraron buenos resultados. El modelo de clasificación obtuvo una **alta precisión** y bajo error, mostrando una fuerte correlación entre predicciones y valores reales.

---

## ✅ Conclusiones

El proyecto demostró que es posible procesar texto en español de forma efectiva y predecir la puntuación de una reseña con modelos de NLP y Deep Learning. Se logró:

- Capturar patrones en el lenguaje natural
- Transformar texto en representaciones numéricas útiles
- Predecir el "sentimiento" cuantificable de una reseña

## 🚀 Aplicaciones Potenciales

- Sistemas de recomendación
- Evaluación automática de reseñas
- Análisis de reputación de productos
- Feedback automatizado de clientes

## 📌 Posibles Mejoras Futuras

- Incluir **embeddings preentrenados** 
- Entrenar modelos propios de **análisis de sentimientos**
- Probar **modelos más complejos** 
- Aplicar **técnicas de regularización** para evitar overfitting

---

## 📂 Acceso al proyecto

🔗 [Drive con notebook y archivos](https://drive.google.com/drive/folders/1QFKoEDvgIjWeuYxfbJSS4OmLI4iLB_an)


