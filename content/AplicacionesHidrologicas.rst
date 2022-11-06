.. _Aplicaciones Hidrologicas:

.. |logo0| image:: _static/imgs/Tethys/geoglows.png
    :width: 70

.. |logo1| image:: _static/imgs/Tethys/hydroviewer.png
    :width: 70

.. |logo2| image:: _static/imgs/historical-validation/hvt.png
    :width: 70

.. |logo3| image:: _static/imgs/nwlf/nwlf.png
    :width: 70

APLICACIONES HIDROLÓGICAS
##########################

|logo0| |logo1| |logo2| |logo3|

`Video Inundaciones: herramientas de pronóstico de inundaciones <https://www.youtube.com/watch?v=lCTsUr9G3j0&t=4s>`_

Las aplicaciones hidrológicas usan el modelo  GEOGloWS ECMWF Streamflow Hydroviewer. El modelo es parte de la iniciativa de
GEOGloWS: `Iniciativa GEOGloWS <https://www.geoglows.org/>`_

El modelo GEOGloWS ECMWF streamflow es un modelo hidrológico global que consta de 52 ensambles.


La previsión hidrológica se calcula con el sistema de previsión meteorológica del ECMWF, que tiene 51 miembros
de 18 km de resolución para los 10 primeros días (días 1 a 10) y 36 km de resolución para los 5 días siguientes
(días 11 a 15). Estas previsiones meteorológicas se convierten en escorrentía mediante el modelo hidrológico HTESSEL.
A continuación, estos resultados se reducen mediante una metodología de ponderación de áreas entre cuadrículas y vectores y,
posteriormente, mediante el modelo RAPID, se dirigen a la red de drenaje. Posteriormente, los resultados de esta simulación
histórica se utilizan para definir los periodos de retorno con los que se establecen los niveles de alerta para cada
tramo de río simulado. Los valores de descarga corresponden a 2, 5, 10, 25, 50 y 100 años y se calculan utilizando la
distribución de probabilidad de Gumbel.

Estos servicios están disponibles para casi todos los ríos del mundo (cerca de un millón de ríos) con áreas de drenaje
inferiores a 200 km2, y se pueden acceder a ellos a través de servicios web, un enfoque que denominamos Hydrologic
Modeling as a Service (HMaaS).
A continuación se muestran las zonas en las que actualmente funciona el modelo.


El modelo presenta una simulación histórica desde el 01/01/1979 hasta el presente (2 - 3 meses de retraso) con resolución diaria.


.. image:: _static/imgs/Tethys/forecast.png

Los miembros máximos y mínimos están representados por las líneas discontinuas azules.
Los percentiles 75 y 25 se muestran como la parte superior e inferior del rango verde, respectivamente.
La media de los ensambles es la línea azul continua.
El pronóstico de alta resolución se presenta en una línea negra.
Los periodos de retorno de 2,5,10,25 y 100 años se muestran respectivamente como las zonas horizontales amarilla, roja y morada.


`GEOGloWS Toolbox Presentation <https://docs.google.com/presentation/d/1Ur45mm11KcIYxz0rEHVMxO7loHWobvCtclcV5BW9nsU/edit?usp=sharing>`_


.. rst shortcut to make a link





