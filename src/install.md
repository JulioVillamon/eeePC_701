# Instalar Debian 12 + LXDE + skin WIndows 95 en Asus eeePC 701 4G
Este manual muestra paso a paso la forma de instalar la distribución Debian 12 (actual en estos momentos) con el escritorio ligero LXDE y con la apariencia de Microsoft Windows 95.

El Asus eeePC 701 4G es un netbook del a&ntilde;o 2007 que tiene tres caracter&iacute;sticas que lo hacen especial para darle uso con los actuales sistemas operativos:
1. Un disco duro de tan s&oacute;lo 4GB soldado en placa (no ampliable)
2. Una pantalla de 7" con una resoluci&oacute;n de 800x480 pixels
3. Un procesador con un s&oacute;lo n&uacute;cleo con una velocidad de 630 MHz

Esto lo convierte en un equipo pr&aacute;cticamente obsoleto, pues hay que aprovechar al m&aacute;ximo el espacio en disco y elegir bien los programas y las interfaces que se muestren mejor para la resoluci&oacute;n de pantalla que tiene.

La CPU es lenta para la internet actual y, si el sitio web tiene mucho contenido a cargar, se hace impracticable la navegaci&oacute;n. Tampoco puede manejar varios programas debido a que s&oacute;lo tiene un n&uacute;cleo.

Se elige a Debian como sistema operativo instal&aacute;ndolo sin entorno gr&aacute;fico para ir cargando despu&eacute;s los elementos necesarios para hacerlo funcionar.

**Tabla de contenidos**  
[Crear medio de arranque](#paso0)  
[Instalar Debian 12 sin escritorio](#paso1)  
[Instalar el escritorio LXDE](#paso2)   
[Instalar las utilidades del sistema](#paso3)  
[Instalar el sonido](#paso4)  
[Instalar los Codecs](#paso5)  
[Instalar el software multimedia](#paso6)  
[Instalar el software para internet](#paso7)  
[Instalar el software para ofim&aacute;tica](#paso8)  
[Instalar algunos juegos](#paso9)  
[Personalizar LXDE con la apariencia de Microsoft Windows 95](#paso10)

<a name="paso0"></a>
## Crear medio de arranque
*NOTA: Para crear la unidad USB arrancable se usa el programa Rufus en Microsoft Windows*
1. Descargamos el programa Rufus desde su direcci&oacute;n: [https://rufus.ie/es/](https://rufus.ie/es/)
2. Descargamos la imagen de instalaci&oacute;n "iso netinst para PC de 32 bits" desde la web de Debian: [https://www.debian.org/distrib/](https://www.debian.org/distrib/)
3. Grabamos la imagen en una memoria USB con capacidad suficiente (como m&iacute;nimo de 2 GB) con las siguientes opciones:  
   ![Opciones grabar Debian 32bit en Rufus](/img/0.png)

<a name="paso1"></a>
## Instalar Debian 12 sin escritorio
**Uso del teclado durante la instalaci&oacute;n**
![Teclas usadas en el teclado para instalar Debian](/img/teclado.png)
Imagen: [https://upload.wikimedia.org/wikipedia/commons/e/e5/Iso-105-dvorak-spanish-keyboard-layout.png](https://upload.wikimedia.org/wikipedia/commons/e/e5/Iso-105-dvorak-spanish-keyboard-layout.png)

Durante la instalaci&oacute;n, el rat&oacute;n no est&aacute; habilitado. Se usa el teclado para navegar por las opciones:
- Escape --> Sale al men&uacute; principal
- Tabulaci&oacute;n --> salta entre opciones
- Barra espaciadora --> marca la opci&oacute;n
- Retroceso --> borra
- Enter --> confirma la opci&oacute;n seleccionada
- Flechas de direcci&oacute;n --> nos movemos por las opciones
    
*Varia en funci&oacute;n del idioma del teclado seleccionado durante la instalaci&oacute;n*

#### [1] Conectamos la memoria USB y arrancamos el equipo presionando la tecla ESC mientras aparece el logo de Asus Eee PC:
![Imagen uno del manual para instalar Debian](/img/1.png)

#### [2] Seleccionamos la memoria USB desde la que va a arrancar:
![Imagen dos del manual para instalar Debian](/img/2.png)

#### [3] Seleccionamos "Install":
![Imagen tres del manual para instalar Debian](/img/3.png)

#### [4] Pulsamos la tecla "espacio" para que elija el instalador el modo de video:
![Imagen cuatro del manual para instalar Debian](/img/4.png)

#### [5] Elegimos nuestro idioma:
![Imagen cinco del manual para instalar Debian](/img/5.png)

#### [6] Elegimos nuestra ubicaci&oacute;n:
![Imagen seis del manual para instalar Debian](/img/6.png)

#### [7] Elegimos la configuraci&oacute;n de teclado:
![Imagen siete del manual para instalar Debian](/img/7.png)

#### [8] Esperamos mientras carga algunos componentes y configura la red:
![Imagen ocho del manual para instalar Debian](/img/8.png)

#### [9] Le damos un nombre al netbook y pulsamos la tecla "tabulaci&oacute;n" y "enter" para continuar:
![Imagen nueve del manual para instalar Debian](/img/9.png)

#### [10] Dejamos en blanco el nombre de dominio ("tabulaci&oacute;n + enter" para continuar):
![Imagen diez del manual para instalar Debian](/img/10.png)

#### [11] Le damos una contrase&ntilde;a al usuario root. ("tabulaci&oacute;n + espacio" para "Mostrar la contrase&ntilde;a en claro":
![Imagen once del manual para instalar Debian](/img/11.png)

#### [12] Nos pide que la verifiquemos:
![Imagen doce del manual para instalar Debian](/img/12.png)

#### [13] Le damos un nombre al usuario del sistema (por seguridad, para usar Debian sin ser administrador):
![Imagen trece del manual para instalar Debian](/img/13.png)

#### [14] Nos pide verificar el nombre del nuevo usuario:
![Imagen catorce del manual para instalar Debian](/img/14.png)

#### [15] Damos una contrase&ntilde;a al nuevo usuario:
![Imagen quince del manual para instalar Debian](/img/15.png)

#### [16] Y la verificamos:
![Imagen diceiséis del manual para instalar Debian](/img/16.png)

#### [17] Seleccionamos nuestra zona horaria:
![Imagen diecisiete del manual para instalar Debian](/img/17.png)

#### [18] Comienza la detecci&oacute;n de los discos y del hardware:
![Imagen dieciocho del manual para instalar Debian](/img/18.png)

#### [19] En particionado de discos elegimos "Manual" (tecla "enter" para aceptar):
![Imagen diecinueve del manual para instalar Debian](/img/19.png)

#### [20] sda es el disco duro interno de 4 GB:
![Imagen veinte del manual para instalar Debian](/img/20.png)

#### [21] sdb es la memoria que hemos conectado por usb con el instalador de Debian:
![Imagen veintiuno del manual para instalar Debian](/img/21.png)

#### [22] sdc es la la tarjeta de memoria de 32 GB:
![Imagen veintidos del manual para instalar Debian](/img/22.png)

#### [23] Seleccionamos el espacio libre del disco duro y elegimos "Crear una partici&oacute;n nueva":
![Imagen veintitrés del manual para instalar Debian](/img/23.png)

#### [24] Le damos 3.8 GB y continuamos:
![Imagen veinticuatro del manual para instalar Debian](/img/24.png)

#### [25] Elegimos Primaria:
![Imagen veinticinco del manual para instalar Debian](/img/25.png)

#### [26] La ubicamos al principio:
![Imagen vintiséis del manual para instalar Debian](/img/26.png)

#### [27] Dejamos el resto de opciones como est&aacute;n y seleccionamos "Se ha terminado de definir la partici&oacute;n":
![Imagen veintisiete del manual para instalar Debian](/img/27.png)

#### [28] Seleccionamos el espacio libre que nos queda en el disco sda:
![Imagen veintiocho del manual para instalar Debian](/img/28.png)

#### [29] Creamos una partici&oacute;n nueva:
![Imagen veintinueve del manual para instalar Debian](/img/29.png)

#### [30] Dejamos el tama&ntilde;o restante y continuamos:
![Imagen treinta del manual para instalar Debian](/img/30.png)

#### [31] Elegimos partición l&oacute;gica:
![Imagen treinta y uno del manual para instalar Debian](/img/31.png)

#### [32] Entramos en "utilizar como":
![Imagen treinta y dos del manual para instalar Debian](/img/32.png)

#### [33] Seleccionamos "área de intercambio":
![Imagen treinta y tres del manual para instalar Debian](/img/33.png)

#### [34] Por &uacute;ltimo seleccionamos "Se ha terminado de definir la partici&oacute;n":
![Imagen treinta y cuatro del manual para instalar Debian](/img/34.png)

#### [35] El disco duro queda con una partici&oacute;n de 3.8 GB para el sistema y otra con 199.2 MB para memoria swap:
![Imagen treinta y cinco del manual para instalar Debian](/img/35.png)

#### [36] Ahora seleccionamos el espacio libre de la tarjeta de memoria:
![Imagen treinta y seis del manual para instalar Debian](/img/36.png)

#### [37] Creamos una partici&oacute;n nueva:
![Imagen treinta y siete del manual para instalar Debian](/img/37.png)

#### [38] Dejamos todo el espacio y continuamos:
![Imagen treinta y ocho del manual para instalar Debian](/img/38.png)

#### [39] Tipo de nueva partici&oacute;n primaria:
![Imagen treinta y nueve del manual para instalar Debian](/img/39.png)

#### [40] En punto de montaje seleccionamos /home:
![Imagen cuarenta del manual para instalar Debian](/img/40.png)

#### [41] Por &iacute;ltimo seleccionamos "Se ha terminado de definir la partici&oacute;n":
![Imagen cuarenta y uno del manual para instalar Debian](/img/41.png)

#### [42] El particionado queda con 3.8 GB para el sistema, 199.2 MB para la memoria swap y 30.9 GB para los datos de usuario:
![Imagen cuarenta y dos del manual para instalar Debian](/img/42.png)

#### [43] Finalizamos el particionado y escribimos los cambios:
![Imagen cuarenta y tres del manual para instalar Debian](/img/43.png)

#### [44] Confirmamos los cambios:
![Imagen cuarenta y cuatro del manual para instalar Debian](/img/44.png)

#### [45] Comienza el formateo de las particiones:
![Imagen cuarenta y cinco del manual para instalar Debian](/img/45.png)

#### [46] Al acabar instala el sistema base:
![Imagen cuarenta y seis del manual para instalar Debian](/img/46.png)

#### [47] Seleccionamos nuestro pa&iacute;s para la r&eacute;plica de Debian:
![Imagen cuarenta y siete del manual para instalar Debian](/img/47.png)

#### [48] Dejamos por defecto la opci&oacute;n recomendada:
![Imagen cuarenta y ocho del manual para instalar Debian](/img/48.png)

#### [49] Dejamos en blanco la informaci&oacute;n del proxy:
![Imagen cuarenta y nueve del manual para instalar Debian](/img/49.png)

#### [50] Descargar&aacute; algunos ficheros:
![Imagen cincuenta del manual para instalar Debian](/img/50.png)

#### [51] Instalaci&oacute;n de programas:
![Imagen cincuenta y uno del manual para instalar Debian](/img/51.png)

#### [52] Elegimos si queremos enviar informaci&oacute;n a Debian sobre el uso de paquetes:
![Imagen cincuenta y dos del manual para instalar Debian](/img/52.png)

#### [53] No instalamos escritorio, ni el servidor SSH ni las utilidades est&aacute;ndar del sistema:
![Imagen cincuenta y tres del manual para instalar Debian](/img/53.png)

#### [54] Tras instalar el software, configura el gestor de arranque:
![Imagen cincuenta y cuatro del manual para instalar Debian](/img/54.png)

#### [55] Confirmamos la instalaci&oacute;n de GRUB en la unidad principal:
![Imagen cincuenta y cinco del manual para instalar Debian](/img/55.png)

#### [56] Seleccionamos /dev/sda para instalar el gestor de arraque en el disco duro del netbook:
![Imagen cincuanta y seis del manual para instalar Debian](/img/56.png)

#### [57] Finalizar&aacute; la instalaci&oacute;n con unos &uacute;ltimos ajustes:
![Imagen cincuenta y siete del manual para instalar Debian](/img/57.png)

#### [58] Nos pedir&aacute; reiniciar el netbook sin la memoria usb de instalaci&oacute;n conectada:
![Imagen cincuenta y ocho del manual para instalar Debian](/img/58.png)

#### [59] Al reiniciar nos pide el nombre de usuario y la contrase&ntilde;a:
![Imagen cincuenta y nueve del manual para instalar Debian](/img/59.png)

#### [60] Accedemos a Debian en modo texto, ya que no hemos instalado un entono gr&aacute;fico:
![Imagen sesenta del manual para instalar Debian](/img/60.png)

<a name="paso2"></a>
## Instalar el escritorio LXDE

#### [61] Accedemos al sistema en modo administrador con el comando su (contraseña adminroot):
![Imagen sesenta y uno del manual para instalar Debian](/img/61.png)

#### [62] Para instalar el escritorio ejecutamos el comando `apt install lxde-core`:
![Imagen sesenta y dos del manual para instalar Debian](/img/62.png)

#### [63] Confirmamos la instalaci&oacute;n tecleando "S" + enter:
![Imagen sesenta y tres del manual para instalar Debian](/img/63.png)

#### [64] Reiniciamos el sistema con "reboot" + enter:
![Imagen sesenta y cuatro del manual para instalar Debian](/img/64.png)

#### [65] Accedemos al entorno gr&aacute;fico con los datos del usuario:
![Imagen sesenta y cinco del manual para instalar Debian](/img/65.png)

<a name="paso3"></a>
## Instalar las utilidades del sistema

#### [66] Abrimos la terminal:
![Imagen sesenta y seis del manual para instalar Debian](/img/66.png)

#### [67] Instalamos hardinfo con `apt install hardinfo`:
![Imagen sesenta y siete del manual para instalar Debian](/img/67.png)

#### [68] Confirmamos la instalaci&oacute;n tecleando "S" + enter:
![Imagen sesenta y ocho del manual para instalar Debian](/img/68.png)

#### [69] Instalamos xarchiver con `apt install xarchiver`y confirmamos la instalaci&oacute;n:
![Imagen sesenta y nueve del manual para instalar Debian](/img/69.png)

#### [70] Instalamos wget con `apt install wget`(este paquete no pide confirmaci&oacute;n):
![Imagen setenta del manual para instalar Debian](/img/70.png)

#### [71] Instalamos el gestor de redes en dos pasos, primero con `apt install network-manager`:
![Imagen setenta y uno del manual para instalar Debian](/img/71.png)

#### [72] Luego con `apt install network-manager-gnome`:
![Imagen setenta y dos del manual para instalar Debian](/img/72.png)

<a name="paso4"></a>
## Instalar el sonido

#### [73] Instalamos el sonido primero con `apt install alsa-utils`:
![Imagen setenta y tres del manual para instalar Debian](/img/73.png)

#### [74] Instalamos el administrador con `apt install wireplumber`:
![Imagen setenta y cuatro del manual para instalar Debian](/img/74.png)

#### [75] Salimos del modo root con "exit":
![Imagen setenta y cinco del manual para instalar Debian](/img/75.png)

#### [76] Ejecutamos el comando `systemctl --user stop pulseaudio`:
![Imagen setenta y seis del manual para instalar Debian](/img/76.png)

#### [77] Y luego `systemctl --user start pipewire`:
![Imagen setenta y siete del manual para instalar Debian](/img/77.png)

#### [78] Cerramos la terminal y reiniciamos:
![Imagen setenta y ocho del manual para instalar Debian](/img/78.png)

<a name="paso5"></a>
## Instalar los codecs

#### [79]  Abrimos la terminal como administrador y actualizamos el sistema con `apt update && sudo apt upgrade`:
![Imagen setenta y nueve del manual para instalar Debian](/img/79.png)

#### [80]  Instalamos los codecs con `apt install ffmpeg libavcodec-extra`:
![Imagen ochenta del manual para instalar Debian](/img/80.png)

#### [81]  Confirmamos la instalación con "S" + enter:
![Imagen ochenta y uno del manual para instalar Debian](/img/81.png)

<a name="paso6"></a>
## Instalar el software multimedia

#### [82]  Instalamos el reproductor parole con `apt install parole`:
![Imagen ochenta y dos del manual para instalar Debian](/img/82.png)

<a name="paso7"></a>
## Instalar el software para internet

#### [83]  Instalamos el navegador por consola con `apt install lynx`:
![Imagen ochenta y tres del manual para instalar Debian](/img/83.png)

#### [84]  Instalamos el cliente para descargar torrents con `apt install transmission`:
![Imagen ochenta y cuatro del manual para instalar Debian](/img/84.png)

#### [85]  Instalamos el cliente de intercambio de archivos con `apt install amule`:
![Imagen ochenta y cinco del manual para instalar Debian](/img/85.png)

<a name="paso8"></a>
## Instalar el software para ofim&aacute;tica

#### [86]  Instalamos el procesador de textos con `apt install abiword`:
![Imagen ochenta y seis del manual para instalar Debian](/img/86.png)

#### [87]  Instalamos el visor de documentos con `apt install evince`:
![Imagen ochenta y siete del manual para instalar Debian](/img/87.png)

#### [88]  Instalamos la calculadora con `apt install galculator`:
![Imagen ochenta y ocho del manual para instalar Debian](/img/88.png)

#### [89]  Instalamos el programa de dibujo `apt install xpaint`:
![Imagen ochenta y nueve del manual para instalar Debian](/img/89.png)

<a name="paso9"></a>
## Instalar algunos juegos

#### [90]  Instalamos el emulador para dosbox con `apt install dosbox`:
![Imagen noventa del manual para instalar Debian](/img/90.png)

#### [91]  Instalamos el juego vodovod con `apt install vodovod`:
![Imagen noventa y uno del manual para instalar Debian](/img/91.png)

#### [92]  Instalamos el juego gweled con `apt install gweled`:
![Imagen noventa y dos del manual para instalar Debian](/img/92.png)

#### [93]  Instalamos el juego epiphany con `apt install epiphany`:
![Imagen noventa y tres del manual para instalar Debian](/img/93.png)

#### [94]  Instalamos el juego alienblaster con `apt install alienblaster`:
![Imagen noventa y cuatro del manual para instalar Debian](/img/94.png)

<a name="paso10"></a>
## Personalizar LXDE con la apariencia de Microsoft Windows 95

#### [95]  Instalamos el gestor de apariencia de LXDE con `apt install lxappearance`:
![Imagen noventa y cinco del manual para instalar Debian](/img/95.png)

#### [96]  Instalamos la herramienta para personalizar el men&uacute; con `apt install menulibre`:
![Imagen noventa y seis del manual para instalar Debian](/img/96.png)

#### [97]  Colocamos la terminal en el directorio descargas y ejecutamos el comando `wget https://github.com/JulioVillamon/eeePC_701/raw/main/src/eeePC-files.zip`:
![Imagen noventa y siete del manual para instalar Debian](/img/97.png)

#### [98]  Vamos a descargas / clic derecho en el rat&oacute;n / Extraer aqu&iacute;:
![Imagen noventa y ocho del manual para instalar Debian](/img/98.png)

#### [99]  Clic derecho en el escritorio / Preferencias del escritorio en Modo de fondo de escritorio rellenamos con el color de fondo, el corlor de fondo es `#008080`:
![Imagen noventa y nueve del manual para instalar Debian](/img/99.png)

#### [100]  Clic derecho en el escritorio / Iconos del escritorio / Mostrar la carpeta "Documentos" y "Papelera" en el escritorio:
![Imagen cien del manual para instalar Debian](/img/100.png)

#### [101]  Inicio / Preferencias / Personalizar apariencia y comportamiento / Pesta&ntilde;a Control / Redmon, aplicamos el cambio:
![Imagen ciento uno del manual para instalar Debian](/img/101.png)

#### [102]  Doble clic en el archivo Retro-5-Classic-98-ObiWine.obt que est&aacute; en la carpeta OpenBox Theme, dentro de la carpeta eeePC-files:
![Imagen ciento dos del manual para instalar Debian](/img/102.png)

#### [103]  El administrador de Openbox deja una ventana peque&ntilde;a DEBAJO de la ventana grande con el directorio donde lo instala, hay que confirmar el directorio en la ventana peque&ntilde;a:
![Imagen ciento tres del manual para instalar Debian](/img/103.png)

#### [104]  Creamos dentro del directorio /home/user la carpeta .icons (habilitando "Mostrar lo oculto" en el men&uacute; Ver):
![Imagen ciento cuatro del manual para instalar Debian](/img/104.png)

#### [105]  Extraemos dentro de .icons el archivo xcursor-retrosmart.tar.xz que est&aacute; en la carpeta Cursor Theme, dentro de eeePC-files:
![Imagen ciento cinco del manual para instalar Debian](/img/105.png)

#### [106]  Para activarlo vamos a Inicio / Preferencias / Personalizar apariencia y comportamiento / Pesta&tilde;a Cursor del rat&oacute;n, seleccionamos Retrosmart Blanco y reiniciamos:
![Imagen ciento seis del manual para instalar Debian](/img/106.png)

#### [107]  Copiamos la carpeta Classic95 (dentro de Full Icon Theme) que est&aacute; en la carpeta eeePC-files, dentro de .icons:
![Imagen ciento siete del manual para instalar Debian](/img/107.png)

#### [108]  Para activarla vamos a Inicio / Preferencias / Personalizar apariencia y comportamiento / Tema de iconos, seleccionamos Classic95 y aplicamos:
![Imagen ciento ocho del manual para instalar Debian](/img/108.png)

#### [109]  Creamos la carpeta .button dentro de /home/user y guardamos el bot&oacute;n de inicio que está en la carpeta Button dentro de eeePC-files:
![Imagen ciento nueve del manual para instalar Debian](/img/109.png)

#### [110]  Para activarlo clic derecho en el bot&oacute;n de inicio de LXDE / Configuraci&oacute;n de men&uacute; / cambiamos el bot&oacute;n:
![Imagen ciento diez del manual para instalar Debian](/img/110.png)

#### [111]  Para cambiar el color de la barra de herramientas clic derecho sobre la barra de herramientas / Configuraci&oacute;n de panel / Seleccionar Tema del sistema como Fondo:
![Imagen ciento once del manual para instalar Debian](/img/111.png)

#### [112]  Clic derecho en el icono de cerrar sesi&oacute;n / Eliminar Barra de aplicaciones del panel:
![Imagen ciento doce del manual para instalar Debian](/img/112.png)

#### [113]  Clic derecho en el rect&aacute;ngulo negro / Eliminar Monitor de uso de la CPU del panel:
![Imagen ciento trece del manual para instalar Debian](/img/113.png)

#### [114]  Clic derecho en el icono del Gestor de archivos PCManFM / Eliminar barra de aplicaciones del panel:
![Imagen ciento catorce del manual para instalar Debian](/img/114.png)

#### [115]  Clic derecho en el icono de la ventana / Eliminar Minimizar todas las ventanas del panel:
![Imagen ciento quince del manual para instalar Debian](/img/115.png)

#### [116]  Clic derecho en el icono de los escritorios / Eliminar escritorios virtuales del panel:
![Imagen ciento dieciseis del manual para instalar Debian](/img/116.png)

#### [117]  Clic derecho en la barra de herramientas, justo al lado del bot&oacute;n inicio / Configuraci&oacute;n del espaciador (lo dejamos con un valor de 5):
![Imagen ciento diecisiete del manual para instalar Debian](/img/117.png)

#### [118]  Clic derecho en la barra de herramientas / Configuraci&oacute;n del panel / Apariencia / Tipo de lera (Color personalizado a negro):
![Imagen ciento dieciocho del manual para instalar Debian](/img/118.png)

*NOTA: Hay que conectar el netbook a una pantalla externa para poder aplicar los cambios*

#### [119]  Creamos la carpeta .fonts dentro de /home/user y pegamos el archivo windows_command_prompt.ttf que est&aacute; dentro de la carpeta CMD Font:
![Imagen ciento diecinueve del manual para instalar Debian](/img/119.png)

#### [120]  Abrimos la terminal, vamos a editar y en Tipo de letra del terminal cambiamos Monospace Regular por Windows Command Prompt Regular (tama&ntilde;o 13) y el estilo de cursor de bloque a subrayado:
![Imagen ciento veinte del manual para instalar Debian](/img/120.png)

#### [121]  A&ntilde;adimos al final del archivo .bashrc que est&aacute; en /home/user el texto que est&aacute; dentro de la carpeta CMD Font:
![Imagen ciento veintiuno del manual para instalar Debian](/img/121.png)

#### [122]  Con esto tendremos la terminal con el aspecto de la consola de Windows 95:
![Imagen ciento veintidos del manual para instalar Debian](/img/122.png)













































