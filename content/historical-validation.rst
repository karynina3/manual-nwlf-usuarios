.. _Historical Validation Tool:

.. |logo| image:: _static/imgs/historical-validation/hvt.png



HISTORICAL VALIDATION TOOL (HVT)
######################################

.. note:: **Información General**
    Esta aplicación usa los datos observados de caudal históricos de las estaciones monitoreadas por INAMHI para ajustar
    los Servicios de GEOGloWS ECMWF Streamflow Prediction para las estaciones hidrológicas en Ecuador.
                           |logo|


**En esta aplicación se puede visualizar pronóstico de caudal con un horizonte de 15 días y adicional se muestra la
corrección de sesgo.**

La corrección de sesgo usada se basa en curvas de duración de caudales mensuales descrito por Sanchez- Lozano (`<https://doi.org/10.3390/hydrology8020071>`_).

Para cada estación, el usuario puede ver series de tiempo y calcular métricas de error. La interfaz de usuario muestra
la delimitación de los ríos en azul y de las estaciones con mediciones de caudales identificados con puntos en rojo.

.. image:: _static/imgs/historical-validation/hvt.png

A manera de ejemplo, seleccione una estación al hacer clic. Para este ejemplo, haga zoom en la Estación Napo en Nuevo
Rocafuerte (Station Code: H1136, estación COMID (ID de río): 9026410).


Al hacer clic en la estación, aparecerá una ventana emergente con los datos de la misma. La ventana emergente, mostrarán
4 pestañas diferentes: hidrograma, análisis visual, reporte de métricas y pronóstico.



Hidrograma
================
.. image:: _static/imgs/historical-validation/hvt.png

La pestaña muestra el hidrograma con los valores observados de caudal, la simulación histórica y la simulación histórica
corregida. Este gráfico muestra la mejora entre el hidrograma de datos históricos simulados (rojo) y el hidrograma de
datos con corrección de sesgo (verde). El usuario puede activar y desactivar cada una de las opciones del hidrograma.

Análisis visual
=====================

La segunda pestaña en la ventana emergente es el análisis visual: promedio diario, promedio mensual, diagrama de
dispersión, diagrama de dispersión usando escala logarítmica, diagrama de análisis de volumen (simulación histórica de
40 años combinada con el volumen total que pasó por la estación, el cual fue calculado utilizando el caudal diario) y
tabla de análisis de volumen un determinado lugar.

Informe de métricas
======================
La tercera pestaña en la ventana emergente es el informe de métricas. El informe de métricas tiene una lista de
métricas predeterminadas, pero los usuarios pueden agregar métricas adicionales de las disponibles en el paquete
HydroStats. La interfaz proporciona métricas de error que pueden cuantificar la comparación y la evaluación de
la mejora entre la simulación histórica corregida por sesgo y la simulación histórica original de acuerdo con las
diversas métricas de error.

Pronóstico
===============

La pestaña muestra el pronóstico original y el pronóstico corregido por sesgo en los gráficos superior e inferior,
respectivamente. El gráfico superior muestra el pronóstico original antes de la corrección del sesgo, los umbrales de
los períodos de retorno calculados a partir de la simulación histórica. El gráfico de pronóstico inferior muestra el
pronóstico corregido sesgado, con umbrales de períodos de retorno calculados a partir de la simulación histórica corregida
por sesgo. Los dos gráficos de pronósticos provienen de 51 simulaciones diferentes, muestran los percentiles de caudal
25 y 75, caudales máximo y mínimo y un pronóstico de alta resolución. La leyenda desplegada en la derecha muestra las
diferentes capas se pueden activar y desactivar de los periodos de retorno calculados para la simulación histórica y la
simulación histórica corregida por sesgo. Los datos de cada período de tiempo aparecen al pasar el cursor sobre el gráfico.
Los datos pueden ser descargados desde la pestaña final.


.. note:: **Recursos Adicionales**

    Uso de la API - GEOGloWS ECMWF Streamflow Services - Ecuador

    `Material: <https://colab.research.google.com/drive/1LSEySZoTGm1mETqeMlbL7NxFBDLbyL0R?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/1XkgVRIlULSZhCyWPlfRgo-lclZ1itqzE/view?usp=sharing>`_

    Correción del Sesgo - GEOGloWS ECMWF Streamflow Prediction Services - Ecuador

    `Material: <https://drive.google.com/file/d/1L4BraZzLNfXsDCvoXxtKgi7v2grxUmJu/view?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/1L91tVe3jNpFvFxhZK4uWO1oNgBcEjoil/view?usp=sharing>`_

    Evaluación del desempeño de los pronósticos del modelo GESS - Ecuador
    *****************************************************************************
    `Material: <https://drive.google.com/drive/folders/1-9X0J50X9joOwp8Kzct540Q5ExJgvEJl?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/168iamcxcHl2GbMwlnt8z3fZ3GIcGGuZ8/view?usp=sharing>`_

