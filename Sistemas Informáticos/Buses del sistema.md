# Buses del sistema
<!-- TODO: completar descripcción inicial -->
Son canales de transmisión de datos digitales, 

## Tipo de buses
### Paralelo
Los datos se envian por bytes al mismo tiempo, dado que hay varios conductores y tienen funciones fijas. El ancho de banda es igual al producto de la frecuencia por el ancho de los datos.

### Serie
Los datos se envian bit a bit y se contruyen por medio de registros o rutinas. Está formado por pocos conductores y su ancho de banda depende de la frecuencia.

Se utiliza en discos duros, unidades de estado solido, tarjetas de expansión y para el bus del procesador.

<!-- TODO: cambiar esta parte, como tal no existe, pero es una breve explicación de "un bus" -->
## Transmisiones
Se busca que las perturbaciones afecten lo menos posible, por ello se usa blindaje y otros metodos para reducirlas a lo minimo posible.

Pasamos de utilizar clables IDE, con bajas frecuencias de transmisión, a cables SATA reduciendo el número de hilos, aumentando la fiabilidad y por ende la frecuencia.

## Otros tipos
<!-- TODO: añadir más tipos, a pesar de que algunos estan obsoletos -->
### Universal Serial Bus
El USB se divide en:

| Año | Modo | Abreviatura | Tasa de transferencia | Version | 
|------|:-----------:|-----------------------|:--------:|:---:|
| 1996 | Low Speed | LS | 1.5 Mbit/s (187.5 KB/s) | 1.0 |
| 1998 | Full Speed | FS | 12 Mbit/s (1.5 MB/s) | 1.1 |
| 2001 | High Speed | HS | 480 Mbit/s (60 MB/s) | 2.0 |
| 2011 | SuperSpeed | SS | 5 Gbit/s (625 MB/s) | 3.0 |
| 2014 | SuperSpeed+ | SS+ | 10 Gbit/s (1.25 GB/s) | 3.1 |
| 2017 | SuperSpeed+ | SS+ | 20 Gbit/s (2.5 GB/s) | 3.2 |

El estándar USB 1.x y 2.0 proporciona 5V de alimentación y una conexión para los dispositivos conectados. La unidad de carga se definión con 100 mA, pudiendo consumir un solo dispositivo 5 (500mA) unidades de carga, y 150mA USB 3.0, llegando a poder utilizar 6 unidades de carga. 

<br>

### Firewire
Es un estándar multiplataforma para entrada y salida de datos en serie a gran velocidad. Se utiliza para interconexión de dispositivos digitales como cámaras digitales y videocámaras.

| Nombre | Versión | Tasa de transferencia |
|--------|---------|-----------------------|
| 400 | IEEE 1394-1995 | 400 Mbit/s (50 MB/s) |
| 800 | IEEE 1394b-2002 | 800 Mbit/s (100 MB/s) |
| S800T | IEEE 1394c-2006 | 800 Mbit/s (100 MB/s) |
| s1600 | IEEE 1394-2008 | 1.6 Gbit/s (200 MB/s) |
| s3200 | IEEE 1394-2008 | 3.2 Gbit/s (400 MB/s) |

