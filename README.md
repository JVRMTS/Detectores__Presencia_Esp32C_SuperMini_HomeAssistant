<h1>DETECTORES DE PRESENCIA UTILIZANDO ESP32C3 SUPER MINI Y LD2410 Y LD2420 PARA ESPHOME Y HOMEASSISTANT</h1>
<P>Despues de estar buscando como configurar los detectores de presencia HLK-LD2410 y HLK-LD2420 y ver que habia poca información,
  me dedique a realizar pruebas para intentar configurarlos, de esas pruebas llegan estos resultados:</P>

<p>He conseguido configurar los dos, y si te fijas en los archivos YAML verás que hay que cambiar los pines 20 y 21 dependiendo 
del sensor que estés utilizando, no se si es por una mala definición de los pines en las placas que tengo o porque estan mal serigrafiados, 
el caso es que así funcionan los dos.</p>

<p>También he realizado dos bocetos en Fritzing para ponerlos en funcionamiento, tiene la PCB diseñada, actualmente los tengo los dos funcionando.</p>

<P>Los dos tienen una fuente de alimentación HLK-PM01 de 5V y 0.6A se alimentan a 220V de corriente alterna, pues tengo intención de colocarlos 
pegados a los plafones que tengo y sacar la alimentación desde estos.</P>
<h2>NOTA 22/07/2025</h2>
<p>El LD2420 me ha fallado al actualiarlo con la versión 2025.7.2 de ESPHOME, funciona con la versión 2025.6.3</p>
<h2>NOTA 06/09/2025</h2>
<p>Desde la actualización 2025.7.2 de ESPHOME dejó de funcionar si se actualizaba por encima de esa versión de ESPHOME, para que funcione hay que con las versiones iguales o superiores a esa hay que cambiar los pines a los que se conecta el HLK-LD2024 - tx_pin: GPIO07 y rx_pin: GPIO06, con la configuración antigua daba problemas con el puerto USB./p>
