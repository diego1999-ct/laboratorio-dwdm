\# 2. Inventario de Equipos y Componentes



A continuación, se detalla la función técnica, el tipo de interfaz y el rol dentro del rack para cada uno de los 7 componentes que conforman la maqueta DWDM:



\## 1. Analizador Ethernet (MTX150x)

\* \*\*Función Técnica:\*\* Generación de tráfico L2/L3 y ejecución de pruebas de rendimiento estandarizadas como RFC 2544 y Y.1564.

\* \*\*Rol en el Rack:\*\* Actúa como el equipo cliente de origen y destino para inyectar tráfico y validar que los datos atraviesan la red óptica sin errores ni pérdida de tramas.



\## 2. Analizador de Espectro Óptico - OSA (RXT4510)

\* \*\*Función Técnica:\*\* Análisis del espectro óptico, medición de potencia por canal y cálculo de la relación señal a ruido óptica (OSNR).

\* \*\*Rol en el Rack:\*\* Permite visualizar gráficamente las longitudes de onda (canales DWDM) que viajan por la fibra y diagnosticar la calidad y salud de la señal transmitida.



\## 3. Switch Ethernet (CSS610)

\* \*\*Función Técnica:\*\* Agregación de clientes Ethernet e interconexión de tráfico de datos.

\* \*\*Rol en el Rack:\*\* Concentra múltiples conexiones de cliente de baja o mediana capacidad antes de entregarlas al chasis transpondedor, gestionando el tráfico a nivel de Capa 2.



\## 4. ODF (Optical Distribution Frame)

\* \*\*Función Técnica:\*\* Panel de parcheo para la organización física de las conexiones ópticas.

\* \*\*Rol en el Rack:\*\* Proporciona un punto centralizado y seguro para interconectar los equipos mediante \*patch cords\* de fibra, facilitando la administración del cableado.



\## 5. Chasis DWDM 1 y DWDM 2 (HT6000)

\* \*\*Función Técnica:\*\* Chasis multiplexor y transpondedor. Aloja tarjetas de línea, módulos WDM y la tarjeta de gestión de red.

\* \*\*Rol en el Rack:\*\* Realiza la conversión electro-óptica, mapea el tráfico de los clientes a longitudes de onda DWDM específicas y multiplexa/demultiplexa los canales hacia el enlace principal.



\## 6. Carretes de Fibra Óptica (AB - 25 KM y BA - 25 KM)

\* \*\*Función Técnica:\*\* Bobinas de prueba que simulan un enlace de transmisión físico de 25 km por sentido.

\* \*\*Rol en el Rack:\*\* Introducen atenuación y dispersión físicas en la señal para replicar las condiciones reales de una red de transporte de larga distancia entre dos nodos.



\## 7. Atenuador Óptico Variable - OVA (JW3303)

\* \*\*Función Técnica:\*\* Control y simulación de la atenuación de potencia en el enlace óptico.

\* \*\*Rol en el Rack:\*\* Se inserta manualmente en el enlace para aumentar artificialmente la pérdida de señal, lo que permite evaluar la sensibilidad de los receptores y medir los umbrales de error.

