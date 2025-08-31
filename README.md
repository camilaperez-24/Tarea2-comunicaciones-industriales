# SEGUNDA TAREA – Comunicaciones Industriales

## Código ASCII (American Estándar Code for Information Interchange)

El código ASCII se creó en el año 1963 por medio del comité ANSI para determinar una forma de unificar la representación de caracteres en sistemas electrónicos, contribuyendo de igual forma a reducir los problemas de compatibilidad entre los fabricantes.  

ASCII utiliza un estándar original de 7 bits para representar 128 caracteres, incluyendo dígitos, símbolos, letras mayúsculas y minúsculas.  

El principal aspecto que habla acerca de su importancia es la estandarización del intercambio de texto entre dispositivos, además de que por esta misma razón fue la base de la codificación de textos en los primeros sistemas de telecomunicaciones.  

Su funcionamiento básico se basa en que cada carácter cuenta con un valor decimal que es único, en comunicaciones seriales como RS232 se transmite bit a bit y los primeros 32 caracteres son de control.  

Un ejemplo podría ser el número 1, que en el código decimal representa un 49 y en binario corresponde a 00110001.  

---

## Pines conectores RS232: DB9 y DB25

El protocolo correspondiente a RS232 define un sistema de comunicación de tipo serial punto a punto y utiliza conectores estándar tipo D-subminiatura, lo que significa el uso de señales asíncronas.  

### DB9 (9 pines)

| Pin | Señal | Descripción |
|-----|-------|-------------|
| 1   | DCD   | Data Carrier Detect – Detecta la portadora del módem |
| 2   | RXD   | Receive Data – Recibe datos |
| 3   | TXD   | Transmit Data – Transmite datos |
| 4   | DTR   | Data Terminal Ready – Indica que el terminal está listo |
| 5   | GND   | Ground – Tierra de señal |
| 6   | DSR   | Data Set Ready – Indica que el módem está listo |
| 7   | RTS   | Request To Send – Solicitud de envío |
| 8   | CTS   | Clear To Send – Permiso para enviar |
| 9   | RI    | Ring Indicator – Señal de timbrado |


![Diagrama DB9](./DB1.jpg)


---

### DB25 (25 pines)

| Pin | Señal | Descripción |
|-----|-------|-------------|
| 2   | TXD   | Transmit Data |
| 3   | RXD   | Receive Data |
| 4   | RTS   | Request To Send |
| 5   | CTS   | Clear To Send |
| 6   | DSR   | Data Set Ready |
| 7   | GND   | Signal Ground |
| 8   | DCD   | Data Carrier Detect |
| 20  | DTR   | Data Terminal Ready |
| 22  | RI    | Ring Indicator |

![Diagrama DB25](./DB2.jpg)

---

## Formato del Protocolo (RS232)

Se determina la comunicación establecida por el protocolo RS232 como asíncrona.  

Por una parte, se habla de niveles de voltaje:  

- -3V a -15V → 1 (Mark)  
- +3V a +15V → 0 (Space)  

Y se considera estar fuera ambos de los rangos establecidos como una condición de estado inválido.  

Además, tiene una estructura establecida donde se tiene el bit de inicio que por lo general es 0, después los datos de 5-8 bits, la paridad y los bits de parada.
También, no tiene direccionamiento incorporado como el internet.  

---

## Referencias

1. ANSI, American National Standard for Information Systems — Coded Character Sets — 7-Bit American Standard Code for Information Interchange (ASCII), ANSI X3.4-1986, American National Standards Institute, 1986.  

2. TIA/EIA, Interface Between Data Terminal Equipment and Data Circuit-Terminating Equipment Employing Serial Binary Data Interchange (RS-232C), TIA/EIA-232-F Standard, Telecommunications Industry Association, 1997.  

3. USconverters, “RS232 Pinout and Specifications,” USconverters.com. [En línea]. Disponible en: https://www.usconverters.com/rs232-pinout-cable. [Accedido: 31-Aug-2025].  

4. CAMI Research, “RS232 Serial Communications - Pinouts,” Camiresearch.com. [En línea]. Disponible en: https://www.camiresearch.com/Data_Com_Basics/RS232_standard.html. [Accedido: 31-Aug-2025].  

5. Aggsoft, “RS232 Pinout and Wiring,” Aggsoft.com. [En línea]. Disponible en: https://www.aggsoft.com/rs232-pinout-cable/RS232.htm. [Accedido: 31-Aug-2025].
