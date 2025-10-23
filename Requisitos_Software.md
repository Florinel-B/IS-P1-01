
| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.F.1 | Gestión de la tensión en vías ferroviarias. | Cada vía de tren tiene sus dispositivos, que enviaran sus señales eléctricas mediante un voltaje e indicará si está o no ocupada esa via y gracias a ellos se podrá predecir y detectar incidencias |
| R.F.1.1 | Ocupación de la vía ferroviaria por un tren | Cada vía de tren cuenta con sus dispositivos, los cuales detectan si está el tren o no. Eso se hara por señales eléctricas que llegan por un voltaje  |
| R.F.1.2 | Detección y predicción de incidencias | En función de los valores que den las vías del tren, es decir, la señal eléctrica en voltios, es posible que surjan incidencias que hay que detectar y predecir. |
| R.F.2 | Atributos que indiquen el estado de la vía | Un elemento que lea los valores de voltajes de las vías desde un fichero CSV con la hora en formato (HH:MM:SS:MS) y un valor binario (0/1) que indica el estado (dependera del valor umbral que nos tendrán que proporcionar). |
| R.F.3 | Dispositivos en la/s vía/s del tren |  Por cada vía de tren pueden existir múltiples dispositivos cada cierto número de metros. Cada dispositivo debe llevar un identificador.  |
| R.F.3.1 | Múltiples dispositivos en cada vía |  Por cada vía de tren pueden existir múltiples dispositivos cada cierto número de metros |
| R.F.3.2 | Dispositivo en la vía del tren | Cada dispositivo debe llevar un identificador |
| R.F.4 | Detección tren en vía | Una funcionalidad que detecte si hay un tren en la vía en función del valor binario (1: vía libre, 0: hay un tren). El sistema registrará el evento en la base de datos y actualizará la visualización de estado de la vía. |
| R.F.5 | Módulo predicción incidencias | Un módulo inteligente que detecte y sea capaz de predecir tipos de incidencias en función de los valores.  |
| R.F.5.1 | Ausencia de datos | Ausencia de datos por bloqueo prolongado donde un dispositivo de vía no emite datos por un periodo de más de 2 minutos |
| R.F.5.2 | Salto de frecuencia | Saltos de frecuencia de al menos 0.5 voltios |
| R.F.6 | Suscripción de incidencias  | Un módulo de suscripción a incidencias por parte de los usuarios del sistema donde se pueden publicar diferentes tipos de incidencias.   |
| R.F.7 | Visualización de incidencias | Un módulo de visualización que muestre gráficamente las incidencias en función de los valores de los voltajes. El usuario podrá filtrar las incidencias por tipo, hora y dispositivo. |

Dominio

| \# | NOMBRE | DESCRIPCIÓN |
| ----- | ----- | ----- |
| R.D.1 | Protocolos HTTP/REST | El software que se pretende diseñar es una aplicación Web basada en protocolos HTTP/REST |
