# Instalación-Sistemas-Operativos



![ÍNDICE](https://user-images.githubusercontent.com/89795512/132549498-85922375-6c1f-4621-893c-c788814fc22c.png)


<h3>1.1 Instalar un Sistema Operativo</h3>

    1.2. Requisitos mínimos	
    1.3. Selección del Sistema Operativo Windows	
    1.4. Ediciones de Windows 10	
    1.5. Requisitos técnicos del Sistema Operativo
    
 <h3>2.1 Planificación de la instalación</h3>
 
    2.2. Soporte utilizado para la instalación	
    2.3. Particionamiento del disco	
    2.4. Esquema de particiones Master Boot Record	
    2.5. Esquema de particiones de tabla de partición GUID (GPT)	
    2.6. Preparar las particiones de los S.O. para permitir su arranque.	
    2.7. Administrar particiones en Windows de forma gráfica	
    2.8. Administrar particiones en Windows por comandos	
    
<h3>3.1 Sistemas de ficheros</h3>	

    3.2. FAT32	
    3.3. NFTS	
    3.4. exFAT	
    3.5. HFS+	
    3.6. Formatear discos en Windows
      
<h3>4.1 Gestores de arranque</h3>

    4.2. Bootmgr	
    4.3. Secuencia de arranque en Windows 7	
    4.4. Secuencia de arranque seguro en Windows 8.1 y superiores	
    4.5. Reparación de MBR	
    4.6. Reparación de EFI Bootloader	
    4.7. Modo seguro	
  
  
<h3>Tipos de instalaciones</h3>

    5.2. Manual	
    5.3. Desatendida	
    5.4. En red por imágenes	
    5.5. En red por servidores	

Documentación de la instalación	
Configuración posteriores a la instalación



 <br>

 <br>
 
 <br>
  
  
![INSTALACION-SOV 2](https://user-images.githubusercontent.com/89795512/132555599-0940007f-9db7-423b-99d1-034a34e4e0fd.png)
					######## 1.1 Instalar un Sistema Operativo ######## 

					   
  
Después de conocer las técnicas básicas que utilizan los SSOO para gestionar los recursos de hardware, es hora de aprender a instalar un sistema operativo.
En esta unidad voy explicar los pasos necesarios para la instalación de los sistemas operativos monousuarios propietarios más extendidos hoy en día, los de Microsoft Windows.

Una familia de SSOO está formada por versiones antiguas del sistema que han dejado de recibir soporte técnico por parte de la propietaria del producto; solamente la versión más reciente incorpora todas las mejoras técnicas que se han implementado por avances del hardware o mejoras de los desarrolladores del software. Por esta razón, aunque parece que existen muchísimos SSOO en el mercado, solo están disponibles las versiones más recientes. 

Por ejemplo, en el caso de Apple tenemos el macOS Big Sur como versión más reciente para ordenadores y iOS 14 para móviles y tabletas.
Microsoft actualmente tiene como versión más reciente Windows 10 tanto para ordenadores como dispositivos móviles.

<br>
<br>

**   <b>  1.2. Requisitos mínimos </b>
![REQUISITOS-MINIMOS](https://user-images.githubusercontent.com/89795512/132554418-d61d1cdf-430f-4bf4-87fd-b457c8131b06.png)


Los Sistemas Operativos necesitan unas características mínimas y recomendadas:

    • Velocidad de CPU mínima, recomendada y óptima
    • Memoria RAM mínima, recomendada, óptimo y máxima
    • Espacio en disco mínimo, recomendado y óptimo
    • Acceso a Internet
    • Etc.

    (Estas características varían en función de la configuración del sistema 
     y de las aplicaciones y características que se instalen.)
	
Para llevar a cabo la instalación de Microsoft Windows tendremos en cuenta las siguientes indicaciones:


    1. Selección de la edición del SSOO Windows 
    2. Comprensión de las  normas del uso del software: licencia
    3. Cumplimiento de los requisitos del hardware específicos para la instalación:
        ◦ Requisitos mínimos y recomendados
        ◦ Lista de compatibilidad del hardware (HCL)
        ◦ Actualización de controladores
        ◦ Compatibilidad de la BIOS/UEFI
    4. Planificación de la instalación: particiones y sistema de archivos
        ◦ ¿Instalar o actualizar?
        ◦ Requisitos de actualización
    5. Instalación de Windows
        ◦ Modos y fases de instalación
        ◦ Proceso de instalación del sistema
    6. Acciones prioritarias de configuración tras la instalación del Sistema Operativo.
        ◦ Configuración de la red (IP, máscara, puerta de enlace etc.)
        ◦ Nombre del equipo y grupo de trabajo
        ◦ Activación de Windows
        ◦ Actualización mediante Windows Update
        ◦ Instalación de los service packs
        ◦ Configuración básica de seguridad
            ▪ Deshabilitar la cuenta “invitado”
            ▪ Firewall de Windows
            ▪ Antivirus y antispyware: Windows Defender
        ◦ Limitación del número de programas que se ejecutan al arrancar el sistema


<br>
<br>

 **   <b> 1.3. Selección del Sistema Operativo Windows </b>
 ![SELECCION-S O](https://user-images.githubusercontent.com/89795512/132552742-80c56d8a-4703-4ca3-919f-5f1249d3dc13.png)


En la página oficial del Sistema Operativo Windows de Microsoft tenemos información oficial del producto: 
https://www.microsoft.com/es-es/windows

En esta página podemos consultar una tabla comparativa de sus diversas versiones y ediciones para poder evaluar cuál resulta más adecuado para instalar o actualizar en nuestro sistema informático.

En la siguiente tabla mostramos las diferencias más importantes entre las distintas versiones de Windows 7, 8.1 y 10, que hemos obtenido de https://www.microsoft.com/es-es/windows/compare


<br>
<br>

**   <b> 1.4. Ediciones de Windows 10 </b>

Microsoft Windows 10 dispone de 4 ediciones, en la página https://www.microsoft.com/es-es/WindowsForBusiness/Compare podemos comparar las diferencias entre cada una de ellas en los apartados de productividad, administración, seguridad y características básicas.

Es recomendable elegir la edición que facilite las tareas de administración del SO una vez instalado.

Estas tareas dependerá de donde se utilice el equipo, no es lo mismo un ordenador de casa, que el de una oficina de una pyme o una gran empresa. La posibilidad de administrar los equipos de una red de manera remota y de centralizar esta tarea se implementa utilizando varias tecnologías, pero el primer paso es que el SO permite esta administración. 

    • Home: para configurar un pc doméstico que será administrado por un usuario sin conocimientos avanzados de         	informática.
    • Pro o Enterprise: para configurar un PC de una red de ordenadores que se necesita ser administrada de manera 		centralizada (Unión a Dominio y escritorio remoto)
    • Education: Para alumnos que esté estudiando por un tiempo determinado y quieran aprender a configurar equipos a 		nivel avanzado.

       
    
<br>
<br>

**   <b> 1.5. Requisitos técnicos del Sistema Operativo </b>

Todos los Sistemas Operativos necesitan de una configuración mínima de hardware para poder ejecutarlo de manera eficiente. Con el tiempo nos podemos encontrar con ordenadores y móviles que funcionan correctamente pero que no son los suficiente potentes para ejecutar los últimos SO y quedan obsoletos. Los programadores añaden nuevas características a sus Sistemas Operativos y programas según los avances tecnológicos, pero muchos ordenadores no pueden ejecutar estos nuevos SO y programas de forma eficiente, por lo que están obligados a adquirir equipos nuevos para utilizar los últimos productos.

Esto fue algo notable con la versión de Windows Vista que aumento los requisitos de forma tan drástica que muchos equipos que tenían instalado windows XP no podían actualizarse, por lo que se prolongó durante mucho tiempo el soporte a este sistema operativo.


Los Sistemas Operativos Windows 7, 8.1 y 10 tienen los siguientes requisitos mínimos:


   SO    Windows 10               
   
    Procesador: 1 GHz 32 o 64 bits          
    Memoria RAM: 2 GiB       
    Disco duro: 16 GiB (32 bits) 20 GiB (64 bits)         
    Adaptador de vídeo: DirectX 9 o posterior con un controlador WDDM 1.0
                                

Windows 10 además añade algunos requisitos extra para utilizar algunas características:

    • Cortana necesita un Micrófono 
    • Windows Hello requiere una cámara por infrarrojos con iluminación especial para 
      el reconocimiento facial o un lector de huellas dactilares compatible con la plataforma de datos biométricos de Windows
    • Para el uso táctil, necesitas una tableta o un monitor que sea compatible con la función multitáctil.
    • Para un arranque seguro se requiere firmware compatible con UEFI v2.3.1 Errata B y con la entidad 
      de certificación de Microsoft Windows en la base de datos de firmas UEFI.
    • El cliente Hyper-V requiere un sistema de 64 bits con servicios de traducción 
      de direcciones de segundo nivel (SLAT) y 2 GB de RAM adicionales (solo para Windows 10 Pro y Windows 10 Enterprise).
    • Para instalar un sistema operativo de 64 bits en un equipo de 64 bits, 
      el procesador tiene que ser compatible con CMPXCHG16b,         PrefetchW y LAHF/SAHF.
    • BitLocker requiere el Módulo de plataforma segura (TPM) 1.2, TPM 2.0 o una unidad flash USB 
      (solo para Windows 10 Pro y Windows 10 Enterprise).


<b> Actualización de controladores </b>

Cuando un controlador de un dispositivo supera las pruebas de compatibilidad, se incluye en el programa de certificación y se publica en el sistema de distribución de drivers de Microsoft. Esto supone:

    • El driver puede ser añadido al DVD o imagen de la instalación de Windows.
    • El driver puede ser descargado desde el servicio Windows Update, un recurso en Internet al que se conecta 
      el sistema operativo si necesita un controlador que no encuentra en \Windows\System32\DriverStore, 
      donde Windows almacena los drivers.

En caso de que Windows no encuentre el driver, tendremos que ir a la web del fabricante del hardware y descargar el controlador para nuestra versión de Windows.


 <br>

 <br>
 
 <br>
 
 
 
                                              ######## 2.1 Planificación de la instalación ######## 
					     

Antes de empezar la instalación del Sistema Operativo en el ordenador es conveniente planificar el proceso por los siguientes motivos:

    • No ejecutar acciones que conlleven la pérdida de información de los usuarios de la máquina
    • No perder tiempo durante el procedimiento debido a no haber preparado de antemano las utilidades de software y periféricos  
      hardware necesarios para llevar a cabo la instalación y proteger la información.

La primera decisión a tomar es si actualizamos el sistema operativo existente en la máquina o realizamos una nueva instalación

 <br>

<h3>Instalar o actualizar</h3>

Previamente debemos saber si el ordenador de destino tiene instalado un sistema operativo desde el que es posible actualizar Windows. Una nueva instalación suponer formatear las particiones existentes (incluso modificar la tabla de particiones)y volver a generar el sistema de archivos.

Si actualizamos un sistema operativo previamente instalado en la máquina de destino, logramos lo siguiente:

    • Mantener las aplicaciones (programas) instalados en el sistema
    • Mantener las cuentas de usuario del sistema
    • Mantener los archivos de los usuarios del sistema
    • Mantener la configuración y preferencias del sistema.

Si realizamos una nueva instalación del sistema operativo, conseguimos:

    • Eliminar los programas e información de los usuarios del sistema
    • Generar de nuevo el sistema de archivos
    • Hacer posible que se configure el arranque dual de la máquina entre windows y otro sistema operativo más reciente.


Los sistemas operativos Windows se degradan con el uso del sistema de archivos debido a problemas como la fragmentación interna y externa del sistema de archivos, las desisntalaciones de programas que no se hayan realizado limpias y que ensucian el registro del sistema, o la instalación de un número muy elevado de aplicaciones.

La solución más drástica a este problema es formatear y reinstalar el sistema operativo.



<b>Degradación del sistema de archivos</b>

	Los sistemas operativos Windows se degradan con el uso del sistema de archivos debido a problemas como 
	la fragmentación interna y externa del sistema de archivos, las desisntalaciones de programas que no se hayan realizado 
	limpias y que ensucian el registro del sistema, o la instalación de un número muy elevado de aplicaciones.


 <br>
 <br>

<b>** 2.2. Soporte utilizado para la instalación</b>

 • Desde una unidad DVD del propio equipo: es la forma más común de iniciar 
 la instalación y puede hacerse de dos 	maneras
 
        ◦ Iniciando el ordenador desde una unidad DVD de un ordenador limpio
        ◦ Iniciando el ordenador desde otro SO
	
• Desde un Pendrive: muchos equipos no disponen de unidades DVD por lo que es necesario instalarlo desde un pendrive. Puede hacerse de dos maneras

        ◦ Utilizar una versión portable que permite ejecutar el SO desde el mismo USB
        ◦ Preparar una unidad USB para arrancar una instalación del Sistema Operativo
	
• Desde un recurso compartido de la red. Utilizando un equipo que ya cuenta con otro sistema operativo



<b>** 2.3. Particionamiento del disco </b>


Es el acto de dividir un disco duro en múltiples unidades lógicas llamadas particiones. Cada partición es tratada como una unidad física. En algunos Sistemas Operativos basados en BSD, Solaris o GNU Hurd las particiones son llamadas "trozos" (slices).

Un programa de particionado en el disco puede ser usado para crear, cambiar de tamaño, borrar o manipular estas particiones.

Las principales ventajas de utilizar particiones:

    • Separación del Sistema Operativo de los programas y ficheros del usuario
      Esto permite copias de seguridad o clones de sólo el SO
    • Tener un área separada del SO para la memoria virtual
    • Mantener cerca los programas y datos usados frecuentemente
    • Mantener ficheros cache y logs separados de otros ficheros
      Estos pueden crecer rápidamente, pudiendo llenar el disco entero
    • Permite instalar varios SO incompatibles (Ej. Linux, Mac OS X y Windows en distintas particiones)
    • Proteger y aislar ficheros, para hacer más fácil la recuperación de un sistema de ficheros o SO
    • Mejora del rendimiento en sistemas donde es más eficiente sistemas de ficheros 
      más pequeños. Por ejemplo NTFS es más eficiente en discos duros de gran capacidad 
      si se divide en particiones.
    
Las desventajas de utilizar particiones:

    • Reduce el espacio disponible al tener que duplicar el SO áreas de administración en cada partición
    • Puede reducir el rendimiento en sistemas donde los datos 
      son accedidos regularmente en paralelo o en particiones múltiples
    • Reduce la eficacia de los optimizadores del disco para reducir el número y 
      distancia de movimientos del cabezal 
    • Incrementa la fragmentación del disco porque reduce la media de bloques libres 
      seguidos en cada partición
    • No se aprovecha todo el espacio libre del disco. 
      Por ejemplo, en 2 particiones libres de 3GB, no cabe un DVD de 4GB
    • Se requiere más tiempo para mover datos entre las diferentes partes del disco duro físico.


<b>** 2.4. Esquema de particiones Master Boot Record </b>

Es un tipo de bloque de arranque popularizado por IBM. Fue utilizado históricamente por  DOS, Microsoft Windows y Linux y otros sistemas operativos compatibles con PC. 


<b>Partición primaria</b>

Son las divisiones crudas del disco. Solo puede haber 4 en controladores IDE (15 en discos SCSI) de éstas o 3 primarias y una extendida. Depende de una tabla de particiones 

<b>Partición extendida o secundaria</b>

Actúa como una partición primaria; sirve para contener infinidad de unidades lógicas en su interior. 
Fue ideada para romper la limitación de 4 particiones primarias en un solo disco físico. Solo puede existir una partición de este tipo por disco y solo sirve para contener particiones lógicas.

<b>Partición lógica</b>
Ocupa una porción de la partición extendida o la totalidad de la misma.
Se formatea con un tipo específico de sistema de archivos (FAT32, NTFS,...) y se le asigna una unidad. 
No se puede instalar un Sistema Operativo en una partición lógica.

![Sistema Particiones](https://user-images.githubusercontent.com/89795512/132535206-31da8ad4-6ecb-460e-8540-9ddc5056b8fd.jpg)


<br>
<br>


<b>** 2.5. Esquema de particiones de tabla de partición GUID (GPT)</b>

Hoy en día todos los Sistemas Operativos soportan. Es parte del estándar  Unified Extensible Firmware Interface (EFI) propuesto por Intel para reemplazar la vieja BIOS del PC.

La GPT sustituye al Master Boot Record (MBR) usado con la BIOS. Se basa en las capacidades extendidas del EFI para estos procesos. 

Las principales ventajas de GPT frente a MBR son:

    • Admite discos de más de 2 TB hasta teóricamente 2 ZB ( 2*109 TB).
    • No es necesario crear particiones extendidas ni lógicas, por defecto admite hasta 128 particiones.
    • Almacena una copia de seguridad del encabezado y de la tabla de particiones al final del disco que ayuda en la recuperación 
      en el caso de que los primeros están dañados.
    • Checksum CRC32 para detectar errores y daños de la cabecera y en la tabla de particiones al proporcionar redundancia.
   
![GPT](https://user-images.githubusercontent.com/89795512/132539970-90e9c8ac-5fbf-4f07-8bc2-b28ed0134e24.jpg)

 <br>
 <br>


<b>** 2.6. Preparar las particiones de los S.O. para permitir su arranque.</b>

Para que un disco sea bootable debe tener debe contener:

    • Una tabla de particiones GUID
    • Al menos una partición
    • Una entrada en su GPT

La GPT es creada por un programa especial que se encarga de crear las particiones en el disco. En windows diskpart.exe.

El código del bootstrap loader es instalado por el programa de instalación del Sistema Operativo.

Para las instalaciones nuevas, el programa de instalación de Windows creará, de forma predeterminada, una partición de sistema Extensible Firmware Interface (partición de sistema EFI o ESP), una partición reservada de Microsoft® (MSR) y una partición principal de Windows.

![EFI](https://user-images.githubusercontent.com/89795512/132541447-f1529ccc-2afc-4e1a-8173-12660bf58320.PNG)


La instalación de Windows crea una partición ESP en el equipo cuando:
	
	• No existe una partición ESP.
	• Hay suficiente espacio en disco para crear una partición de 100 MB.

La instalación de Windows crea la partición MSR cuando:

    • No existe una partición MSR.
    • Hay suficiente espacio en disco para crear una partición de 128 MB.

La creación de la partición ESP tiene prioridad sobre la partición MSR porque la partición ESP es necesaria para arrancar el equipo.

<br>
<br>

** <b>2.7. Administrar particiones en Windows de forma gráfica</b>

En Windows podemos configurar los discos en dos tipos:

    • Disco básico: es un disco físico que contiene particiones primarias, extendidas o dispositivos lógicos (volúmenes básicos).

    • Disco dinámico: es un disco físico que contiene volúmenes dinámicos.

Convertir discos básicos a dinámicos en Windows

Condiciones:

    • Disponer al menos 1 MB libre al final del disco
    • Cerrar todos los programas ejecutados en ellos
    • No puede ser un medio extraible (pendrive)
    • No puede ser un disco duro externo que utilice USB o Firewire

Una vez convertido, no se podrá convertir los volúmenes dinámicos en particiones, no podrá contener particiones ni unidades lógicas, tampoco se  tendrá acceso desde MS-DOS o Windows anteriores a Windows 2000. Todas las particiones se convertirán en volúmenes simples

Para realizar la conversión tenemos realizar lo siguiente:

    1. Ir al Administrador de discos
    2. Seleccionar el disco que se desea actualizar, en su menú contextual, seleccionar convertir en disco dinámico
    3. Seleccionar los discos que se desea actualizar y pulsar aceptar
    
	Cuando esté preparado, pulsar en convertir, mostrará una ventana de aviso, pulsar Sí

    4. Si hay una partición en uso, mostrará un mensaje indicando que se desmontarán, pulsar sí
    5. Mostrará un aviso de que se reiniciará el equipo para completar el proceso. Pulsar Aceptar.
    6. Si volvemos al administrador de discos, mostrará el disco convertido en dinámico.
    
![ad equipos](https://user-images.githubusercontent.com/89795512/132541689-0b3de9dd-6307-4780-b5ae-361d4818325b.PNG)


<b>Convertir dinámicos a discos básicos en Windows</b>


Condiciones:

    • Realizar una copia de seguridad o mover los datos
    • El disco no puede contener datos
    • No se pueden cambiar los volúmenes dinámicos en particiones
    • Hay que borrar todos los volúmenes del disco dinámico

Una vez convertido, solo se podrán crear particiones y unidades lógicas 

Para realizar la conversión tenemos realizar lo siguiente:

    1. Ir al Administrador de discos
    2. Seleccionar el disco que se desea convertir
    3. Situarse en uno de los volúmenes que contenga y mostrar el menú contextual, seleccionar Eliminar volumen y confirmar.
    4. Repetir el proceso con todos los volúmenes que contenga
    5. Cuando no quede ningún volumen automáticamente se convertirá en disco básico. En caso contrario mostrar el menu contextual y seleccionar Convertir en disco básico
    6. Una vez finalizado, crear las particiones que desees

Crear un volumen simple de forma gráfica

    1. Ir al Administrador de discos y seleccionar el espacio no asignado de un disco dinámico y pulsar el botón derecho para mostrar el menú contextual
    2. Seleccionar Nuevo volumen simple (Nuevo volumen en Windows server 2003) y pulsar siguiente
    3. Elegir Simple y pulsar siguiente
    4. En la pantalla, indicar que tamaño tendrá el volumen y pulsar siguiente
    5. Asignar una letra de unidad al volumen que está creando o montar la unidad en una carpeta NTFS
    6. Pulsar siguiente  y en la pantalla indicar si desea formatear el volumen. 
    7. Pulsar siguiente
    8. Verificar que todo es correcto y pulsar finalizar

![volumen](https://user-images.githubusercontent.com/89795512/132542311-6e301fd5-b9a2-4516-94ae-0374878fb5cc.PNG)


<b>Extender un volumen de forma gráfica</b>
	

    1. Ir al Administrador de discos y seleccionar el volumen que quieras extender, pulsar el botón derecho para mostrar el menú contextual y selecciona Extender volumen
    2. Pulsa siguiente y verás una pantalla en la que se ven los discos que tienen espacio sin asignar, selecciona el disco o discos donde vas a extender el volumen y el tamaño          que vas a utilizar en cada uno de ellos.
    3. Después pulsa siguiente y verás la pantalla de finalización del asistente con un resumen
    4. Pulsar Finalizar y se extenderá el volumen.

<b>Reducir un volumen (windows 10 y server 2012)</b>

    1. Ir al Administrador de discos y seleccionar el volumen que quieras reducir, pulsar el botón derecho para mostrar el menú contextual y selecciona reducir volumen
    2. En el apartado Tamaño del espacio que desea reducir, indicamos el tamaño que queremos disminuir del que tiene actualmente el volumen (si el volumen ocupaba más de un disco, 	   puede reducirse a menos discos).
    3. Cuando lo hayamos indicado, pulsamos reducir y se reducirá el tamaño del volumen
    
    
<b>Volúmenes distribuidos</b>

Un volumen distribuido lo forman la unión de dos o más áreas de espacio no asignado que están en dos o más discos duros. Cuando se guardan datos en un volumen distribuido, primero se ocupa el espacio libre del primer disco, cuando éste se ha llenado se pasa al segundo y así sucesivamente. Esto permite aprovechar pequeñas partes del espacio libre para formar un volumen de gran tamaño, ¡pero cuidado! si falla una parte del disco, se perderá toda la información del volumen. En cada disco se creará un volumen y cada uno tend

Para crear un volumen distribuido necesitaremos al menos dos discos duros con espacio sin asignar en cada uno de ellos.
	
    1. Ir al Administrador de discos y seleccionar el disco donde que quieras crear el volumen distribuido
    2. Mostrar el menú contextual y seleccionar Nuevo volumen distribuido
    3. Pulsar siguiente y aparecerá el asistente para volumen nuevo
    4. Seleccionar el disco o discos e indicar el tamaño del volumen distribuido
    5. Pulsar siguiente
	
<br>	
<br>

<b> ** 2.8. Administrar particiones en Windows por comandos</b>

Diskpart es una herramienta de línea de comandos incluida a partir del Windows 2000 en adelante para sustituir a fdisk. Diskpart soporta el uso de scripts para automatizar el uso mediante el comando diskpart /s nombrescript.txt.

    • Para ejecutar diskpart dirígete a Inicio -> Ejecutar y escribe cmd.
    • En la línea de comandos escribe diskpart.
    • Para conseguir una lista de los comandos disponibles en diskpart  usa el comando ? ó help.
    • Para mostrar todos los discos usamos el comando list disk
    
    
 Discos básicos

    • Crear partición primaria: create partition primary [size=n] 
    • Escribe list partition para mostrar las particiones existentes en el equipo.
    • Crear partición extendida create partition extended [size=n] 
    • Crear partición lógica create partition logical [size=n] 
    • Asignar una letra a la partición assign letter=H
    • Buscar dispositivos nuevos Rescan.
    • Borra todos los datos y particiones del disco. Clean all
    • Quitar una letra de una partición. Remove 
    
 Discos dinámicos

    • Crear un volumen simple: create volume simple [size=n] [disk=n]
    • Escribe list volume para mostrar los volúmenes existentes en el equipo.
    • Escribe Select volume <número de volumen> donde número de volumen es el número del volumen que quieras seleccionar
    • Escribe extend [size=m] [disk=n]  para extender el volumen seleccionado al disco n con tamaño m MB
    • Escribe shrink [desired=n] [minimun=m]  para reducir el volumen seleccionado n MB con un tamaño mínimo de m MB
    • Escribe delete volume <número de volumen> para eliminar el volumen

Más opciones del comando diskpart https://technet.microsoft.com/es-es/library/cc766465(v=ws.10).aspx





<br>
<br>
<br>


							
							######## 3.1 Sistemas de Ficheros ########
    

Los archivos están almacenados en soportes de almacenamiento permanente. El SO los manipula a través de herramientas como el gestor de archivos.

A nivel de programas, un archivo es una secuencia de bytes sin orden o agrupados en registros. Como se almacenan en dispositivos orientados a bloques, los archivos o ficheros están compuestos de bloques de tamaño fijo, normalmente 512 bytes. El sistema de archivos permite la organización de estos bloques en archivos o directorios. Guarda, además, la información de qué bloques pertenecen a qué archivos y cuáles están libres.

El sistema de ficheros debe ofrecer los siguientes servicios:

    • Seguridad y permisos.
    • Mecanismos para evitar la fragmentación
    • Capacidad de enlaces simbólicos o duros
    • Integridad de archivos
    • Soporte para archivos dispersos
    • Cuotas de disco
    • Soportar el crecimiento del sistema de archivos.
    • Caches de disco
    
Los discos tienen su propia caché, pero el SO puede implementar una caché en memoria principal para no tener que hacer tantas peticiones al disco. La gestión de la caché es similar a la gestión de la memoria. Hay dos maneras de comunicar la caché con el disco:

    • Escritura diferida, en la que se escribe en caché para luego pasar al disco
    • Escritura directa, en la que se escribe en la caché y el disco a la vez

La caché mejora considerablemente el rendimiento del sistema.

El tamaño medio que ocupan los archivos en Linux y Windows es de 1KB, por lo que se recomienda bloques de tamaño de 512 bytes, 1 KB o 2 KB en discos de hasta 16 TB.
Si el disco es de gran capacidad, se utilizarán bloques de 8KB ( 16-32TB) a 64KB (>256TB). Si se elige un tamaño de bloque de 2KB en un disco con 512 bytes de tamaño de sector, cada bloque estará formado por 4 sectores.
Algunos sistemas de archivos modernos utilizan extends. Son un conjunto de bloques contiguos reservados para un fichero para mejorar el rendimiento y reducir la fragmentación


 <br>
 <br>

<b>** 3.2. FAT32</b>

Este formato es el más antiguo de todos, y lleva presente entre nosotros desde el lanzamiento de Windows 95, el cual fue desarrollado para sustituir al anterior FAT16.

Ser el formato más antiguo tiene sus ventajas, por ejemplo, que prácticamente cualquier dispositivo va a ser compatible con él, especialmente si estamos hablando de compartir archivos entre dos ordenadores. Por ejemplo, es posible copiar un archivo en una memoria USB formateada en FAT32 desde Windows y leer su contenido, por ejemplo, en un televisor, un móvil o una videoconsola, los cuales probablemente no sean compatibles con el privativo NTFS.

Sin embargo, este sistema antiguo tiene una limitación muy grave, y es que no puede almacenar archivos de más de 4 GB. Mientras los archivos sean menores de ese tamaño, o estén divididos, no hay problema, sin embargo, si intentamos copiar un archivo de más de dicho tamaño obtendremos un error. Otra limitación, aunque menos importante, es que las particiones en FAT32 no pueden ser mayores de 8 TB.

El uso ideal de FAT32 es para memorias externas donde no vayamos a guardar archivos mayores de 4GB y queramos asegurarnos que es compatible con prácticamente todo tipo de dispositivos.

 <br>
 <br>

<b>** 4.2. NFTS</b>

Este formato es el sucesor de FAT32, desarrollado por Microsoft. NTFS elimina las dos limitaciones de FAT32 (los 4GB y los 8TB). Este formato de archivos también incluye una serie de novedades y mejoras necesarias para que los sistemas operativos modernos puedan funcionar sin problema y, sobre todo, en temas de seguridad, entre otras:

    • Escalabilidad: Teóricamente soporta volúmenes de hasta 16 EB
    • Journaling: Crear y guardar un diario de cambios que nos pueden ayudar a recuperarnos rápidamente de los errores si el ordenador se bloquea.
    • Compresión
    • Cifrado: Encrypting File System (EFS)
    • Cuotas
    • Redimensionamiento
    • Seguridad: Posibilidad de configurar permisos de archivo.
    • Volume Shadow Copy  (VSS): Soporta la creación de copias de seguridad instantáneas.

Sin embargo, aunque a nivel lógico NTFS es un sistema de archivos muy avanzado y prácticamente sin limitaciones (a día de hoy), tiene el principal inconveniente de la compatibilidad. Todos los sistemas operativos modernos de Windows funcionan perfectamente con NTFS, sin embargo, si vamos a utilizar otros sistemas como Mac OS X o Linux es posible que tengamos dificultad para leer y, sobre todo, escribir datos en estas unidades, salvo que utilicemos software de terceros. Igualmente es muy probable que en muchos dispositivos (móviles, televisores, reproductores multimedia, etc) no sean compatibles con este formato de archivos, por lo que de conectar una unidad NTFS a estos equipos no compatibles nos devolverá un error, en el mejor de los casos.

Este formato es el ideal para trabajar con discos duros internos que vayamos a utilizar con Windows.
    
 <br>
 <br>
 
<b>** 4.3. exFAT</b>

	exFAT vio la luz en 2006 y se introdujo en la mayoría de los sistemas operativos modernos, incluido Windows XP. Este sistema de archivos está pensado para unidades flash, siendo un sistema mucho más liviano que NTFS, sin las características de seguridad de este, pero también sin las limitaciones de FAT32.

	Todos los sistemas operativos de PC (Windows, Mac y Linux (aunque en este es posible que tengamos que instalar algunas librerías)) son compatibles de forma nativa con exFAT, al contrario que con NTFS. Este formato de archivos también es compatible con un gran número de dispositivos (televisiones, reproductores multimedia, videoconsolas, etc), aunque no llega al nivel de compatibilidad de FAT32.

	exFAT podría definirse como una actualización de FAT32 donde prima principalmente la compatibilidad y sencillez del formato de archivos, aunque eliminando las restricciones de los 4GB por archivo y 8 TB de tamaño máximo de partición.

	El uso recomendado para exFAT es para unidades externas (generalmente memorias USB o tarjetas SD) donde vayamos a guardar archivos de más de 4 GB y que queramos que sea compatible con el mayor número de dispositivos posibles. Si no vamos a guardar archivos de más de 4 GB en esas unidades, mejor optar por FAT32.  
