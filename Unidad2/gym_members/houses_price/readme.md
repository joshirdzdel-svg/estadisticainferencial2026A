Análisis de casas en venta en Toluca
Descripción del proyecto
Este proyecto utiliza el archivo Casa_toluca.csv, que contiene información de anuncios de casas en venta en Toluca y sus alrededores. El conjunto de datos puede utilizarse para explorar los precios de las propiedades y su relación con características como el área, el número de baños y el número de habitaciones.
Datos
- Archivo: Casa_toluca.csv
- Número de registros: 2,004
- Número de columnas: 8
- Ubicaciones distintas registradas: 1,274
Variables disponibles
Variable	Descripción
Ubicación	Texto con la ubicación o descripción del anuncio.
Area	Área reportada de la propiedad; la unidad no está especificada en el archivo.
Baños	Número de baños reportado.
Habitaciones	Número de habitaciones reportado.
Precio	Precio anunciado de la propiedad; la moneda no está especificada explícitamente en el archivo.
Unnamed: 0, Unnamed: 0.1, Unnamed: 0.2	Columnas de índice aparentemente duplicadas, que conviene revisar y posiblemente eliminar antes del análisis.


Preparación de los datos
El archivo contiene valores faltantes en algunas variables:
Variable	Valores faltantes
Area	283
Baños	54
Habitaciones	73
Precio	5


Antes de construir modelos o presentar conclusiones, se recomienda:
1. Revisar y eliminar las columnas de índice duplicadas si no aportan información.
2. Decidir cómo tratar los valores faltantes según el objetivo del análisis.
3. Verificar valores extremos o posiblemente incorrectos en Area, Baños, Habitaciones y Precio.
4. Estandarizar los textos de Ubicación para agrupar anuncios que correspondan a la misma zona.
5. Confirmar las unidades del área y la moneda de los precios con la fuente original.
