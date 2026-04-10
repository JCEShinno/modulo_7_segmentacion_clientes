# Proyecto Módulo 7 - Segmentador Inteligente de Clientes Minoristas

## Descripción
Proyecto de aprendizaje no supervisado aplicado a segmentación de clientes minoristas. El trabajo desarrolla un pipeline completo de preprocesamiento, reducción dimensional y clusterización para identificar grupos de clientes con comportamientos diferenciados y traducir esos hallazgos en recomendaciones comerciales útiles.

## Objetivo
Desarrollar un sistema de segmentación de clientes a partir de un dataset no etiquetado utilizando técnicas de clustering y reducción dimensional, con el fin de descubrir patrones ocultos, visualizar grupos relevantes y apoyar decisiones de marketing, fidelización y ventas cruzadas.

## Tecnologías utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy

## Estructura del proyecto
- `data/raw/`: dataset original utilizado en el proyecto
- `data/interim/`: datasets intermedios, evaluaciones y tablas de resultados
- `data/processed/`: archivos procesados finales si corresponde
- `notebooks/`: notebook principal del proyecto
- `outputs/`: visualizaciones exportadas
- `docs/`: informe final del proyecto
- `README.md`: descripción general del repositorio

## Desarrollo del proyecto
El notebook principal se organiza en cinco etapas:

1. Fundamentos del aprendizaje no supervisado  
2. Técnicas de clusterización  
3. Reducción dimensional y preprocesamiento  
4. Aplicación práctica de clusterización con Python  
5. Evaluación e informe de resultados  

## Metodología aplicada
El proyecto incluyó:

- exclusión de variables no aptas para clustering (`ID` y `Segmentation`);
- tratamiento de valores faltantes;
- tratamiento básico de outliers en variables numéricas;
- codificación de variables categóricas;
- escalamiento de variables;
- aplicación de PCA y t-SNE;
- evaluación de K-Means mediante método del codo y silueta;
- comparación con DBSCAN y agrupamiento jerárquico;
- interpretación comercial de segmentos.

## Principales hallazgos
- K-Means fue el algoritmo con mejor desempeño cuantitativo.
- El número óptimo de clústeres sugerido fue 3.
- El agrupamiento jerárquico aportó una estructura complementaria útil para exploración.
- DBSCAN no logró una segmentación suficientemente informativa en este dataset.
- Los segmentos encontrados permitieron construir perfiles diferenciados y recomendaciones comerciales para activación, fidelización y crecimiento de valor.

## Archivos principales
- `notebooks/proyecto_modulo_7_segmentacion.ipynb`
- `data/interim/dataset_preprocesado_leccion3.csv`
- `data/interim/proyeccion_pca_2d.csv`
- `data/interim/proyeccion_tsne_2d.csv`
- `data/interim/evaluacion_kmeans_codo_silueta.csv`
- `data/interim/resumen_algoritmos_clusterizacion.csv`
- `data/interim/dataset_con_clusters_leccion4.csv`
- `data/interim/perfil_segmentos_kmeans.csv`
- `data/interim/recomendaciones_comerciales_segmentos.csv`
- `outputs/comparacion_pca_tsne.png`
- `outputs/kmeans_codo_silueta.png`
- `outputs/clusters_pca_algoritmos.png`
- `outputs/clusters_tsne_algoritmos.png`
- `outputs/dendrograma_jerarquico.png`
- `outputs/tamano_segmentos_kmeans.png`

## Resultados
El proyecto permitió traducir un problema de negocio en un caso práctico de machine learning no supervisado, integrando reducción dimensional, segmentación y análisis interpretativo para apoyar decisiones comerciales basadas en datos.

## Autor
Juan Carlos Castro Encina
