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
![Imagen ocho del manual para instalar Debian](/img/11.png)

#### [12] Nos pide que la verifiquemos:
![Imagen ocho del manual para instalar Debian](/img/12.png)

#### [13] Le damos un nombre al usuario del sistema (por seguridad, para usar Debian sin ser administrador):
![Imagen ocho del manual para instalar Debian](/img/13.png)

#### [14] Nos pide verificar el nombre del nuevo usuario:
![Imagen ocho del manual para instalar Debian](/img/14.png)

#### [15] Damos una contrase&ntilde;a al nuevo usuario:
![Imagen ocho del manual para instalar Debian](/img/15.png)

#### [16] Y la verificamos:
![Imagen ocho del manual para instalar Debian](/img/16.png)

#### [17] Seleccionamos nuestra zona horaria:
![Imagen ocho del manual para instalar Debian](/img/17.png)

#### [18] Comienza la detecci&oacute;n de los discos y del hardware:
![Imagen ocho del manual para instalar Debian](/img/18.png)

#### [19] En particionado de discos elegimos "Manual" (tecla "enter" para aceptar):
![Imagen ocho del manual para instalar Debian](/img/19.png)

#### [20] sda es el disco duro interno de 4 GB:
![Imagen ocho del manual para instalar Debian](/img/20.png)

#### [21] sdb es la memoria que hemos conectado por usb con el instalador de Debian:
![Imagen ocho del manual para instalar Debian](/img/21.png)

#### [22] sdc es la la tarjeta de memoria de 32 GB:
![Imagen ocho del manual para instalar Debian](/img/22.png)

#### [23] Seleccionamos el espacio libre del disco duro y elegimos "Crear una partici&oacute;n nueva":
![Imagen ocho del manual para instalar Debian](/img/23.png)

#### [24] Le damos 3.8 GB y continuamos:
![Imagen ocho del manual para instalar Debian](/img/24.png)

#### [25] Elegimos Primaria:
![Imagen ocho del manual para instalar Debian](/img/25.png)

#### [26] La ubicamos al principio:
![Imagen ocho del manual para instalar Debian](/img/26.png)

#### [27] Dejamos el resto de opciones como est&aacute;n y seleccionamos "Se ha terminado de definir la partici&oacute;n":
![Imagen ocho del manual para instalar Debian](/img/27.png)

#### [28] Seleccionamos el espacio libre que nos queda en el disco sda:
![Imagen ocho del manual para instalar Debian](/img/28.png)

#### [29] Creamos una partici&oacute;n nueva:
![Imagen ocho del manual para instalar Debian](/img/29.png)

#### [30] Dejamos el tama&ntilde;o restante y continuamos:
![Imagen ocho del manual para instalar Debian](/img/30.png)














































