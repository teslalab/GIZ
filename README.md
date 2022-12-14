# Tarjeta de control Escuela Taller
![](/img/kit.png)
![](/img/logos.png)
## Guia de Instalación de Tarjeta ESP32 en Arduino IDE
### Pasos A Seguir:
1. Instalar Arduino IDE (no usar el zip)
2. Abrir ARDUINO IDE
3. Debemos ir a la pestaña ***Archivo***->***Preferencias***.
	- En la pestaña ***Ajustes*** buscamos la opción: ***Gestor de URLs Adicionales de Tarjetas: ***
	- Pegamos la siguiente URL: `https://dl.espressif.com/dl/package_esp32_index.json`
	- Luego precionamos la opción ***OK*** y automaticamente se cerrara la ventana.
4. Debemos ir a la pestaña ***Herramientas***->***Placa***->***Gestor de tarjetas***.
	- Colocamos en la barra de busqueda ***ESP32***.
	- Seleccionamos la opción que nos muestre ***esp32***.
	- Instalamos y luego precionamos la opción de ***Cerrar***.

Con esto tendremos completa la instalación de nuestra tarjeta ESP32 y lista para ser programada.	
![Arduino Settings](arduino_settings.png)

5. Instalar el módulo del ESP32 en el gestor de tarjetas.

### Instalación USB Driver ***(Si no reconoce el puerto COM)***

En algunos casos nuestra PC no es capaz de reconocer el dispositivo USB que nosotros conectamos, es por ello que dejaremos un archivo para la instalación del driver con ello nuestra PC deberá ser capaz de reconocer el dispositivo conectado, en caso de que el problema persista asegúrese de que su dispositivo no se este sobre calentando.

[Descarga este driver para Windows][DRIVER_USB]

[DRIVER_USB]: https://www.arduined.eu/files/windows10/CH341SER.zip

1. Descomprimir el archivo ZIP descargado 
2. Seleccionar el archivo para instalación de Windows
	- SETUP.exe
3. Seleccionar CH341SER.INF
4. Click en la opción ***Install***
5. Cuando este instalado cerrar la ventana y listo.!

Con esto estaría lista la instalación del Driver USB para nuestra tarjeta en el Sistema Operativo Windows.

Puede seguir está guía para la instalación como una segunda opción 

[Sigue la guía para instalar el driver CH340][DRIVER_CH340]

[DRIVER_CH340]: https://www.arduined.eu/ch340-windows-10-driver-download/

# Mapeo de Pines

## STEM Board v1.0 

### NeoPixel
Dispositivo | GPIO 
--- | --- 
NeoPixel 1 | 15 
NeoPixel 2 | 13 

### Buzzer
Dispositivo | GPIO 
--- | --- 
Buzzer | 27 

### Motores
Dispositivo | GPIO 
--- | --- 
AIN 1 | 32
AIN 2 | 33
BIN 1 | 25
BIN 2 | 26

### Ultrasónico
Dispositivo | GPIO 
--- | --- 
VCC | 5V
GND | Ground
Trigger | 17
Echo | 16

### Comunicación I2C
Dispositivo | GPIO 
--- | --- 
VCC | 3V3
GND | Ground
SCL | 22
SDA | 21

### Comunicación SPI
Dispositivo | GPIO 
--- | --- 
VCC | 3V3
GND | Ground
CLK | 18
CS | 5
SDI | 19
SDO | 23


### GPIO Extras
Dispositivo | GPIO 
--- | --- 
VCC | 5V
GND | Ground
0 | 36
1 | 39
2 | 34
3 | 35
