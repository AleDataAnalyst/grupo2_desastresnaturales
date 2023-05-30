Propuesta de gobernanza de datos
Organizar datos en carpetas conforme se van manipulando datos y cambiando el dataset.
00OriginalNoEditar: Como su nombre lo indica, este archivo es el original y solo para referencia de la fuente. IMPORTANTE: No debe editarse ni manipularse su contenido. El README de esta carpeta debe contener url fuente así como sinopsis de la metodología de recogida de datos.
01Crudo: Copia del original con un nombre más corto para facilitar incorporarlo con readcsv en la primera fase de exploración SIN MANIPULAR, BORRAR o guardar otros valores sobre este. Con este definiremos objetivos, haremos EDA básico de estadísticas, .shape, .info, .describe, .columns, etc. para conocer volumen de datos, relacionarnos con los datos y decidiremos qué borrar/limpiar.
01ParaLimpiar: Copia del anterior que no debe haber sido manipulada. En este limpiaremos valores nulos, borraremos columnas y filas, etc. Guardaremos el archivo tras haberlo manipulado como 02desastres_cleaned en la carpeta 02Limpio.
02Limpio: Seguiremos realizando EDA con estadísticas.
...
Añadiremos y nombraremos carpetas según nos demande el proceso,
cuidando metodología de gobernanza.


Organizar carpetas según procesos.
Los procesos son: 
00ExplorarDatos: Estadísticas básicas (shape, info, describe, valores nulos...)
01LimpiarDatos: Se borran filas o columnas y/o cambian a 0 o media/mediana valores nulos.
02EDADatosLimpios: Una vez limpio el dataset, se realiza EDA para responder preguntas cuantitativas y cualitativas.
Usar prefijos de números 00, 01 para ordenar proceso según metodología lógica de avance.

Dentro de cada proceso hay una carpeta propia con tu nombre para trabajar.
SIEMPRE verificar que te encuentras en tu carpeta.

Recomendaciones para guardar en local y remoto:
Para realizar el GitHub Clone trabajar siempre en local, ya sea en tu ordenador o el de clase. Por ejemplo, en C:/Usuario/Documentos u otra carpeta segura que identifiques rápido con algún enlace rápido en escritorio o anclaje al inicio, barra de tareas o barra lateral de carpetas.
No trabajar directamente en el entorno nube de GitHub por ningún motivo.
No trabajar en USB. Respalda tu trabajo si quieres pero procura mantener los archivos seguros, evitando que se corrompan, en disco local más potente.
NO HACER COMMITS si no se está seguro/a. Consultar a compañeros.
Comunicar conflictos a compañeros en caso de mucha duda.

Al nombrar carpetas y archivos:
Utiliza nombres cortos e intuitivos
No usar espacios, caracteres raros o especiales (!"·$%&/()?) ni ñ.
Usar punto (.) solo para separar nombre de extensión.
No mayúsculas en todo el nombre
Para separar palabras utiliza guión bajo _, de preferencia.
Recuerda la nomenclatura numérica como prefijo al seguir la metodología.
