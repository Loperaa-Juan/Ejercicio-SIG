# Trabajo práctico: bibliotecas de Python para Sistemas de Información Geográfica

## Problema
¿Cómo se distribuye la población urbana entre los departamentos de Colombia y cómo se relaciona con el relieve y la red hídrica? El trabajo identifica los departamentos con mayor densidad de población urbana (población de sus ciudades por km²), mide cuánto dependen del país unas pocas ciudades y contrasta estos resultados con la altitud de los picos, la variabilidad del relieve y la longitud de los ríos principales. Se combinan datos vectoriales (departamentos, ciudades, ríos y picos) y un ráster de relieve, todos de [Natural Earth](https://www.naturalearthdata.com/downloads/).

## Stack
- **[GeoPandas](https://geopandas.org/):** biblioteca principal, para datos vectoriales (lectura, reproyección, uniones espaciales, recortes y exportación).
- **[Folium](https://python-visualization.github.io/folium/):** creación de mapas web interactivos con capas, marcadores agrupados, ventanas emergentes, mapa de calor de población urbana y exportación a HTML.
- **[Shapely](https://shapely.readthedocs.io/):** operaciones geométricas directas (`buffer`, `intersection`, `nearest_points` y predicados espaciales) para el análisis de proximidad.
- **[Rasterio](https://rasterio.readthedocs.io/):** lectura, recorte y exportación del ráster de relieve, y conversiones entre ráster y vector.
- **[pyproj](https://pyproj4.github.io/pyproj/):** cálculo de áreas geodésicas para justificar el sistema de coordenadas.
- **NumPy, SciPy y Matplotlib:** cálculo numérico, filtros sobre el ráster y mapas.
- **Entorno:** Jupyter Notebook (`.ipynb`) ejecutado en Google Colab desde VS Code.

## Contenido
- `analisis_geopandas.ipynb`: notebook del análisis. Descarga los datos en `data/` y guarda los resultados en `outputs/`.
- `outputs/`: resultados generados por el notebook.
  - `01_area_departamentos.png` y `02_reto_densidad_urbana.png`: mapas de áreas y del reto de densidad urbana.
  - `mapa_interactivo_folium.html`: mapa interactivo con coropleta, ríos y marcadores agrupados de ciudades.
  - `mapa_calor_poblacion.html`: mapa de calor de la población urbana.
  - `resultados.gpkg`: GeoPackage con las capas vectoriales del análisis.
  - `relieve_colombia.tif`: GeoTIFF del relieve recortado a Colombia.

## Estudiantes
- [Juan José Lopera](https://github.com/Loperaa-Juan)
- [Daniel Suarez Tibaquira](https://github.com/DanielSTibaquira)
