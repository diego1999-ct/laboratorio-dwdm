\# 4. Esquemas de Red y Topología



\## 4.1 Diagrama de Conexiones Físicas

El siguiente diagrama ilustra el cableado físico entre el Switch Ethernet, el chasis HT6000, el ODF, los carretes de fibra y los instrumentos de medición.



!\[Diagrama Físico](../diagramas/imagenes/diagrama\_fisico.png)

\*(Nota: Reemplazar con la imagen exportada de Draw.io en la carpeta correspondiente)\*



\## 4.2 Mapeo de Puertos (Tabla de Interconexión)

| Origen (Equipo / Puerto TX) | Destino (Equipo / Puerto RX) | Tipo de Cable / Interfaz |

| :--- | :--- | :--- |

| MTX150x (Puerto TX L2) | Switch CSS610 (Puerto 1) | Cobre UTP (RJ45) / Óptico SFP |

| Switch CSS610 (Puerto 2) | HT6000 DWDM 1 (Cliente SFP+ TX) | Patchcord Óptico LC-LC |

| HT6000 DWDM 1 (Línea OUT) | ODF (Puerto IN) | Patchcord Óptico LC-LC |

| ODF (Puerto OUT) | Carrete Fibra AB 25km | Fibra Monomodo (SMF) |

| Carrete Fibra AB 25km | OVA (JW3303 IN) | Fibra Monomodo (SMF) |

| OVA (JW3303 OUT) | HT6000 DWDM 2 (Línea IN) | Patchcord Óptico LC-LC |



\## 4.3 Flujo de la Señal Óptica

La trayectoria que recorre la señal de extremo a extremo es la siguiente:

1\. \*\*Transmisión de Cliente:\*\* El analizador MTX150x genera el tráfico Ethernet y lo envía al Switch para su agregación.

2\. \*\*Conversión Electro-Óptica:\*\* El Switch entrega la señal al puerto de cliente del chasis HT6000, donde la tarjeta transpondedora modula esta señal sobre un láser DWDM específico (ej. Canal ITU 32).

3\. \*\*Multiplexación:\*\* La señal DWDM se agrupa con otros canales y sale por la interfaz de línea hacia el ODF.

4\. \*\*Enlace Físico:\*\* La luz viaja a través del carrete de fibra de 25 km, sufriendo atenuación natural. Luego pasa por el atenuador (OVA), donde agregamos atenuación controlada manual.

5\. \*\*Recepción y Demultiplexación:\*\* La señal atenuada llega al segundo chasis HT6000, se demultiplexa, se convierte nuevamente a una señal Ethernet estándar y se valida en el equipo destino.



\## 4.4 Topología Lógica

!\[Diagrama Lógico](../diagramas/imagenes/diagrama\_logico.png)

\*(Nota: Reemplazar con la imagen exportada de Draw.io)\*

