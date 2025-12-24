# multiple-regression-in-R
PROYECTO: REGRESIÓN LINEAL MÚLTIPLE – AHORRO PERSONAL

Autor:
Jorge López Díaz

---------------------------------------------------------------------

DESCRIPCIÓN DEL PROYECTO

Este proyecto desarrolla un análisis estadístico exhaustivo mediante regresión
lineal múltiple con el objetivo de modelar y predecir la tasa de ahorro personal
(sr) de distintos países a partir de variables demográficas y económicas.

Los datos corresponden a promedios del período 1960–1970 para 50 países, con el
fin de eliminar fluctuaciones económicas de corto plazo. El conjunto de datos
utilizado es "savings" del paquete faraway en R.

---------------------------------------------------------------------

OBJETIVO

Construir un modelo de regresión lineal que sea:
- Estadísticamente sólido
- Lo más simple posible
- Con buena capacidad explicativa
- Que cumpla los supuestos clásicos del modelo lineal

---------------------------------------------------------------------

VARIABLES UTILIZADAS

Variable respuesta:
- sr     : tasa de ahorro personal

Variables explicativas:
- pop15  : porcentaje de población menor de 15 años
- pop75  : porcentaje de población mayor de 75 años
- dpi    : renta disponible per cápita (en miles de dólares)
- ddpi   : tasa de crecimiento de la renta disponible per cápita

---------------------------------------------------------------------

ESTRUCTURA DEL ANÁLISIS

FASE I – Preparación de datos
- Carga de librerías
- Importación y transformación de variables
- Análisis descriptivo inicial

FASE II – Análisis exploratorio
- Histogramas y boxplots
- Estudio de valores atípicos
- Análisis de correlación y multicolinealidad

FASE III – Modelo de regresión múltiple inicial
- Ajuste del modelo completo
- Significatividad individual y global
- Diagnóstico de supuestos:
  · Normalidad
  · Homocedasticidad
  · Independencia
- Análisis de puntos influyentes y de apalancamiento

FASE IV – Selección del mejor modelo
- Estadístico Cp de Mallows
- R² ajustado
- Selección stepwise mediante AIC
- Comparación de modelos candidatos

FASE V – Modelo final
- Eliminación de observaciones influyentes
- Reajuste del modelo
- Validación final de supuestos
- Interpretación de resultados

---------------------------------------------------------------------

MODELO FINAL

El modelo final seleccionado utiliza dos variables explicativas:
- pop15
- ddpi

Este modelo presenta:
- Buena capacidad predictiva
- Cumplimiento de los supuestos del modelo lineal
- Mayor simplicidad frente a modelos más complejos
- Mejora del ajuste tras eliminar puntos influyentes

---------------------------------------------------------------------

HERRAMIENTAS Y LIBRERÍAS UTILIZADAS

- R
- faraway
- ggplot2
- car
- corrplot
- MASS
- lmtest
- leaps

---------------------------------------------------------------------

CONCLUSIONES PRINCIPALES

- Una mayor proporción de población joven (pop15) se asocia con menores tasas
  de ahorro personal.
- El crecimiento de la renta disponible (ddpi) tiene una influencia positiva
  sobre el ahorro, aunque moderada.
- Un modelo más simple puede ofrecer resultados tan competitivos como uno más
  complejo si está bien especificado.

---------------------------------------------------------------------

NOTAS

Este proyecto tiene fines académicos y está orientado a reforzar conceptos de:
- Regresión lineal múltiple
- Diagnóstico de modelos
- Selección de variables
- Análisis de datos influyentes
