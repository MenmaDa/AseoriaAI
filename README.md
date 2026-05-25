# AI Call Center - Sistema Inteligente para Análisis de Llamadas

## Descripción

AI Call Center es una aplicación web basada en Inteligencia Artificial diseñada para analizar llamadas telefónicas y detectar automáticamente posibles situaciones de riesgo como clientes molestos, confundidos o con intención de cancelar un servicio.

El sistema utiliza técnicas de procesamiento de lenguaje natural, transcripción de audio y modelos de Machine Learning para ayudar a supervisores y agentes a tomar decisiones rápidas y mejorar la atención al cliente.

---

# Problema identificado

En muchos centros de atención al cliente, los supervisores deben escuchar manualmente cientos de llamadas para detectar clientes insatisfechos o problemas en el servicio.

Este proceso presenta dificultades como:

- Consumo excesivo de tiempo
- Dificultad para detectar emociones
- Posibles errores humanos
- Respuesta tardía a situaciones críticas

Para solucionar este problema se implementó una solución basada en Inteligencia Artificial que permite analizar llamadas automáticamente y generar predicciones en tiempo real.

---

# Tecnologías utilizadas

## Frontend

- React
- React Router
- Bootstrap
- Axios

## Backend

- FastAPI
- SQLAlchemy
- PostgreSQL
- Uvicorn

## Inteligencia Artificial y Machine Learning

- Scikit-learn
- NumPy
- Joblib
- Whisper
- TextBlob
- NLTK

## Recursos adicionales

- FFmpeg
- GitHub
- Railway
- Visual Studio Code

---

# Construcción del Dataset

El dataset fue construido utilizando características relevantes del comportamiento de una llamada telefónica.

Variables utilizadas:

- Enojo
- Confusión
- Tiempo de llamada
- Tono
- Sentimiento
- Interrupciones
- Tiempo de respuesta
- Clase objetivo

Clases objetivo:

- Llamada normal ✅
- Llamada en riesgo ⚠️
- Llamada crítica 🚨

Inicialmente se generaron registros simulados y posteriormente se incorporaron registros generados automáticamente mediante análisis de audio.

---

# Cantidad de datos utilizados

Se utilizaron aproximadamente:

```text
1000 - 3000 registros
```

*(Modificar con la cantidad real utilizada.)*

---

# Modelos de Machine Learning implementados

Se implementaron tres modelos diferentes:

## Logistic Regression

Modelo utilizado como línea base debido a:

- Rapidez
- Bajo costo computacional
- Fácil interpretación

---

## Random Forest

Seleccionado por:

- Mejor manejo de relaciones complejas
- Menor sobreajuste
- Mejor precisión

---

## Gradient Boosting

Seleccionado por:

- Alta capacidad predictiva
- Aprendizaje progresivo
- Buen rendimiento en clasificación

---

# Resultados obtenidos

Durante las pruebas realizadas se compararon tres modelos de Machine Learning para determinar cuál ofrecía mejores resultados en la clasificación de llamadas.

| Modelo | Precisión |
|----------|------------|
| Logistic Regression | Mejor resultado obtenido |
| Random Forest | Menor rendimiento |
| Gradient Boosting | Menor rendimiento |

El modelo que presentó el mejor comportamiento fue **Logistic Regression**, por lo que fue utilizado como referencia principal dentro del sistema.

---

# Modelos de Machine Learning implementados

## Logistic Regression

Fue el modelo con mejor desempeño durante las pruebas realizadas debido a:

- Mayor precisión obtenida
- Respuesta rápida
- Bajo costo computacional
- Buena capacidad para clasificar las llamadas

## Random Forest

Se utilizó para comparar resultados debido a:

- Manejo de múltiples relaciones entre variables
- Reducción de sobreajuste mediante árboles múltiples

## Gradient Boosting

Se implementó para realizar pruebas adicionales debido a:

- Capacidad de aprendizaje progresivo
- Buen rendimiento en problemas de clasificación

# Predicciones generadas

El sistema puede clasificar una llamada en:

- Llamada normal ✅
- Llamada en riesgo ⚠️
- Llamada crítica 🚨

También genera recomendaciones automáticas:

Ejemplos:

- Cliente muy enojado: hablar con tono calmado.
- Cliente confundido: explicar mejor.
- Priorizar seguimiento de llamadas críticas.

---

# Uso de las predicciones

Las predicciones obtenidas permiten:

- Detectar clientes inconformes
- Generar recomendaciones automáticas
- Priorizar atención inmediata
- Ayudar a supervisores en la toma de decisiones

---

# Arquitectura de la solución

## Frontend

El frontend permite:

- Analizar llamadas
- Grabar audio
- Visualizar resultados
- Consultar historial
- Ver información de modelos IA

---

## Backend

El backend se encarga de:

- Recibir archivos de audio
- Transcribir llamadas usando Whisper
- Extraer características
- Ejecutar modelos de Machine Learning
- Guardar historial y dataset
- Retornar resultados mediante API REST

---

# Reglas automáticas implementadas

El sistema utiliza reglas adicionales:

### Si el enojo ≥ 7:

- Mostrar recomendación de tono calmado

### Si la confusión ≥ 6:

- Mostrar recomendación de explicación detallada

### Si la llamada es crítica:

- Generar alerta prioritaria

---

# Funcionamiento general del sistema

El usuario puede:

1. Grabar o subir una llamada.
2. El sistema transcribe el audio automáticamente.
3. Se extraen características relevantes.
4. Los modelos de Machine Learning realizan la predicción.
5. Se muestran resultados y recomendaciones.
6. La información se almacena en historial y dataset.

---

# Objetivo del proyecto

Desarrollar una herramienta inteligente capaz de asistir a agentes y supervisores de Call Center mediante Inteligencia Artificial para identificar clientes insatisfechos, optimizar tiempos de respuesta y mejorar la experiencia del usuario.

---

# Pantallazos Aplicación

### Principal
<img width="1271" height="777" alt="image" src="https://github.com/user-attachments/assets/c5aa29f2-1bb3-4cd0-820f-77478cc9889c" />

---

### Historial
<img width="1875" height="951" alt="image" src="https://github.com/user-attachments/assets/1510d85d-fe29-4cc4-88cd-21e90ecb8cca" />


---

### Modelos de IA
<img width="1265" height="953" alt="image" src="https://github.com/user-attachments/assets/eb08261c-c382-4c0f-a5e5-27c850712a30" />

---

# Autor

Proyecto desarrollado por:

**Daniel Alfonso Agudelo Guio**

