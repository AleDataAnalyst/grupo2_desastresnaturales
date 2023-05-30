Propuesta de gobernanza de datos
Organizar datos en carpetas conforme se van manipulando datos y cambiando el dataset.
00OriginalNoEditar: Como su nombre lo indica, este archivo es el original y solo para referencia de la fuente. IMPORTANTE: No debe editarse ni manipularse su contenido. El README de esta carpeta debe contener url fuente así como sinopsis de la metodología de recogida de datos.
01Crudo: Copia del original con un nombre más corto para facilitar incorporarlo con readcsv en la primera fase de exploración SIN MANIPULAR, BORRAR o guardar otros valores sobre este. Con este definiremos objetivos, haremos EDA básico de estadísticas, .shape, .info, .describe, .columns, etc. para conocer volumen de datos, relacionarnos con los datos y decidiremos qué borrar/limpiar.
01ParaLimpiar: Copia del anterior que no debe haber sido manipulada. En este limpiaremos valores nulos, borraremos columnas y filas, etc. Guardaremos el archivo tras haberlo manipulado como 02desastres_cleaned en la carpeta 02Limpio.
02Limpio: Seguiremos realizando EDA con estadísticas.
...
Añadiremos y nombraremos carpetas según nos demande el proceso,
cuidando metodología de gobernanza.

Al nombrar carpetas y archivos:
Utiliza nombres cortos e intuitivos
No usar espacios, caracteres raros o especiales (!"·$%&/()?) ni ñ.
Usar punto (.) solo para separar nombre de extensión.
No mayúsculas en todo el nombre
Para separar palabras utiliza guión bajo _, de preferencia.
Recuerda la nomenclatura numérica como prefijo al seguir la metodología.
