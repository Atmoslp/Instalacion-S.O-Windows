# Instalación-Sistemas-Operativos


<h2>#ÍNDICE</h2>
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
 
 
                                            ######## 1.1 Instalar un Sistema Operativo ######## 
					    ----------------------------------------------------
  
Después de conocer las técnicas básicas que utilizan los SSOO para gestionar los recursos de hardware, es hora de aprender a instalar un sistema operativo.
En esta unidad voy explicar los pasos necesarios para la instalación de los sistemas operativos monousuarios propietarios más extendidos hoy en día, los de Microsoft Windows.

Una familia de SSOO está formada por versiones antiguas del sistema que han dejado de recibir soporte técnico por parte de la propietaria del producto; solamente la versión más reciente incorpora todas las mejoras técnicas que se han implementado por avances del hardware o mejoras de los desarrolladores del software. Por esta razón, aunque parece que existen muchísimos SSOO en el mercado, solo están disponibles las versiones más recientes. 

Por ejemplo, en el caso de Apple tenemos el macOS Big Sur como versión más reciente para ordenadores y iOS 14 para móviles y tabletas.
Microsoft actualmente tiene como versión más reciente Windows 10 tanto para ordenadores como dispositivos móviles.


**   <b>  1.2. Requisitos mínimos </b>

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


 
 **   <b> 1.3. Selección del Sistema Operativo Windows </b>

En la página oficial del Sistema Operativo Windows de Microsoft tenemos información oficial del producto: https://www.microsoft.com/es-es/windows

En esta página podemos consultar una tabla comparativa de sus diversas versiones y ediciones para poder evaluar cuál resulta más adecuado para instalar o actualizar en nuestro sistema informático.

En la siguiente tabla mostramos las diferencias más importantes entre las distintas versiones de Windows 7, 8.1 y 10, que hemos obtenido de https://www.microsoft.com/es-es/windows/compare



**   <b> 1.4. Ediciones de Windows 10 </b>



      • Home: Para configurar un pc doméstico que será administrado por un usuario 
        sin conocimientos avanzados de informática.
        
      • Pro o Enterprise: Para configurar un PC de una red de ordenadores que se necesita 
        ser administrada de manera centralizada (Unión a Dominio y escritorio remoto)
        
     • Education: Para alumnos que esté estudiando por un tiempo determinado y quieran 
       aprender a configurar equipos a nivel avanzado.
    


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
 
 
 
 
 
 
 
 
 
 
 
                                                  2.1 Planificación de la instalación

Antes de empezar la instalación del Sistema Operativo en el ordenador es conveniente planificar el proceso por los siguientes motivos:

    • No ejecutar acciones que conlleven la pérdida de información de los usuarios de la máquina
    • No perder tiempo durante el procedimiento debido a no haber preparado de antemano las utilidades de software y periféricos  
      hardware necesarios para llevar a cabo la instalación y proteger la información.

La primera decisión a tomar es si actualizamos el sistema operativo existente en la máquina o realizamos una nueva instalación


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




** <b> 2.2. Soporte utilizado para la instalación</b>

 • Desde una unidad DVD del propio equipo: es la forma más común de iniciar 
 la instalación y puede hacerse de dos 	maneras
 
        ◦ Iniciando el ordenador desde una unidad DVD de un ordenador limpio
        ◦ Iniciando el ordenador desde otro SO
	
• Desde un Pendrive: muchos equipos no disponen de unidades DVD por lo que es necesario instalarlo desde un pendrive. Puede hacerse de dos maneras

        ◦ Utilizar una versión portable que permite ejecutar el SO desde el mismo USB
        ◦ Preparar una unidad USB para arrancar una instalación del Sistema Operativo
	
• Desde un recurso compartido de la red. Utilizando un equipo que ya cuenta con otro sistema operativo



** <b> 2.3. Particionamiento del disco </b>


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


** <b> 2.4. Esquema de particiones Master Boot Record </b>

Es un tipo de bloque de arranque popularizado por IBM. Fue utilizado históricamente por  DOS, Microsoft Windows y Linux y otros sistemas operativos compatibles con PC. 


<h3>Partición primaria</h3>

Son las divisiones crudas del disco. Solo puede haber 4 en controladores IDE (15 en discos SCSI) de éstas o 3 primarias y una extendida. Depende de una tabla de particiones 

<h3>Partición extendida o secundaria</h3>

Actúa como una partición primaria; sirve para contener infinidad de unidades lógicas en su interior. 
Fue ideada para romper la limitación de 4 particiones primarias en un solo disco físico. Solo puede existir una partición de este tipo por disco y solo sirve para contener particiones lógicas.

<h3>Partición lógica</h3>
Ocupa una porción de la partición extendida o la totalidad de la misma.
Se formatea con un tipo específico de sistema de archivos (FAT32, NTFS,...) y se le asigna una unidad. 
No se puede instalar un Sistema Operativo en una partición lógica.

![Sistema Particiones](https://user-images.githubusercontent.com/89795512/132535206-31da8ad4-6ecb-460e-8540-9ddc5056b8fd.jpg)





** <b>2.5. Esquema de particiones de tabla de partición GUID (GPT)</b>

Hoy en día todos los Sistemas Operativos soportan. Es parte del estándar  Unified Extensible Firmware Interface (EFI) propuesto por Intel para reemplazar la vieja BIOS del PC.

La GPT sustituye al Master Boot Record (MBR) usado con la BIOS. Se basa en las capacidades extendidas del EFI para estos procesos. 

Las principales ventajas de GPT frente a MBR son:

    • Admite discos de más de 2 TB hasta teóricamente 2 ZB ( 2*109 TB).
    • No es necesario crear particiones extendidas ni lógicas, por defecto admite hasta 128 particiones.
    • Almacena una copia de seguridad del encabezado y de la tabla de particiones al final del disco que ayuda en la recuperación 
      en el caso de que los primeros están dañados.
    • Checksum CRC32 para detectar errores y daños de la cabecera y en la tabla de particiones al proporcionar redundancia.
   
![GPT](https://user-images.githubusercontent.com/89795512/132539970-90e9c8ac-5fbf-4f07-8bc2-b28ed0134e24.jpg)




** <b>2.6. Preparar las particiones de los S.O. para permitir su arranque.</b>

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


<b>Extender un volumen de forma gráfica
	

    1. Ir al Administrador de discos y seleccionar el volumen que quieras extender, pulsar el botón derecho para mostrar el menú contextual y selecciona Extender volumen
    2. Pulsa siguiente y verás una pantalla en la que se ven los discos que tienen espacio sin asignar, selecciona el disco o discos donde vas a extender el volumen y el tamaño          que vas a utilizar en cada uno de ellos.
    3. Después pulsa siguiente y verás la pantalla de finalización del asistente con un resumen
    4. Pulsar Finalizar y se extenderá el volumen.

<b>Reducir un volumen (windows 10 y server 2012)

    1. Ir al Administrador de discos y seleccionar el volumen que quieras reducir, pulsar el botón derecho para mostrar el menú contextual y selecciona reducir volumen
    2. En el apartado Tamaño del espacio que desea reducir, indicamos el tamaño que queremos disminuir del que tiene actualmente el volumen (si el volumen ocupaba más de un disco, 	   puede reducirse a menos discos).
    3. Cuando lo hayamos indicado, pulsamos reducir y se reducirá el tamaño del volumen
    
    
Volúmenes distribuidos

Un volumen distribuido lo forman la unión de dos o más áreas de espacio no asignado que están en dos o más discos duros. Cuando se guardan datos en un volumen distribuido, primero se ocupa el espacio libre del primer disco, cuando éste se ha llenado se pasa al segundo y así sucesivamente. Esto permite aprovechar pequeñas partes del espacio libre para formar un volumen de gran tamaño, ¡pero cuidado! si falla una parte del disco, se perderá toda la información del volumen. En cada disco se creará un volumen y cada uno tend

Para crear un volumen distribuido necesitaremos al menos dos discos duros con espacio sin asignar en cada uno de ellos.
	
    1. Ir al Administrador de discos y seleccionar el disco donde que quieras crear el volumen distribuido
    2. Mostrar el menú contextual y seleccionar Nuevo volumen distribuido
    3. Pulsar siguiente y aparecerá el asistente para volumen nuevo
    4. Seleccionar el disco o discos e indicar el tamaño del volumen distribuido
    5. Pulsar siguiente
	
	

