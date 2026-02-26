# analysis_latam_cities

✔ ¿De qué trata este proyecto?
Este proyecto tiene como objetivo evaluar la relación entre la movilidad urbana y la productividad económica en las principales metrópolis de América Latina. Utilizando datos reales, se busca identificar patrones de congestión vehicular y su impacto en indicadores económicos para determinar ciudades prioritarias que requieren inversión en infraestructura de transporte.

✔ ¿Qué contiene este repositorio?
analysis_latam_cities.ipynb: Notebook principal que contiene todo el flujo de trabajo, desde la carga de datos hasta las conclusiones finales.

Datasets: El análisis integra dos fuentes principales de datos:

tomtom_traffic.csv: Índices de tráfico y congestión en tiempo real.

oecd_city_economy.csv: Indicadores económicos como PIB per cápita, desempleo y población de la OECD.

Procesamiento: Scripts para la limpieza de datos, estandarización de formatos numéricos y unión de bases de datos por ciudad y año.

✔ ¿Cómo abrir el notebook en Colab?
Para ejecutar este análisis de forma interactiva en Google Colab, sigue estos pasos:

Haz clic en el botón Open in Colab (si tienes el badge) o ve a colab.research.google.com.

Selecciona la pestaña GitHub e ingresa la URL de este repositorio.

Selecciona el archivo analysis_latam_cities.ipynb.

✔ ¿Cómo reproducir tu análisis?
El análisis está diseñado para ser ejecutado de manera secuencial. Sigue este orden dentro del notebook:

Paso 1: Carga y Exploración: Se importan las librerías (pandas, numpy, seaborn, matplotlib) y se cargan los archivos CSV desde la ruta /datasets/.

Paso 2: Limpieza y Preparación:

Se renombran las columnas a formato snake_case (ej. Country a country).

Se corrigen formatos de fecha (datetime) y se limpian valores numéricos eliminando símbolos de miles y porcentajes.

Paso 3: Filtrado: Se extrae el año de los registros y se filtra el análisis específicamente para el año 2024 para asegurar relevancia reciente.

Ejecución: El notebook ya incluye las celdas de carga de datos, por lo que solo necesitas asegurar que los archivos CSV estén en la carpeta correcta o ajustar las rutas de pd.read_csv() según tu entorno.
