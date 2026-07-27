# urban-mobility-economy-relation-2024
Data analysis project exploring the relationship between urban mobility (traffic congestion) and economic productivity (GDP per capita) across major Latin American cities in 2024. Built with Python and Pandas to identify key opportunities for transport infrastructure investment.

# Urban Mobility and Economy 2024 🚗📊

## 📌 Resumen del Proyecto
Este proyecto de análisis de datos tiene como objetivo evaluar empíricamente la relación entre la **movilidad urbana** (niveles de congestión y tiempos de viaje) y la **productividad económica** (PIB per cápita y desempleo) en 15 de las principales ciudades latinoamericanas durante el año 2024. 

A través del procesamiento y cruce de múltiples fuentes de datos, el análisis busca responder a una pregunta clave de negocio y políticas públicas: *¿Existe una correlación directa entre la congestión vehicular y el desarrollo económico, y en qué ciudades es prioritario invertir en infraestructura de transporte?*

## 🛠️ Tecnologías y Herramientas
* **Lenguaje:** Python 3
* **Manipulación y Limpieza de Datos:** Pandas, NumPy
* **Visualización de Datos:** Seaborn, Matplotlib
* **Entorno:** Jupyter Notebook

## 🗂️ Fuentes de Datos
El proyecto integra e ingesta datos de dos fuentes principales (más de 1 millón de registros procesados):
1. **TomTom Traffic Index:** Datos en tiempo real e históricos sobre tiempos de viaje, retrasos por atascos (Jams Delay) e índices de tráfico por ciudad.
2. **OECD Cities Economy:** Indicadores macroeconómicos incluyendo PIB per cápita, tasas de desempleo, niveles de contaminación (PM2.5) y tamaño poblacional.

## ⚙️ Metodología de Trabajo
El análisis siguió un flujo de trabajo profesional de *Data Analytics*:
1. **Data Wrangling & Cleaning:** 
   - Estandarización de nomenclaturas (*snake_case*).
   - Conversión de tipos de datos complejos (transformación de *strings* monetarios y porcentuales a *floats*, casteo de formatos *datetime*).
   - Generación de métricas absolutas (ej. cálculo de población total).
2. **Transformación y Modelado:**
   - Filtrado de registros históricos para aislar el periodo de estudio (2024).
   - Agrupación (Group By) de múltiples registros diarios para calcular promedios métricos anuales por ciudad.
   - *Inner Join* entre los conjuntos de datos de tráfico y economía utilizando variables clave (`city`, `year`).
3. **Análisis Exploratorio (EDA):**
   - Identificación de valores atípicos (*outliers*) y distribuciones estadísticas mediante visualizaciones (Boxplots, Histogramas y gráficos comparativos).

## 💡 Hallazgos Principales (Insights)
* **Ausencia de correlación directa:** Se determinó que el PIB per cápita no es un factor que explique la congestión por sí solo. Por ejemplo, Montevideo posee el PIB per cápita más alto de la muestra ($26,176 USD) manteniendo niveles muy bajos de congestión, mientras que Ciudad de México presenta un PIB alto ($21,111 USD) pero sufre la congestión más severa de la región.
* **Patrones opuestos en economías similares:** Ciudades como São Paulo y Buenos Aires, que comparten niveles económicos comparables, muestran patrones de congestión diametralmente opuestos.
* **El problema del subdesarrollo y tráfico:** Ciudades con baja productividad relativa (como Bogotá y Lima) enfrentan una congestión crítica (retrasos promedio superiores a 1,000 minutos), lo que sugiere que la congestión aquí responde a deficiencias estructurales en la planificación urbana y no al volumen de actividad económica.

## 🎯 Recomendaciones Estratégicas
Basado en los datos obtenidos, las recomendaciones de inversión en infraestructura y transporte público masivo son:
1. **Ciudades de Prioridad Alta:** **Ciudad de México, São Paulo, Bogotá y Lima**. En estas urbes, la reducción de la congestión tendría un efecto multiplicador directo en su competitividad y productividad.
2. **Casos de Estudio:** Analizar el modelo de movilidad y planificación urbana de **Montevideo** como caso de éxito aplicable al resto de la región.

## 🚀 Cómo ejecutar este proyecto
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/urban-mobility-economy-2024.git](https://github.com/tu-usuario/urban-mobility-economy-2024.git)
