## RETO DE DISEÑO
### ¿En qué consiste?
Se nos ocntrató para crear un control de potencia de un motor destinado a dar movimiento a una maquina que mezcla sangre en un laboratorio, para evitar que la sangre se coagule. El usuario debe ser capaz de modificar la potencia del motor y debe poder visualizarla en 3 displays 7 segmentos que le muestran el porcentje de potencia de 0 a 100. Tambien debe ser capaz de cambiar de dirección (horario y antihorario) y tener dos luces testigos que me indiquen la dirección, rojo para horario y verde para antihorario, las direcciones se deben seleccionar con dos pulsadores y la potencia se modifica con un potenciometro.

### ¿Cómo se desarrolló?
El codigo se cargó a una ESP32. La potencia se modificó utilizando el PWM del canal 1 salida DAC, y la entrada del potenciometro en una entrada ADC, la conversión para el Duty cycle se hizo de manera directa. El cambio de dirección es simplemente variando las salidas de los pines conectados a las salidas left y right.

## ¿Qué puedo encontrar en el repositorio?
Aquí puedes encontrar el esquema electrico utilizado y el codigo que hace posible que funcione.