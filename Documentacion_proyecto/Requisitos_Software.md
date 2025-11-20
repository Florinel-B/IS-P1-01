| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.F.1 | Dispositivo que te dicen la ocupación de la vía | Cada vía contará con múltiples dispositivos sensores que envían señales eléctricas en voltios para detectar la ocupación de la vía. |
| R.F.2 | Valores para la predicción e incidencias | Gracias a los valores obtenidos podremos detectar ciertas incidencias o predecir gracias a ellas. Estos valores serán utilizados por el módulo inteligente para detectar y predecir incidencias. |
| R.F.3 | Fichero CSV | El elemento que lea los valores de los voltajes de cada vía será de un fichero CSV. |
| R.F.4 | Formato de como vera el voltaje el elemento | La hora irá en un formato (HH:MM:SS:MS) y el estado de la vía será un formato en valor binario (0/1). |
| R.F.5 | Dispositivos en la vía ferroviaria | Cada vía ferroviaria podrá llevar varios dispositivos y estos irán colocados cada ciertos metros. Además, los dispositivos tendrán un identificador propio. |
| R.F.6 | Valor de presencia de tren en la vía | Para saber si hay un tren en la vía, el valor en binario que se nos devuelve es 0 si hay un tren o un 1 si la vía está libre. |
| R.F.7 | Modulo inteligente para las incidencias | Tendremos un módulo inteligente que pueda predecir tipos de incidencias gracias a la información que tenemos del R.F.7.1 Y R.F.7.2. |
| R.F.7.1 | Incidencia de dispositivo bloqueado | Habrá una falta de datos debido al bloqueo prolongado donde un dispositivo de la vía ferroviaria dejará de emitir datos durante un tiempo de más de 2 minutos. |
| R.F.7.2 | Incidencia de saltos de frecuencia | Los saltos de frecuencia serán de 0.5 voltios |
| R.F.8 | Módulo de suscripción | Un módulo de suscripción a incidencias por parte de los usuarios del sistema donde se pueden publicar diferentes tipos de incidencias. (no se sabe el que publica las incidencias). |
| R.F.9 | Módulo de visualización | El módulo de visualización mostrará gráficamente las incidencias de los valores del voltaje obtenidos. |

| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.D.1 | Protocolos HTTP/REST | El software que se va a diseñar será una aplicación web la cual se basará en HTTP/REST |

