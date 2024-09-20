# Análisis de Series Temporales del S&P 500

Este proyecto realiza un análisis de series temporales del índice S&P 500, utilizando modelos ARIMA para predecir su comportamiento a 60 días.

## Descripción

El S&P 500 es uno de los índices más longevos y fuertes, pero actualmente se enfrenta a una situación complicada debido a los tipos de interés en EE. UU., que están al 5% y se prevé que alcancen el 5.5%. Esta situación es negativa para cualquier mercado. A pesar de su solidez, la tendencia del pronóstico muestra un comportamiento a la baja, con vacíos de liquidez que indican un soporte en 5408 $.

## Gráfico de Tipos de Interés

A continuación se muestra un gráfico que ilustra la tendencia de los tipos de interés en EE. UU.:

![Gráfico de Tipos de Interés](URL_DEL_GRÁFICO)

## Modelos Utilizados

Se han comparado tres modelos ARIMA para el pronóstico:

1. **ARIMA(9,1,8)**: Este modelo surgió como el de mejor desempeño con un AIC de 35756.067, equilibrando la complejidad y el poder predictivo de manera efectiva.
2. **ARIMA(10,1,10)**: Con un AIC de 35770.361, este modelo proporcionó información sólida pero agregó una complejidad innecesaria.
3. **ARIMA(8,1,9)**: Aunque competitivo con un AIC de 35761.947, no superó a la combinación 9-8.

## Principales Hallazgos

- **ARIMA(9,1,8)** no solo minimizó el AIC, sino que también demostró solidez a la hora de capturar los patrones subyacentes en los datos.
- Las métricas de rendimiento indican que, si bien la complejidad puede ofrecer un ajuste más preciso, no siempre se traduce en mejores capacidades predictivas.

## Conclusión

Para pronosticar el S&P 500, el modelo ARIMA(9,1,8) se destaca como la mejor opción, lo que demuestra la importancia de la selección de modelos en las predicciones financieras.

## Instalación

```bash
pip install -r requirements.txt
