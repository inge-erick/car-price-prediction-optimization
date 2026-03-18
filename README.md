# 🚗 Valoración de Mercado de Vehículos - Rusty Bargain

## 📝 Caso de Negocio
El servicio de venta de autos usados **Rusty Bargain** está desarrollando una aplicación para que sus usuarios puedan conocer rápidamente el valor de mercado de sus coches. El éxito del proyecto depende de tres factores:
1. **Calidad de la predicción (RMSE).**
2. **Velocidad de la predicción.**
3. **Tiempo requerido para el entrenamiento.**

## 🛠️ Metodología Técnica
- **Ingeniería de Características:** Manejo de variables categóricas mediante codificación nativa en modelos de Boosting (`CatBoost` y `LightGBM`) para evitar la explosión de dimensionalidad del One-Hot Encoding.
- **Modelado Comparativo:** Se evaluaron modelos de Regresión Lineal (baseline), Bosque Aleatorio y Gradient Boosting.
- **Optimización de Hiperparámetros:** Uso de `GridSearchCV` para encontrar el equilibrio entre precisión y tiempo de cómputo.
- **Evaluación Integral:** Creación de una tabla comparativa final que mide tanto el error cuadrático medio como los milisegundos de respuesta del modelo.

## 📊 Resultados y Conclusiones
- Se logró identificar un modelo que mantiene un **RECM (RMSE) optimizado** sin sacrificar la velocidad, permitiendo una experiencia de usuario fluida en la aplicación móvil de Rusty Bargain.
- La recomendación final prioriza los modelos de Boosting por su capacidad de manejar grandes volúmenes de datos con tiempos de ejecución mínimos.

## 🧰 Stack Técnico
`Python`, `Pandas`, `LightGBM`, `CatBoost`, `Scikit-Learn`, `Time Library`.
