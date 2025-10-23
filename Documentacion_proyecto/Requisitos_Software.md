| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.F.1 | Dispositivo que te dicen la ocupación de la vía | Cada vía de tren tendrá ciertos dispositivos que mediante señales eléctricas, envíen un cierto voltaje para saber si está ocupada la vía |
| R.F.2 | Valores para la predicción e incidencias | Gracias a los valores obtenidos podremos detectar ciertas incidencias o predecir gracias a ellas |
| R.F.3 | Fichero CSV | El elemento que lea los valores de los voltajes de cada vía será de un fichero CSV |
| R.F.4 | Formato de como vera el voltaje el elemento | La hora ira en un formato (HH:MM:SS:MS) y el estado de la vía será un formato en valor binario (0/1). |
| R.F.5 | Dispositivos en la vía ferroviaria | Cada vía ferroviaria podrá llevar varios dispositivos y estos irán colocados cada ciertos metros. Además los dispositivos tendrán un identificador propio |
| R.F.6 | Valor de presencia de tren en la vía | Para saber si hay un tren en la vía el valor en binario que se nos devuelve es 0 si hay un tren o un 1 si la vía está libre |
| R.F.7 | Modulo inteligente para las incidencias | Tendremos un módulo inteligente que pueda predecirnos tipos de incidencias gracias a los valores. |
| R.F.7.1 | Incidencia de dispositivo bloqueado | Habrá una falta de datos debido al bloqueo prolongado donde un dispositivo de la vía ferroviaria dejará de emitir datos durante un tiempo de más de 2 minutos |
| R.F.7.2 | Incidencia de saltos de frecuencia | Los saltos de frecuencia serán de 0.5 voltios |
| R.F.8 | Módulo de suscripción | El módulo de suscripción de incidencias permitirá a los usuarios publicar diferentes tipos de incidencias |
| R.F.9 | Módulo de visualización | El modulo de visualización mostrará gráficamente las incidencias de los valores del voltaje obtenidos |

| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.D.1 | Protocolos HTTP/REST | El software que se va a diseñar será una aplicación web la cual se basará en HTTP/REST |

