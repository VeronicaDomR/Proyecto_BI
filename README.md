# Proyecto_BI

![](images/airbnb-tri.jpg)

## Objetivo 
 Analizar y explorar los datos relacionados con la disponibilidad de habitaciones en Airbnb utilizando herramientas y técnicas de Business Intelligence (BI), con el fin de:

1. **Identificar patrones y tendencias** en la ocupación y disponibilidad de alojamientos, considerando factores como temporada, ubicación y precios.
2. **Optimizar la disponibilidad de habitaciones** para maximizar la eficiencia operativa y los ingresos tanto para los anfitriones como para la plataforma.
3. **Mejorar la toma de decisiones estratégicas** mediante la extracción de información valiosa que ayude a los anfitriones y a Airbnb a mejorar la experiencia del usuario y aumentar la rentabilidad.
Este análisis busca generar insights que permitan una gestión más eficaz de los alojamientos y una mejor experiencia en la plataforma.

## Resumen de Preprocesamiento de Datos

El dataset original contenía columnas desordenadas, con campos importantes como `host_id`, `host_name`, `name`, `neighbourhood_group` y `neighbourhood` fuera de lugar. Para resolver este problema, se unieron múltiples tablas, lo que permitió identificar patrones y reorganizar los datos adecuadamente utilizando Python. Este paso de preprocesamiento aseguró un dataset estructurado, preparando el terreno para análisis posteriores, incluyendo la detección de valores nulos y duplicados, que guiarán las próximas decisiones.
## Manejo de nulos en room_type

Este script carga un dataset de Airbnb desde un archivo CSV y realiza varias transformaciones:

1. **Capitalización de Nombres**: Se transforma la columna `name` para que solo la primera letra esté en mayúscula.
2. **Asignación de Tipos de Habitación**: Basado en palabras clave, el script asigna valores a la columna `room_type` si está vacía. Las categorías de habitación son: `Entire home/apt`, `Private room` y `Shared room`.
3. **Manejo de Datos Nulos**: Antes y después de la asignación de los tipos de habitación, se verifican los valores nulos en la columna `room_type`.

Este proceso automatiza la clasificación de las propiedades según el nombre del anuncio en función de palabras clave predefinidas.
