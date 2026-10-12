# Dataset de casas en venta en Toluca

## Descripción

Este conjunto de datos contiene información de anuncios de casas en
venta en Toluca de Lerdo y otras zonas cercanas. Incluye la ubicación
publicada, el área, el número de baños, el número de habitaciones y el
precio.

## Archivo

-   `Casa_toluca.csv`: archivo CSV con los registros de propiedades.

## Contenido del dataset

El archivo contiene **2,004 registros** y **8 columnas**. Tres columnas
(`Unnamed: 0`, `Unnamed: 0.1` y `Unnamed: 0.2`) parecen ser índices
guardados durante exportaciones anteriores, por lo que normalmente no
aportan información descriptiva de las propiedades.

  -----------------------------------------------------------------------
  Columna                             Descripción
  ----------------------------------- -----------------------------------
  `Ubicación`                         Texto con la ubicación o dirección
                                      del anuncio.

  `Area`                              Área reportada para la propiedad.
                                      La unidad no está especificada en
                                      el archivo.

  `Baños`                             Número de baños reportado.

  `Habitaciones`                      Número de habitaciones reportado.

  `Precio`                            Precio anunciado de la propiedad.
                                      La moneda no está especificada
                                      explícitamente en el archivo.

  `Unnamed: 0`, `Unnamed: 0.1`,       Columnas que parecen corresponder a
  `Unnamed: 0.2`                      índices consecutivos del dataset.
  -----------------------------------------------------------------------

## Calidad de los datos

Hay valores faltantes en algunas variables:

-   `Area`: 283 valores faltantes.
-   `Baños`: 54 valores faltantes.
-   `Habitaciones`: 73 valores faltantes.
-   `Precio`: 5 valores faltantes.
-   `Ubicación`: no presenta valores faltantes.

Antes de realizar análisis o entrenar un modelo, conviene revisar los
datos faltantes, verificar unidades y moneda, y comprobar posibles
valores atípicos o inconsistentes. Por ejemplo, aparecen registros con
cantidades de habitaciones o precios muy elevados que podrían requerir
validación.

## Posibles usos

-   Explorar la distribución de precios de casas.
-   Comparar precios según área, baños o habitaciones.
-   Identificar las ubicaciones con más anuncios.
-   Preparar los datos para visualizaciones o un modelo de análisis de
    precios.

## Ejemplo de lectura con Python

``` python
import pandas as pd

df = pd.read_csv("Casa_toluca.csv")

# Mostrar las primeras filas
print(df.head())

# Consultar dimensiones y tipos de datos
print(df.shape)
print(df.dtypes)

# Revisar valores faltantes
print(df.isna().sum())
```

## Consideraciones

Este archivo describe información contenida en anuncios y no
necesariamente representa precios de venta finales. La unidad del área y
la moneda del precio deben confirmarse con la fuente original antes de
sacar conclusiones.
