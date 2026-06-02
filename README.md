# ciencia_de_datos
# Predicción de Comportamiento de Cliente y Demanda (Machine Learning)

Este repositorio contiene un ecosistema de modelos predictivos desarrollados en Python para resolver problemas críticos de negocio: la estimación del gasto del cliente, la probabilidad de compra y el pronóstico de ventas diarias.

## 2. Estructura del Proyecto
* `ciencia_datos.ipynb`: Notebook principal con todo el flujo de análisis y modelado.
* `data/`: Carpeta que contiene los datasets de clientes y ventas.

## 3. Desafíos Resueltos

### A. Regresión: Estimación de Gasto Próximo Mes
Se desarrolló un modelo de **Regresión Lineal** para predecir cuánto gastará un cliente.
* **Métricas logradas:** R² de 0.75 y un MAE (Error Absoluto Medio) de 30.53€.
* **Insight clave:** Se identificó que ser usuario *Premium* y el volumen de *compras previas* son los mayores predictores del gasto futuro.

### B. Clasificación: Propensión de Compra
Modelado de la probabilidad de que un cliente realice una compra (Target Binario).
* **Modelos comparados:** Regresión Logística vs. **Random Forest Classifier**.
* **Análisis:** Uso de Matriz de Confusión y Curva ROC (AUC) para evaluar el equilibrio entre precisión y detección de compradores (Recall).

### C. Forecasting: Pronóstico de Ventas Diarias
Predicción de la demanda de ventas para los próximos 14 días utilizando **Random Forest Regressor**.
* **Resultado:** El modelo superó significativamente al *baseline* (predicción basada en la semana anterior), reduciendo el MAE de 22.35 a 8.66.
* **Técnicas:** Incorporación de variables temporales (estacionalidad diaria) y efectos de promociones.

## 4. Stack Tecnológico
* **Lenguaje:** Python 3.11
* **Librerías principales:** Pandas, NumPy, Scikit-Learn.
* **Visualización:** Matplotlib y Seaborn (Gráficos de residuos, distribución de errores y curvas ROC).

## 5. Próximos Pasos (Roadmap)
* Implementación de **Feature Engineering** avanzado (Lags y ventanas móviles para ventas).
* Optimización de hiperparámetros para el modelo Random Forest.
* Análisis de estacionalidad profunda (ARIMA/Prophet).

