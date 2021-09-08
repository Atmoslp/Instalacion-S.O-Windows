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
 
 
                                                 1.1 Instalar un Sistema Operativo
  
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
    
    ![GPT](https://user-images.githubusercontent.com/89795512/132539267-7cfbb81f-7d7f-444d-a2c3-b5e919018af4.jpg)

    
   
    
    

