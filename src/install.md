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
[Instalaci&oacute;n de Debian 12 sin escritorio](#paso1)  
[Instalaci&oacute;n del escritorio LXDE](#paso2)   
[Instalaci&oacute;n de las utilidades del sistema](#paso3)  
[Instalaci&oacute;n del sonido](#paso4)  
[Instalaci&oacute;n de los Codecs](#paso5)  
[Instalaci&oacute;n del software multimedia](#paso6)  
[Instalaci&oacute;n del software para internet](#paso7)  
[Instalaci&oacute;n del software para ofim&aacute;tica](#paso8)  
[Instalaci&oacute;n de juegos](#paso9)  
[Personalizaci&oacute;n con la apariencia de Microsoft Windows 95](#paso10)

<a name="paso0"></a>
## Crear medio de arranque
*NOTA: Para crear la unidad USB arrancable se usa el programa Rufus usando un sistema operativo Windows*
1. Descargamos el programa Rufus desde su direcci&oacute;n: [https://rufus.ie/es/](https://rufus.ie/es/)
2. Descargamos la imagen de instalaci&oacute;n "iso netinst para PC de 32 bits" desde la web de Debian: [https://www.debian.org/distrib/](https://www.debian.org/distrib/)
3. Grabamos la imagen en una memoria USB con capacidad suficiente (como m&iacute;nimo de 2 GB) con las siguientes opciones:  
d
