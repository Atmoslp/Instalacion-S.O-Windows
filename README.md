# Instalación Sistemas Operativos (Windows)



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
    4.3. Reparación de MBR	
    4.4. Reparación de EFI Bootloader	
    4.5. Modo seguro	
  
  
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


![requisitos](https://user-images.githubusercontent.com/89795512/132556850-fb0775d1-134b-47e9-9d92-ecd821cd6640.png)

<b> ** 1.2. Requisitos mínimos </b>



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

 <b> ** 1.3. Selección del Sistema Operativo Windows </b>
 ![SELECCION-S O](https://user-images.githubusercontent.com/89795512/132552742-80c56d8a-4703-4ca3-919f-5f1249d3dc13.png)


En la página oficial del Sistema Operativo Windows de Microsoft tenemos información oficial del producto: 
https://www.microsoft.com/es-es/windows

En esta página podemos consultar una tabla comparativa de sus diversas versiones y ediciones para poder evaluar cuál resulta más adecuado para instalar o actualizar en nuestro sistema informático.

En la siguiente tabla mostramos las diferencias más importantes entre las distintas versiones de Windows 7, 8.1 y 10, que hemos obtenido de https://www.microsoft.com/es-es/windows/compare


<br>
<br>

<b> ** 1.4. Ediciones de Windows 10 </b>

Microsoft Windows 10 dispone de 4 ediciones, en la página https://www.microsoft.com/es-es/WindowsForBusiness/Compare podemos comparar las diferencias entre cada una de ellas en los apartados de productividad, administración, seguridad y características básicas.

Es recomendable elegir la edición que facilite las tareas de administración del SO una vez instalado.

Estas tareas dependerá de donde se utilice el equipo, no es lo mismo un ordenador de casa, que el de una oficina de una pyme o una gran empresa. La posibilidad de administrar los equipos de una red de manera remota y de centralizar esta tarea se implementa utilizando varias tecnologías, pero el primer paso es que el SO permite esta administración. 

    • Home: para configurar un pc doméstico que será administrado por un usuario sin conocimientos avanzados de informática.
    • Pro o Enterprise: para configurar un PC de una red de ordenadores que se necesita ser administrada de manera centralizada 
    • Education: Para alumnos que esté estudiando por un tiempo determinado y quieran aprender a configurar equipos a nivel avanzado.

       
    
<br>
<br>

<b> ** 1.5. Requisitos técnicos del Sistema Operativo </b>

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
      el procesador tiene que ser compatible con CMPXCHG16b, PrefetchW y LAHF/SAHF.
    • BitLocker requiere el Módulo de plataforma segura (TPM) 1.2, TPM 2.0 o una unidad flash USB 
      (solo para Windows 10 Pro y Windows 10 Enterprise).

<br>

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
 
  <br>
  
  
  
 ![PLANIFICACION](https://user-images.githubusercontent.com/89795512/132727704-9109fd09-6710-4d5e-8a66-c60d06a9e5c1.png)
 
                                              ######## 2.1 Planificación de la instalación ######## 
					      
					
		     

Antes de empezar la instalación del Sistema Operativo en el ordenador es conveniente planificar el proceso por los siguientes motivos:

    • No ejecutar acciones que conlleven la pérdida de información de los usuarios de la máquina
    • No perder tiempo durante el procedimiento debido a no haber preparado de antemano las utilidades de software y periféricos  
      hardware necesarios para llevar a cabo la instalación y proteger la información.

La primera decisión a tomar es si actualizamos el sistema operativo existente en la máquina o realizamos una nueva instalación

 <br>

<b> Instalar o actualizar </b>

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


<br>

<b> Degradación del sistema de archivos </b>

	Los sistemas operativos Windows se degradan con el uso del sistema de archivos debido a problemas como 
	la fragmentación interna y externa del sistema de archivos, las desisntalaciones de programas que no se hayan realizado limpias 
	y que ensucian el registro del sistema, o la instalación de un número muy elevado de aplicaciones.


 <br>
 <br>

<b> ** 2.2. Soporte utilizado para la instalación </b>

 • Desde una unidad DVD del propio equipo: es la forma más común de iniciar 
 la instalación y puede hacerse de dos 	maneras
 
        ◦ Iniciando el ordenador desde una unidad DVD de un ordenador limpio
        ◦ Iniciando el ordenador desde otro SO
	
• Desde un Pendrive: muchos equipos no disponen de unidades DVD por lo que es necesario instalarlo desde un pendrive. Puede hacerse de dos maneras

        ◦ Utilizar una versión portable que permite ejecutar el SO desde el mismo USB
        ◦ Preparar una unidad USB para arrancar una instalación del Sistema Operativo
	
• Desde un recurso compartido de la red. Utilizando un equipo que ya cuenta con otro sistema operativo

<br>
<br>

<b> ** 2.3. Particionamiento del disco </b>


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
    

<br>
<br>

<b> ** 2.4. Esquema de particiones Master Boot Record </b>

Es un tipo de bloque de arranque popularizado por IBM. Fue utilizado históricamente por  DOS, Microsoft Windows y Linux y otros sistemas operativos compatibles con PC. 


<b> Partición primaria </b>

Son las divisiones crudas del disco. Solo puede haber 4 en controladores IDE (15 en discos SCSI) de éstas o 3 primarias y una extendida. Depende de una tabla de particiones 

<b> Partición extendida o secundaria </b>

Actúa como una partición primaria; sirve para contener infinidad de unidades lógicas en su interior. 
Fue ideada para romper la limitación de 4 particiones primarias en un solo disco físico. Solo puede existir una partición de este tipo por disco y solo sirve para contener particiones lógicas.

<b> Partición lógica </b>
Ocupa una porción de la partición extendida o la totalidad de la misma.
Se formatea con un tipo específico de sistema de archivos (FAT32, NTFS,...) y se le asigna una unidad. 
No se puede instalar un Sistema Operativo en una partición lógica.

![Sistema Particiones](https://user-images.githubusercontent.com/89795512/132535206-31da8ad4-6ecb-460e-8540-9ddc5056b8fd.jpg)


<br>
<br>


<b> ** 2.5. Esquema de particiones de tabla de partición GUID (GPT) </b>

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


<b> ** 2.6. Preparar las particiones de los S.O. para permitir su arranque </b>

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

** <b>2.7. Administrar particiones en Windows de forma gráfica </b>

En Windows podemos configurar los discos en dos tipos:

    • Disco básico: es un disco físico que contiene particiones primarias, 
      extendidas o dispositivos lógicos (volúmenes básicos).

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

<br>

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
	

    1. Ir al Administrador de discos y seleccionar el volumen que quieras extender, pulsar el botón derecho para mostrar 
       el menú contextual y selecciona Extender volumen
    2. Pulsa siguiente y verás una pantalla en la que se ven los discos que tienen espacio sin asignar, 
       selecciona el disco o discos donde vas a extender el volumen y el tamaño que vas a utilizar en cada uno de ellos.
    3. Después pulsa siguiente y verás la pantalla de finalización del asistente con un resumen
    4. Pulsar Finalizar y se extenderá el volumen.

<b> Reducir un volumen (windows 10 y server 2012) </b>

    1. Ir al Administrador de discos y seleccionar el volumen que quieras reducir, pulsar el botón derecho para mostrar el menú contextual y selecciona reducir volumen
    2. En el apartado Tamaño del espacio que desea reducir, indicamos el tamaño que queremos disminuir del que tiene actualmente el volumen (si el volumen ocupaba más de un        	   disco, puede reducirse a menos discos).
    3. Cuando lo hayamos indicado, pulsamos reducir y se reducirá el tamaño del volumen
    
    
<b> Volúmenes distribuidos </b>

Un volumen distribuido lo forman la unión de dos o más áreas de espacio no asignado que están en dos o más discos duros. Cuando se guardan datos en un volumen distribuido, primero se ocupa el espacio libre del primer disco, cuando éste se ha llenado se pasa al segundo y así sucesivamente. Esto permite aprovechar pequeñas partes del espacio libre para formar un volumen de gran tamaño, ¡pero cuidado! si falla una parte del disco, se perderá toda la información del volumen. En cada disco se creará un volumen y cada uno tend

Para crear un volumen distribuido necesitaremos al menos dos discos duros con espacio sin asignar en cada uno de ellos.
	
    1. Ir al Administrador de discos y seleccionar el disco donde que quieras crear el volumen distribuido
    2. Mostrar el menú contextual y seleccionar Nuevo volumen distribuido
    3. Pulsar siguiente y aparecerá el asistente para volumen nuevo
    4. Seleccionar el disco o discos e indicar el tamaño del volumen distribuido
    5. Pulsar siguiente
	
<br>	
<br>

<b> ** 2.8. Administrar particiones en Windows por comandos </b>

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


							
![fat32-vs-exfat-vs-ntfs-thumbnail-1024x576](https://user-images.githubusercontent.com/89795512/132729138-ff67befd-28e7-4285-b75b-304d76742ef3.png)
					
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

<b> ** 3.3. NFTS </b>

Este formato es el sucesor de FAT32, desarrollado por Microsoft. NTFS elimina las dos limitaciones de FAT32 (los 4GB y los 8TB). Este formato de archivos también incluye una serie de novedades y mejoras necesarias para que los sistemas operativos modernos puedan funcionar sin problema y, sobre todo, en temas de seguridad, entre otras:

    • Escalabilidad: Teóricamente soporta volúmenes de hasta 16 EB
    • Journaling: Crear y guardar un diario de cambios que nos pueden ayudar a recuperarnos rápidamente de los errores 	       si el ordenador se bloquea.
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
 
<b>** 3.4. exFAT</b>

	exFAT vio la luz en 2006 y se introdujo en la mayoría de los sistemas operativos modernos, incluido Windows XP. 	Este sistema de archivos está pensado para unidades flash, siendo un sistema mucho más liviano que NTFS, sin las 	características de seguridad de este, pero también sin las limitaciones de FAT32.

	Todos los sistemas operativos de PC (Windows, Mac y Linux (aunque en este es posible que tengamos que instalar 		algunas librerías)) son compatibles de forma nativa con exFAT, al contrario que con NTFS. Este formato de 		archivos también es compatible con un gran número de dispositivos (televisiones, reproductores multimedia, 		videoconsolas, etc), aunque no llega al nivel de compatibilidad de FAT32.

	exFAT podría definirse como una actualización de FAT32 donde prima principalmente la compatibilidad y sencillez 	del formato de archivos, aunque eliminando las restricciones de los 4GB por archivo y 8 TB de tamaño máximo de 		partición.

	El uso recomendado para exFAT es para unidades externas (generalmente memorias USB o tarjetas SD) donde vayamos 	a guardar archivos de más de 4 GB y que queramos que sea compatible con el mayor número de dispositivos 		posibles. Si no vamos a guardar archivos de más de 4 GB en esas unidades, mejor optar por FAT32. 
	
	
<br>
<br>
	
	
<b>**3.5. HFS+</b>

Hierarchical File System + es el sistema de archivos desarrollado por Apple Inc. para reemplazar al HFS. 

Soporta archivos mucho más grandes, y permite nombres de fichero de hasta 255 caracteres, de longitud UTF-16. Sin embargo, estas no son sus únicas ventajas frente a HFS, ya que también utiliza una tabla de asignación de 32 bits, permitiendo el uso de más de 65.536 bloques de asignación.

El funcionamiento de HFS+ es muy parecido a su antecesor, aunque las características más llamativas han sido corregidas con el fin de hacerlo un programa más eficiente.
	
<br>
<br>

<b> **3.6. Formatear discos en Windows </b>

Podemos dar formato a un disco desde la herramienta de disco.
![FORMAT](https://user-images.githubusercontent.com/89795512/132566254-12dc9975-0f5e-4df6-bed2-bf5ceab96664.jpg)


También podemos formatear desde diskpart con la opción format.

![FORMAT2](https://user-images.githubusercontent.com/89795512/132566343-67e6af48-1cbc-48a8-8cf8-e2d9afa4882d.jpg)



<br>
<br>
<br>




					######## 4.1. Gestores de arranque ########
					
			

Un gestor de arranque es un programa que administra el arranque del sistema operativo. En el caso de tener en tu ordenador más de un sistema operativo como Windows o Linux, el gestor lo que hace es permitir al usuario elegir entre un sistema u otro.

Un ordenador actual tiene las siguientes fases de arranque:

<b> 1. Iniciador ROM: </b>
   
En esta fase se envía una señal	de RESET para cargar los valores predefinidos en todos los 				registros. Especialmente, se inicializará el contador de programa con la dirección de arranque del cargador ROM 	(almacenado en la BIOS del computador).
	
<b> 2. Cargador de SO: </b>	

En esta fase, se indica el	sector	de inicio del	disco	donde	se encuentra el sistema operativo.
Parte	residente del SO: Esta fase es la responsable de la inicialización del sistema operativo y se realizan las	siguientes tareas:
	
        a. verificación	de la consistencia del sistema de ficheros
      	b. la creación de las estructuras en memoria principal de los datos internos del sistema operativo,	
        c. la inicialización del sistema de memoria virtual,
        d. habilitación	de interrupciones,
        e. etc...
	
	
<b> 3. Fase normal de ejecución del S.O </b>

En esta fase se inicializan los servidores principales del sistema operativo y de todos los servicios
a nivel de usuario. Windows utiliza actualmente el gestor de arranque <b>Bootmgr</b>


<br>
<br>
	
	
<b> **4.2. Bootmgr </b>

La  secuencia  de  arranque  de  Windows  7 y superiores  es  distinta  de anteriores versiones de Windows. La principal diferencia estriba en que se ha cambiado el gestor de arranque, ya no se usa el ntldr sino que se usa el Windows Boot Manager (bootmgr).

El Administrador de arranque de Windows (Bootmgr) es el archivo encargado del arranque de los SO Windows actuales. Controla el proceso de arranque mostrando el menú multiarranque. Después llama al archivo WinLoad.exe en \Windows\system32 y dará paso al archivo ntoskrnl.exe que arrancará el sistema.

	
	
<b> Modificación del arranque en Windows </b>

Es posible elegir que Sistema Operativo que deseamos utilizar al arrancar si tenemos instalado más de uno, por ejemplo Windows 10 o Windows Server 16. 

Mientras  que  el  gestor  ntldr  usaba  un  fichero  de  texto  denominado  boot.ini  para  configurar sus opciones,  bootmgr  utiliza  una  base  de  datos  conocida  como  Boot  Configuration  Data (BCD)  que  no puede ser editada directamente como lo era el boot.ini ya que no es un fichero de texto.

El BCD es una base de datos con datos sobre la configuración del arranque que se suele almacenar en \Boot\Bcd.

La configuración se guarda en una serie de ficheros llamados BCD (Boot Configuration Data) que se administran mediante el comando bcdedit.exe

![boot](https://user-images.githubusercontent.com/89795512/132568212-d657a9c5-21ea-4c3f-a885-67eb29f26cbf.JPG)

<br>
<br>
	
<b> Secure Boot </b>

Secure Boot es una nueva característica de las placas base UEFI que impide la ejecución de cualquier software no firmado y certificado por el fabricante, por lo que cualquier amenaza que intentará atacar durante el inicio se vería frustrada, pues se detendría el arranque del sistema. Los fabricantes pueden decidir si permiten desactivar esta opción. 
A partir de Microsoft Windows 8, Windows exige tener esta opción en los fabricantes para obtener la certificación Windows compatible. Esta opción dio muchos problemas para instalar el Sistema Operativo GNU/Linux por lo que muchos usuarios lo desactivaron. Actualmente existen distribuciones que pueden instalar también con el sistema activado.
 Vídeo de demostración de Secure Boot:
 https://technet.microsoft.com/en-us/windows/jj737995.aspx
 
 <br>
 
<b> Trusted Boot </b>

Después de pasar Secure Boot, se activa Trusted Boot. El bootloader verifica la firma digital del kernel de Windows antes de cargarlo. El kernel de Windows, por turnos, verifica cada componente de windows en el proceso de arranque, incluyendo controladores de inicio, ficheros de arranque y ELAM. Si un fichero ha sido modificado, el bootloader detecta el problema y no cargará el componente corrupto. Muchas veces Windows puede reparar el componente corrupto automáticamente, restaurante la integridad de Windows y permitiendo arrancar el PC normalmente.

<br>

<b> Measured Boot </b>

Permite que un servidor de confianza en la red verifique la integridad del proceso de arranque en Windows. Dependiendo de la configuración permite detectar si el cliente está sano y darle acceso a toda la red o solo a una parte limitada mientras esté en cuarentena.

<br>
<br>

<b> ** 4.3. Reparación de MBR </b>

Tenemos que iniciar el sistema desde el CD original de instalación de Windows. Llegará un momento en que el propio programa de instalación nos dará la opción de realizar una reparación automática del inicio de Windows. Escogemos esta opción y comprobamos si el sistema es capaz de repararse automáticamente. 

![mbr](https://user-images.githubusercontent.com/89795512/132570640-a5ba29d3-01a1-4b82-bbed-b5a870ccbea7.JPG)

![mbr2](https://user-images.githubusercontent.com/89795512/132570692-0f0fb3c2-2d85-4e3d-b2dd-c41e012978ff.JPG)

![recu](https://user-images.githubusercontent.com/89795512/132570772-76605b32-41bc-4c56-af8b-e86cffab04b2.JPG)

Si comprobamos que dicho automatismo falla (cosa bastante probable), volvemos a iniciar el sistema desde el CD, pero esta vez desde el menú avanzado escogemos la opción de consola de recuperación o símbolo del sistema. 

![image](https://user-images.githubusercontent.com/89795512/132570813-e6f40079-5640-4292-a18d-4c9b34b3bf54.png)

Desde allí podemos ejecutar las siguientes órdenes:

1. Si el archivo bootmgr está dañado o no aparece, desde la Consola de Recuperación reconstruimos el almacén BCD con el comando:
		
		bootrec.exe  /RebuildBcd 
	
2. Este comando instala el gestor de arranque de Windows 7 en el MBR. 

		bootrec.exe /fixmbr
	
3. Este comando recupera el sector de arranque de Windows 7.

		bootrec.exe /fixboot

<br>

Si esto no funciona podremos probar a restaurar el código del sector de arranque con los siguientes comandos:

1. Averiguamos la letra de la unidad de instalación del CD/DVD o pendrive escribiendo los siguientes comandos

		diskpart
		select disk 0
		list volume

2. Buscamos la palabra  “DVD-ROM” o “extraible” en la columna “Type”. La letra está en la columna Ltr. Si la unidad fuera D:\, escribe los siguientes comandos:

		exit
		D:
		cd boot
		dir

Recuerda, si la letra de la unidad es diferente a D:\, reemplaza el segundo comando con la letra de la unidad que vieras con el comando list

3. Escribe el siguiente comando

		bootsect /nt60 SYS /mbr
	
4. Pulsa Intro
5. Quita el DVD o pendrive  
6. Escribe Exit
7. Presiona Intro para reiniciar el ordenador

<br>
<br>

<b> ** 4.4. Reparación de EFI Bootloader </b>

Si tienes un  CD/DVD/USB Windows arrancable, selecciona "Reparar el equipo"

![image](https://user-images.githubusercontent.com/89795512/132572153-b21d39d3-9df0-42a5-8b74-d5ef4a883b86.png)

Selecciona "Solucionar problemas"

![image](https://user-images.githubusercontent.com/89795512/132572309-6fa479ff-bb06-4a78-81df-1fe9306100e1.png)

Y a continuación, "Opciones avanzadas"

![image](https://user-images.githubusercontent.com/89795512/132572382-876f37fa-1427-4f31-9dde-307da45aadbd.png)

Para terminar, "Símbolo del sistema"

![image](https://user-images.githubusercontent.com/89795512/132572428-ae54f03c-dcd1-490c-8f97-058ca5f52bfe.png)


<br>

Si no tienes un CD/DVD/USB Windows

Reinicia el PC
Toca rápidamente sobre la tecla F8 una vez que el PC se ha encendido, (o en su defecto, la tecla asignada por el fabricante de tu placa base. Compruébalo por google)

Tenga en cuenta que este puede tardar varios intentos. El tiempo para esta opción se ha acortado notablemente en Windows 7.
Seleccione Reparar el equipo desde el menú que aparece.

Seleccione el símbolo de la ficha Opciones avanzadas en la solución pantalla):

<b> 1. En la ventana del símbolo del sistema: </b>
	
a. escribe y ejecuta el siguiente comando:

		Diskpart
		
b. Escribe y ejecuta el siguiente comando:

		sel disk 0
		
c. Escribe y ejecuta el siguiente comando:

		list vol

![image](https://user-images.githubusercontent.com/89795512/132573065-a3269132-3d6a-4252-9525-f371486ee9d1.png)


<b> 2. Comprueba que la partición EFI utiliza el sistema de archivos FAT32 y asigne una letra de unidad  </b>


a. Escribe y ejecuta el siguiente comando:
      
	sel vol <number of volume>
	
b. Escribe y ejecuta el siguiente comando:
	
	assign letter=<drive letter>
	
c. Escribe y ejecuta el siguiente comando:
	
	exit
			
![image](https://user-images.githubusercontent.com/89795512/132573327-b2730c05-6fbd-4a6b-9258-fa9c0fae2182.png)
		
		
3. Para reparar el registro de inicio :

a. Escribe y ejecuta el siguiente comando:
      
  	 cd /d <drive letter>:\EFI\Microsoft\Boot\
	 
b. Escriba y ejecute el siguiente comando:
      
 	bootrec /FixBoot	
	

4. Reconstruir el almacén BCD

a. En primer lugar ejecutamos el siguiente comando para hacer una copia de seguridad de la BCD vieja:

	ren BCD BCD.old 
	
b. Ahora volvemos a crearlo con este comando:
	
	bcdboot c:\Windows /l es-es /s <boot letter>: All

El parámetro /f ALL actualiza la configuración de la BIOs incluido el Firmware/NVRAM de UEFI, /l  es-es es para utilizar el locale Español de españa es/ES. 

Reinicia y cruza los dedos...

http://www.dell.com/support/Article/es/es/esbsdt1/SLN300987/ES


<br>
<br>

<b> ** 4.5. Modo seguro </b>

La forma normal de encender el sistema es simplemente pulsando el botón de encendido del equipo. Si la última vez que utilizamos el equipo lo cerramos correctamente, el equipo se volverá a encender de forma correcta.

A veces ocurre que el sistema no se cierra de forma adecuada. Las causas pueden ser: bloqueo del equipo, corte del fluido de corriente eléctrica, instalación de software no verificado, virus, etc. En este caso puede aparecernos una pantalla en modo texto con varias opciones que nos permitirá iniciar el sistema de una u otra forma, dependiendo de lo que queramos hacer.

![image](https://user-images.githubusercontent.com/89795512/132575369-b6d2977e-3bb7-44c5-8a7b-dcc69d695b30.png)


Esta forma de arrancar el equipo también es voluntaria, es decir, puede que simplemente queramos seleccionar una opción de iniciar el sistema diferente a la normal, y que no tiene por qué ser necesariamente por un problema. En este caso, cuando esté iniciándose el equipo, pulsaremos repetidamente la tecla F8 y nos aparecerán las diferentes opciones de inicio.

En general, se muestra una lista de herramientas de recuperación del sistema que se pueden utilizar para reparar problemas de inicio, e¡ecutar diagnósticos o restaurar el sistema. Esta opción solo está disponible si las herramientas están instalados en el disco duro del equipo. Si tienes un disco de instalación de Windows, las herramientas de recuperación del sistema se encuentran en el disco de instalación.

Con el lanzamiento de Windows 8, la implementación de las UEFI en la mayoría de equipos nuevos y el auge de las unidades de estado sólido para almacenamiento, las cosas han cambiado y no podemos acceder con el habitual ‘F8’ en todos los equipos. Ello no quiere decir que no podamos acceder al mismo pero de otras formas.

En Windows 8 y 10 se pulsa SHIFT+ F8, es un comando correcto y el método más rápido para arrancar en modo seguro en Windows 10 pero no funciona en la mayoría de equipos con UEFI y SSD. Microsoft explica que la rapidez de las nuevas BIOS UEFI sumadas a la de una unidad de estado sólido no dejan tiempo para interrumpir el proceso. Si has actualizado (o tienes pensado hacerlo) a Windows 10 desde Windows 7 sin implementación de UEFI, seguro que te va a funcionar.

Otra forma es mantener pulsada la tecla mayúsculas a la vez que haces clic en reinicio del sistema. Abre el menú de inicio y pulsa sobre el botón de apagado. Con la tecla mayúsculas pulsada (Shift) haz clic sobre el botón de reinicio.

![image](https://user-images.githubusercontent.com/89795512/132575577-31ef8eca-0e0a-4ed2-b8aa-1de2db239d5d.png)

Accederás a otra pantalla de configuración que te permitirá acceder al modo seguro, mediante “Solución de problemas-Opciones avanzadas-Configuración de Inicio”.

![image](https://user-images.githubusercontent.com/89795512/132576076-89c3456c-a3e1-4ab0-96dd-454cced75081.png)

Reinicia el sistema y accederás a una pantalla que te permitirá inicio en modo seguro, con funciones de red, con símbolo del sistema, etc.

![image](https://user-images.githubusercontent.com/89795512/132576171-9919f302-8fd3-42ed-9ab6-d03c4461b120.png)

<br>
<br>
<br>

					######## 5.1. Tipos de Instalaciones ########
					
					
<br>				
					
<b> ** 5.2. Manual </b>


Si utilizamos un Pendrive, utilizamos una herramienta para prepararlo de Microsoft:

Media Creation Tool para Windows 8.1 y 10:

https://www.microsoft.com/en-us/software-download/windows8
https://www.microsoft.com/es-es/software-download/windows10

Utiliza una herramienta de terceros para quemar la imagen:

Rufus: https://rufus.akeo.ie/?locale=es_ES


Metemos el CD/DVD o pinchamos el USB de instalación en dicha unidad y arrancamos el Equipo. Una vez la BIOS termine de chequear el PC, oirás el CD/DVD girar y aparecerá la siguiente pantalla:

![image](https://user-images.githubusercontent.com/89795512/132724466-335ae874-aa35-4a69-8cb8-128391e2e686.png)

Si no apareciera, es que no está activado o disponible el arranque del ordenador a través de CD/DVD o USB en la BIOS. Para activarlo, debes estar atento al momento en que arranca, cuando se muestra el chequeo de la memoria RAM y demás:

![image](https://user-images.githubusercontent.com/89795512/132724582-907572ee-9392-4bdb-85d8-b5524c7184b8.png)

En este momento debes pulsar la tecla "Supr" (fijate que dice "Press DEL to run Setup") para entrar en el menú de la BIOS y activarlo. En otras BIOS / BIOS UEFI son comunes las combinaciones F1, F2, F10, DEL, ESC, y también combinaciones como  CTRL + ALT + ESC o CTRL + ALT + DEL en máquinas antiguas.

Utiliza los cursores para desplazarte hasta el apartado "Boot" (arranque):

![image](https://user-images.githubusercontent.com/89795512/132724624-5a39caff-9c1f-4721-8225-fbd59d5fd21e.png)

Después pulsa "Enter" para ir al sub-menú:

![image](https://user-images.githubusercontent.com/89795512/132724653-87a72f0a-4242-4093-89d6-3aa2d73a92bb.png)


Debería estar configurado como opción de arranque el lector de CD/DVD o Removable Device antes del disco duro (Hard drive). Si no estuviera asi, utiliza los cursores para seleccionar el primer, segundo o tercer puesto y la  flecha a izquierdas, para cambiarlo. Al terminar, pulsa F10 para guardar cambios y salir:

![image](https://user-images.githubusercontent.com/89795512/132724703-5e85da87-afb6-481b-900e-83ba99f30fed.png)


Selecciona "[OK]" y pulsa "Enter" para guardar y salir. Si todo ha ido bien, debería aparecer el mensaje que ves al principio de esta opción. En el momento en que lo veas, pulsa cualquier tecla y se iniciará el proceso de instalación.

En equipos nuevos, está configurado por defecto Secure Boot, si tienes problemas para arrancar desde el CD/DVD o el USB de por ejemplo un Windows 7 puedes desactivar esta opción en la BIOS UEFI utilizando el modo Legacy, en cada fabricante es diferente.


![image](https://user-images.githubusercontent.com/89795512/132724747-7964e815-a80a-4fb7-998b-4dc2d36a8933.png)

<br>
<br>

<b> Acceder a UEFI desde la configuración de Windows 10 </b>

Si tienes Windows 10 instalado, puedes entrar en la configuración de UEFI desde Windows.

Si tener ningún programa en ejecución, vamos a la Configuración del sistema desde el menú inicio y a continuación elegimos la opción Actualización y seguridad para posteriormente elegir la opción Recuperación del menú del lateral izquierdo. Esto nos mostrará en el panel de la derecha la opción de Inicio avanzado junto con un botón de Reiniciar ahora.

![image](https://user-images.githubusercontent.com/89795512/132724925-033eaf02-69ad-452d-bcaa-bbf046f493db.png)

Al pulsar sobre él, el sistema nos mostrará una pantalla donde podremos elegir la forma en la que queremos realizar el reinicio. En esta ocasión elegiremos Solucionar problemas, a continuación indicaremos que queremos entrar en las Opciones Avanzadas y posteriormente en los ajustes de UEFI. Una vez ahí, sólo queda pulsar sobre el botón de reinicio para entrar en la configuración de firmware UEFI.

![image](https://user-images.githubusercontent.com/89795512/132724950-d1a493d7-fd99-4a98-a7e5-d1834874bf7e.png)


Acceder desde el símbolo del sistema a UEFI en Windows 10

En esta ocasión, lo primero que hacemos es abrir una ventana de símbolo de sistema con permisos de administrador haciendo clic con el botón derecho del ratón sobre el menú inicio y seleccionando la opción Símbolo del sistema (administrador).

A continuación, escribimos el comando shutdown.exe /r /o y pulsamos Enter. Esto nos mostrará un mensaje en el que se nos dice que nuestro ordenador se va a reiniciar en menos de un minuto. Una vez que se reinicie, tendremos que seguir los pasos realizados en el anterior punto desde que elegimos la opción de Solucionar problemas.

![image](https://user-images.githubusercontent.com/89795512/132724991-b7992700-3359-42e8-81b9-5810f6e5066b.png)


Hasta este punto también podemos llegar pulsando sobre la opción Apagar del menú inicio y manteniendo la tecla Shift pulsada, elegir la opción de reiniciar el equipo.

<br>
<br>


<b> ** 5.3. Desatendida </b>

La instalación desatendida en Windows 8 y posteriores se realiza a través de la herramienta ADK ( Assessment and Deployment Kit), descargable también desde la web de Microsoft.También nos permite generar un fichero .iso, que se puede grabar para generar un DVD de instalación desatendida.

![image](https://user-images.githubusercontent.com/89795512/132725175-10f41d85-c655-4552-8537-4d3696b9dcb8.png)

Descarga de Windows 10 ADK https://developer.microsoft.com/en-us/windows/hardware/windows-assessment-deployment-kit

Existen herramientas de tercero que permiten realizarlo, como Windows Answer File Generator:
![image](https://user-images.githubusercontent.com/89795512/132725232-a0fc601c-b4ac-4943-9853-d54419ee56c9.png)

<b> ** 5.4. En red por imágenes </b>

Consiste en la utilización de un software especial, que permite clonar desde particiones, a discos duros enteros.  Los programas más utilizados son Norton Ghost y Clonezilla.

![image](https://user-images.githubusercontent.com/89795512/132725393-567d7c39-c36e-45c4-90ce-9d667c899bc5.png)


l problema con Windows, es que el proceso de instalación del Sistema operativo incluye tanto un número de licencia como un identificador para el equipo, que se genera con datos proporcionados por la BIOS, que debería ser único para cada ordenador. El problema se plantea en el caso de la clonación, que duplica dicho identificador. Esto provoca fallos inesperados en los sistemas clonados, por lo que los programas de clonación deberían incluir una herramienta que permita cambiar dicho identificador, y también el número de licencia.

	Cosas que hay que hacer después de clonar: 

    • Cambiar la dirección IP del Equipo: En ninguna red puede haber dos ordenadores con la misma IP.
    • Cambiar el nombre del equipo: En ninguna red puede haber dos ordenadores con el mismo nombre. (Si el equipo forma       parte de un dominio, para hacer el cambio, debo pasarlo a un grupo de trabajo, cambiar el nombre, y luego               volver a introducirlo en el dominio).
    • Cambiar el identificador, o el número de licencia. Esto es opcional, en el caso de sistemas operativos clientes 	    de red, e imperativo en el caso de los servidores.

<br>
<br>

<b> ** 6.4. En red por servidores </b>

Esta opción está desarrollada para el despliegue de sistemas Windows. Se realiza la instalación desde un servidor a ordenadores clientes dentro de la red de área local. Para poder instalar el sistema operativo, necesitamos una serie de requisitos:

1.- El/Los ordenadores cliente deberán contar con una tarjeta de red que admita PXE. Esta tarjeta intentará obtener una dirección IP válida, a través de un servidor DHCP. 

2.- El ordenador Servidor: Que tenga activado el servicio DHCP, y el de instalación remota: Servicio WDS en el caso de servidores Windows Server 2008/2012.

![image](https://user-images.githubusercontent.com/89795512/132725599-24a7d51e-8b56-4153-9c8d-70b2eefbc1a3.png)

    
