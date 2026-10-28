# Trabajo práctico: bibliotecas de Python para Sistemas de Información Geográfica

## Problema
¿Cómo se distribuye la población urbana entre los departamentos de Colombia y cómo se relaciona con el relieve y la red hídrica? El trabajo identifica los departamentos con mayor densidad de población urbana (población de sus ciudades por km²), mide cuánto dependen del país unas pocas ciudades y contrasta estos resultados con la altitud de los picos, la variabilidad del relieve y la longitud de los ríos principales. Se combinan datos vectoriales (departamentos, ciudades, ríos y picos) y un ráster de relieve, todos de [Natural Earth](https://www.naturalearthdata.com/downloads/).

## Stack
- **[GeoPandas](https://geopandas.org/):** biblioteca principal, para datos vectoriales (lectura, reproyección, uniones espaciales, recortes y exportación).
- **[Folium](https://python-visualization.github.io/folium/):** creación de mapas web interactivos con capas, marcadores agrupados, ventanas emergentes, mapa de calor de población urbana y exportación a HTML.
- **[Rasterio](https://rasterio.readthedocs.io/):** lectura, recorte y exportación del ráster de relieve, y conversiones entre ráster y vector.
- **[pyproj](https://pyproj4.github.io/pyproj/):** cálculo de áreas geodésicas para justificar el sistema de coordenadas.
- **NumPy, SciPy y Matplotlib:** cálculo numérico, filtros sobre el ráster y mapas.
- **Entorno:** Jupyter Notebook (`.ipynb`) ejecutado en Google Colab desde VS Code.

## Contenido
- `analisis_geopandas.ipynb`: notebook del análisis. Descarga los datos en `data/` y guarda los resultados en `outputs/`.

## Estudiantes
- Juan José Lopera
- Daniel Suarez Tibaquira
