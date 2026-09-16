\# 3. Manual de Configuración y Seguridad Óptica



\## 3.1 Medidas de Seguridad Óptica

El trabajo con redes DWDM involucra radiación láser de alta potencia que es \*\*invisible\*\* al ojo humano.

\* \*\*Radiación Láser (Clase 1M/3R):\*\* Nunca se debe mirar directamente a los extremos de una fibra óptica activa o a los puertos de transmisión del equipo. 

\* \*\*Limpieza de Conectores:\*\* Siempre se debe inspeccionar la fibra y limpiar los terminales (con lápiz limpiador o casetes de limpieza en seco) antes de cada inserción. La suciedad es la principal causa de pérdida de señal.

\* \*\*Manejo de Conectores APC y UPC:\*\* 

&#x20; \* \*\*UPC (Azul):\*\* Conector de contacto ultra físico (pulido plano).

&#x20; \* \*\*APC (Verde):\*\* Conector de contacto físico en ángulo (pulido a 8 grados).

&#x20; \* \*\*¡ADVERTENCIA CRÍTICA!:\*\* Nunca se debe conectar un terminal UPC con uno APC directamente. Esta acción destruirá físicamente la férula de cristal de ambos conectores.



\## 3.2 Configuración del Chasis HT6000

Para establecer el enlace de transporte, se deben seguir estos pasos genéricos en la plataforma de gestión del chasis:

1\. \*\*Aprovisionamiento de Servicios:\*\* Ingresar al sistema de gestión, reconocer las tarjetas transpondedoras / muxpondedoras instaladas y encender administrativamente los puertos ópticos.

2\. \*\*Mapeo de Puertos:\*\* Configurar la asignación lógica, vinculando la interfaz de entrada del cliente (el puerto SFP/SFP+ donde llega el tráfico) con la interfaz de línea (la salida de alta capacidad hacia el ODF).

3\. \*\*Asignación de Canales:\*\* Configurar el láser sintonizable de la interfaz de línea DWDM para que transmita en la longitud de onda o frecuencia exacta dictada por el diseño de red, respetando la grilla de la ITU-T.



\## 3.3 Procedimiento de Prueba y Medición

Una vez que el enlace DWDM está activo, se debe validar su calidad e integridad:

1\. \*\*Inserción del OVA (JW3303):\*\* Conectar el atenuador óptico variable en el trayecto de la fibra y aumentar gradualmente la atenuación (dB) para simular la degradación de un enlace de larga distancia.

2\. \*\*Análisis Espectral (OSA RXT4510):\*\* Conectar el analizador de espectro a un puerto de monitoreo. Se debe verificar la presencia del canal DWDM encendido, medir su potencia óptica de recepción (Rx) y calcular la Relación Señal a Ruido Óptica (OSNR).

3\. \*\*Pruebas Ethernet (MTX150x):\*\* Ejecutar una prueba de tráfico desde el analizador. Monitorear los resultados para garantizar que no exista pérdida de tramas y que la Tasa de Error de Bits (BER) sea cero (o esté dentro del margen aceptable soportado por la corrección de errores FEC) durante la simulación de atenuación.

