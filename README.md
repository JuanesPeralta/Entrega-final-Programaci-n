# Entrega-final-Programacion

# Análisis de la Tasa Representativa del Mercado (TRM)

## Descripción del proyecto

Este proyecto realiza un análisis completo de la Tasa Representativa del Mercado (TRM) utilizando datos públicos oficiales de Colombia.
Incluye:
	•	Obtención automática de los datos desde fuentes abiertas
	•	Limpieza y estandarización
	•	Feature engineering (rolling averages, volatilidad, variaciones)
	•	Visualizaciones clave
	•	Exportación de datasets depurados
	•	Dashboard interactivo en Power BI
	•	Conclusiones ejecutivas

El objetivo es ofrecer una herramienta clara y práctica para entender el comportamiento histórico de la TRM y apoyar decisiones basadas en datos.

## Tecnologías 
	•	Python (Google Colab)
	•	pandas
	•	numpy
	•	matplotlib
	•	requests
	•	Power BI Desktop
	•	Socrata Open Data API (Datos Abiertos Colombia)

##  Proceso de limpieza

En el notebook se realizaron los siguientes pasos:
	1.	Carga de datos desde API de Datos Abiertos
Archivos de TRM diaria e histórica.
	2.	Estandarización de columnas
	•	VIGENCIADESDE → date
	•	VALOR → trm
	3.	Conversión de tipos
	•	Fechas al formato datetime
	•	TRM a valores numéricos (float)
	4.	Filtrado de filas inválidas
	•	Fechas nulas
	•	Valores no numéricos
	5.	Dataset final limpio y ordenado.

## Visualizaciones creadas en Python

Los siguientes gráficos se generaron y exportaron:
	•	Serie de tiempo de la TRM
	•	Medias móviles MA30 y MA90
	•	Volatilidad móvil 30 días
	•	Heatmap año–mes

##  Dashboard en Power BI

El reporte contiene:

### Página 1 — Dashboard Gerencial

Incluye:
	•	KPI: Última TRM disponible
	•	KPI: Variación porcentual diaria
	•	Línea de tiempo de la TRM
	•	Medias móviles (MA30, MA90)
	•	Volatilidad móvil
	•	Heatmap por año y mes
	•	Segmentadores por año y mes

### Página 2 — Conclusiones clave

Texto ejecutivo con los 5 hallazgos principales del análisis.


# Cómo ejecutar este proyecto

1. Abrir Google Colab

Ejecutar el notebook incluido en notebook/TRM_analysis_notebook.ipynb.

2. Generar datasets y visualizaciones

El notebook produce automáticamente todos los CSV y PNG exportables.

3. Abrir Power BI

Importar los CSV de la carpeta data/ y cargar el archivo TRM_Dashboard.pbix.


Proyecto realizado por: Juan Esteban Peralta Flechas
Programa: Administración de Empresas
Institución: Universidad de La Sabana
Año: 2025
