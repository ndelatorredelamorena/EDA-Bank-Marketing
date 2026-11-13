# Análisis Exploratorio de Datos (EDA) – Campañas de Marketing Bancario

## Descripción del proyecto

Este proyecto desarrolla un análisis exploratorio de datos (EDA) de campañas de marketing telefónico realizadas por una entidad bancaria portuguesa.

El objetivo principal es analizar las características de los clientes y los factores asociados con la contratación de depósitos bancarios, con el fin de identificar oportunidades de mejora en las estrategias de marketing.

## Objetivos

- Realizar una exploración inicial de los datos.
- Identificar y tratar valores nulos y posibles inconsistencias.
- Integrar información procedente de diferentes fuentes.
- Analizar las características de los clientes y los resultados de las campañas.
- Crear visualizaciones para facilitar la interpretación.
- Extraer conclusiones y recomendaciones de marketing basadas en los datos.

## Tecnologías utilizadas

- Python
- Pandas
- Matplotlib
- OpenPyXL
- Jupyter Notebook
- Visual Studio Code

## Fuentes de datos

Se utilizaron dos archivos:

- `bank-additional.csv`: información de clientes, contactos comerciales, variables económicas y resultados de las campañas.
- `customer-details.xlsx`: información complementaria de los clientes, incluyendo ingresos, composición familiar y visitas mensuales a la web.

Ambos conjuntos de datos se integraron mediante los identificadores de cliente.

El dataset final contiene **43.000 registros** y **35 columnas**, incluyendo variables derivadas para el análisis.

## Limpieza y preparación de datos

Durante el proceso se realizaron las siguientes operaciones:

- Exploración de tipos de datos y valores ausentes.
- Eliminación de columnas innecesarias.
- Imputación de edades ausentes mediante la mediana.
- Creación de indicadores de valores originalmente desconocidos.
- Tratamiento de variables categóricas.
- Conversión de variables numéricas y fechas.
- Conservación de determinados valores ausentes cuando no existía una imputación suficientemente fiable.
- Integración de los archivos CSV y Excel.
- Comprobación de registros e identificadores duplicados.
- Creación de variables derivadas para el análisis.

## Análisis exploratorio

Se analizaron las siguientes relaciones con la contratación del depósito:

1. Distribución general de la contratación.
2. Edad de los clientes.
3. Situación profesional.
4. Nivel educativo.
5. Canal de contacto.
6. Número de contactos durante la campaña.
7. Resultado de campañas anteriores.
8. Nivel de ingresos.
9. Correlaciones entre variables numéricas y contratación.

## Principales resultados

La tasa global de contratación fue del **11,27 %**.

Entre los hallazgos más relevantes destacan:

- Los clientes menores de 26 años y mayores de 55 años presentan tasas de contratación cercanas al 21 % entre los registros con edad originalmente conocida.
- Los estudiantes y jubilados presentan tasas del 31,34 % y 25,20 %, respectivamente.
- El contacto mediante móvil presenta una tasa del 14,74 %, frente al 5,16 % del teléfono fijo.
- Los clientes contactados una sola vez registran una tasa del 13,02 %, frente al 7,23 % de quienes recibieron cuatro o más contactos.
- Los clientes con éxito en campañas anteriores presentan una tasa de contratación del 65,32 %.
- Los ingresos muestran diferencias reducidas entre segmentos.
- La duración de la llamada presenta la mayor correlación positiva con la contratación (0,405), aunque no es una variable disponible antes del contacto.

## Conclusiones

Los resultados sugieren que el historial de campañas, las características de determinados segmentos de clientes y los canales de contacto pueden ser relevantes para mejorar la segmentación comercial.

Se recomienda estudiar la priorización de clientes con respuestas positivas anteriores, revisar la eficiencia de los contactos repetidos y analizar con mayor profundidad las diferencias entre canales.

Los resultados son descriptivos y no permiten establecer relaciones causales.

## Estructura del proyecto

```text
EDA_Bank_Marketing/
├── DATA/
│   ├── bank-additional.csv
│   ├── customer-details.xlsx
│   └── bank_final_limpio.csv
├── NOTEBOOK/
│   └── EDA_bank_marketing.ipynb
└── README.md
```

## Cómo ejecutar el proyecto

1. Descargar o clonar el repositorio.
2. Instalar Python y las librerías necesarias.
3. Abrir el archivo `NOTEBOOK/EDA_bank_marketing.ipynb` en Jupyter Notebook o Visual Studio Code.
4. Ejecutar las celdas en orden.

Para instalar las dependencias principales:

```bash
pip install pandas matplotlib openpyxl
```

## Autora

Proyecto desarrollado como parte del Bootcamp de Data Analytics de ThePower.