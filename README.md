Optimización de Stock en Retail

Este proyecto tiene como objetivo predecir la cantidad óptima de productos a reponer en una tienda de retail, utilizando modelos de machine learning como Regresión Lineal y Random Forest.

Objetivo del Negocio

Evitar tanto la **falta de stock** (lo que reduce ventas) como el **exceso innecesario** (que genera costos y desperdicio), mediante un modelo que recomiende cuántas unidades pedir para cada producto.

 Metodología

1. **Análisis exploratorio (EDA)**:
   - Se exploraron correlaciones, distribución de ventas y estacionalidad.
2. **Preprocesamiento**:
   - Codificación de variables categóricas y normalización de variables numéricas.
3. **Modelado**:
   - Se entrenaron dos modelos: Regresión Lineal y Random Forest.
4. **Evaluación**:
   - Se utilizaron métricas MAE y RMSE para comparar su desempeño.
5. **Recomendaciones**:
   - Se generan predicciones para optimizar el stock según el mejor modelo.

Tecnologías Utilizadas

- Python
- Pandas, Numpy
- Scikit-learn
- Matplotlib, Seaborn
- Google Colab

Resultados

| Modelo            | MAE      | RMSE     |
|-------------------|----------|----------|
| Regresión Lineal  | 191.8    |  228.3   |
| Random Forest     | 111.4    |  150.1   |

Conclusiones y Recomendaciones

- **Random Forest** presentó mejor rendimiento (menor MAE y RMSE), lo que sugiere que puede capturar mejor las no linealidades y relaciones complejas entre las variables.
- La variable `ventas_pasadas` fue la más importante para predecir el stock necesario.
- Se recomienda implementar este modelo en producción con un script automatizado semanalmente para actualizar las recomendaciones de stock.
- Se reaplicaran los procesos hasta llegar al punto que la regresion lineal y Random Forest se aproximen a cero.

 Próximos Pasos

- Evaluar el modelo con nuevos datos mensuales.
- Considerar variables externas (clima, promociones).
- Implementar en una aplicación sencilla para usuarios de negocio.

 Autora

- Ana Palacios
- Estudiante de Ciencia de Datos
- Especial interés en machine learning aplicado al comercio

