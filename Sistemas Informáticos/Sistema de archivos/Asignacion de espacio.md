# Asignación de espacio
Existen dos metodos para almacenar archivos, asignar bytes consecutivos o dividir el archivo en bloques no necesariamente adyacentes. El almacenamiento de manera adyacente tiene el problema de que si el archivo crece, tiene que moverse en el disco.

Una vez se decidió almacenar los archivos en bloques de tamaño fijo, se debe definir el tamaño de los bloques. Si son muy grandes, se presenta el problema de fragmentación interna en el disco, por otra parte, si se define muy pequeño implica que el archivo constará de muchos bloques y por lo tanto la recuperación de la información será lenta.

Tamaño de bloque: 512 b a 4Kb