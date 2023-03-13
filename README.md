# PZEM-004-T-Software-GUI
Este software de interfaz de usuario, diseñado en NI LabVIEW : www.ni.com,  nos permite hacer una prueba -rapida y/o test de los modulos medidores de energia y potencia en Wattios PZEM 004T via interfaz TTL usando el protoclo de transmision Modbus RTU. 

Podemos encontrar mas informacion acerca de estos medidores en este enlace : https://www.aliexpress.us/item/2251832720824955.html?spm=a2g0o.store_pc_groupList.8148356.6.200f6800CcWMP4&pdp_npi=2%40dis%21USD%21US%20%2416.70%21US%20%2412.52%21%21%21%21%21%402101e9cf16786540942424107e7fef%2165858793245%21sh&gatewayAdapt=glo2usa&_randl_shipto=US

![Kwh Meters Modbus _ Modbus Volt Meter _ Modbus Current _ 100a Pzem 004t _ Pzem 3 Phases - Current Meters - Aliexpress y 4 páginas más -  InPrivate _ Microsoft​ Edge 12_03_2023 15_59_59 (2)](https://user-images.githubusercontent.com/106831539/224573460-57b4504d-4a7f-44b6-a7d0-ffc7f1bc79a0.png)

Podemos descargar en Software instalador a traves del enlace mostrado abajo en la imagen : 

# Vista Previa del GUI
![PZEM 004T-100A GUI 12_03_2023 15_59_42](https://user-images.githubusercontent.com/106831539/224573508-2d887a11-e3c0-43ef-8f26-c8f5831a5d81.png)
 
 Link de Descarga: https://mega.nz/file/uUBxyCQa#HZUQ4Pi5p9FOQSlbY4vdXwci1E3NGybYaARUrqmVA7I

# Nota 1
Se requiere una interfaz de tipo TTL -USB para conectar directamente a la maquina o Laptop en alguno de sus puertos, tal como se muestra a continuacion:
![Kwh Meters Modbus _ Modbus Volt Meter _ Modbus Current _ 100a Pzem 004t _ Pzem 3 Phases - Current Meters - Aliexpress y 4 páginas más -  InPrivate _ Microsoft​ Edge 12_03_2023 16_05_52 (2)](https://user-images.githubusercontent.com/106831539/224573830-fcfad8a4-eaac-4305-a6dd-1e226a7fbb28.png)

OBS: Recuerde que para poder establecer la comunicacion, por lo menos los terminales de Linea (L) y Neutro(N) deben estar sensando las fases de los puntos monofasicos

# Pasos de Descarga e Instalacion
1.- El link de descarga de mega, podra bajar el archivo "PZEM Software Installer.rar" , la misma que debe descomprimir y dirigirse a la ruta: /../PZEM Software Installer/Volume/Setup.exe haciendo clic en el instalador ejecutable : 

![PZEM GUI 13_03_2023 11_25_22](https://user-images.githubusercontent.com/106831539/224764998-5991f24f-4041-4d30-bbc5-71343a83b434.png)

2.- Le solicitara privilegios de administrador. Luego debe especificar alguna ruta de instalacion (archivos de programa por default) y dar en siguiente hasta Finalizar.

![PZEM GUI 13_03_2023 11_26_22](https://user-images.githubusercontent.com/106831539/224766047-abd3ea19-2d16-405e-aa0c-a08b5af80d16.png)

Nota: No es necesario que tenga instalado el sistema de desarrollo de NI LabVIEW, ya que esta aplicacion funciona como stand-alone post-instalacion

# Pasos de Ejecuacion.
1.- Una vez terminado el asistente de instalacion, le mostrara una ruta de fichero similar a : /../PZEM Software GUI/PZEM GUI en donde encontrara la aplicacion PZEM004T.exe , debe darle clic: 

![PZEM GUI 13_03_2023 11_38_04 (2)](https://user-images.githubusercontent.com/106831539/224767845-65b59d9a-1e91-4dfc-af09-fff720bc4119.png)

Nota: Se recomienda crear un acceso directo a la aplicacion en el Escritorio (Desktop) 

2.- Aparecera el siguiente GUI:

![PZEM 004T-100A GUI 12_03_2023 15_59_42](https://user-images.githubusercontent.com/106831539/224769318-9f733bac-7181-4e40-9e35-b456720904f3.png)

3.- Segun la nota 1, la interfaz USB-TTL ya debe de estar conectada y reconocida en el computador por lo que se le asiganara un COM#. Asegurese tambien que los rings "Address(1)" , "BaudRate(9600)" tengan valores correctos acorde el sensor. Luego click en OpenCOM.Le saldra un mensaje de confirmacion de apertura de puerto. Click en "Aceptar" 

![Screenshot 12_03_2023 11_10_27](https://user-images.githubusercontent.com/106831539/224770981-03a0f427-4382-4eab-ae75-fe6bc93f74b0.png)

4.- Para iniciar las lecturas, haga Click en el boton "GO". Vera algo similar a lo que se muestra en la imagen: 

![PZEM 004T-100A GUI 12_03_2023 11_16_47](https://user-images.githubusercontent.com/106831539/224772545-70c3eaf1-d3f3-4be9-9ac6-0718ac3b5234.png)

Entre otras opciones que puede cambiar esta el tiempo en segundos entre lecturas en el menu desplegable "D.S" para asi hacerlas mas rapidas o mas lentas

5.- Si desea finalizar con lac lecturas, haga click primero en el boton "STOP" asi el modulo ya no seguira leyendo y conservara los ultimos valores muestreados.

![PZEM 004T-100A GUI 12_03_2023 11_13_42](https://user-images.githubusercontent.com/106831539/224774066-3005d4bf-b545-43c1-8ebd-bc833ef81948.png)

6.- Le saldra un mensaje de aviso , de en "Aceptar"

![Screenshot 12_03_2023 11_15_20](https://user-images.githubusercontent.com/106831539/224774703-73ad1060-f052-494c-af61-c4d1effce17e.png)

# OBS
Si desea salir de la aplicacion, primero debe cerrar el COM : "CloseCOM". Enseguida puede dar click en el boton "EXIT" o en "cerrar", para esto el COM# no debe de estar abierto ni adquiriendo datos

![Screenshot 12_03_2023 11_17_53](https://user-images.githubusercontent.com/106831539/224775028-03966dc5-8c5f-4d88-a8cf-8afb82ba6251.png)

# Nota Final
El leguaje de programacion LabVIEW permite programar, validar de forma rapida e intuitiva mediante iconos graficos y la vez comunicarnos con Hardware propietario de NI o HW abierto. Podemos encontrar mayor informacion de este entorno de desarrollo aqui: https://www.ni.com/es-cr/shop/labview.html
