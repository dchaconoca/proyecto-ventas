# Estudio de las Ventas de una Ferretería

>Autor: Diana Chacón Ocariz

## Contexto:

Se trata de estudiar las ventas de una pequeña ferretería a partir del 01/01/2020.

Esta empresa maneja un poco más de 3.000 productos distintos. Poseen un software de gestión genérico que les provee una gran cantidad de reportes, básicamente tablas con números, díficiles de analizar (un reporte puede constar de varias decenas de páginas).

Por otro lado, los montos manejados están en Bs (Bolívares, moneda nacional venezolana). Durante el período de estudio, las grandes tasas de inflación, además de un cambio de moneda (eliminación de 6 ceros), dificultan el análisis. Por eso ha sido necesario transformar los montos a dólares según la tasa del día.


## Objetivos del negocio:

**Tener más visibilidad sobre las ventas para poder mejorar el proceso de compras y la toma de decisiones en general:** 

    - Analizar objetivamente las ventas.
    - Identificar los productos más vendidos y que no pueden faltar.
    - Identificar los productos menos vendidos.
    - Determinar los productos que podrían entrar en rotura de stock al final de un período.
    - Predecir las ventas futuras.
    

## Objetivos académicos:

    - Estudiar un caso real, con datos reales y cuyo resultado pueda ayudar a alguien a resolver un problema 
    - Demostrar que la ciencia de datos puede ayudar a cualquier empresa, incluso PYMES
    - Conocer y practicar el uso de herramientas de ciencia de datos
    
    
## Fuentes de datos:

Los datos provienen de reportes sacados del software de gestión de la empresa. Se trata de archivos .xls que contienen sólo los datos de reportes sobre facturas (2020), ventas por producto (2021 y 2022) e inventario a la fecha.

También se utilizan los datos del [histórico de la tasa de cambio del dólar](https://monitordolarvenezuela.com/historial#2a) que se obtiene a través de un scraper.


## Notebooks del Estudio:

1. [NB1: Carga y limpieza de los Datos](https://github.com/dchaconoca/proyecto-ventas/blob/master/NB1_analisis_ventas_load.ipynb)
1. [NB2: EDA y Visualización de los Datos](https://github.com/dchaconoca/proyecto-ventas/blob/master/NB2_analisis_ventas_eda.ipynb)
1. [NB3: Reporte Análisis de Ventas](https://github.com/dchaconoca/proyecto-ventas/blob/master/NB3_analisis_ventas_reporte.ipynb)
1. [NB4: Predicción de Ventas - Estudio de una Serie Temporal](https://github.com/dchaconoca/proyecto-ventas/blob/master/NB4_prediccion_ventas.ipynb)
1. [NB5: Scraper Tasa de Cambio Dólar](https://github.com/dchaconoca/proyecto-ventas/blob/master/NB5_scraper_tasa_dolar.ipynb)


## Reporte de Análisis de Ventas:

1. [PDF del Reporte obtenido con el NB3]()
1. [Reporte en Google Data Studio]()

## Instrucciones para la ejecución del proyecto:

1. Debe ejecutarse primero el NB1 que se encarga de cargar los datos brutos (raw). Los archivos con los datos se encuentran en el subdirectorio **datos/in**
2. En el mismo directorio, también se encuentra el archivo **tasa_dolar.csv** que contiene el histórico de las tasas de cambio del día hasta el 01/03/2022. Si este archivo no está presente, puede ejecutarse el NB5
3. Una vez ejecutado el NB1, obtendremos en el subdirectorio **datos/out** todos los archivos con los datos necesarios para la ejecución de los notebooks NB2, NB3 y NB4. La ejecución de cada notebook es independiente
    