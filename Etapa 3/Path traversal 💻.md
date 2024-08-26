También conocido como "directory traversal" o "arbitrary file access," es un tipo de vulnerabilidad de seguridad web que permite a un atacante acceder a archivos y directorios fuera del directorio raíz del servidor web. Esto puede llevar a la exposición de información sensible, como archivos de configuración, contraseñas, y otros datos críticos que no deberían ser accesibles públicamente

# Simple Path Traversal

![[01.PathTraversalSimple.png]]
![[02.PathTraversalSimple.png]]

# Recorrido de rutas de archivos, secuencias de recorrido bloqueadas con omisión de ruta absoluta

![[01.RecorridoBloqueado.png]]
![[02.RecorridoBloqueado.png]]
![[03.RecorridoBloqueado.png]]

# Recorrido de rutas de archivos , secuencias de recorrido eliminadas de forma no recursiva

![[01.FLP_SecuenciaNoRecursiva.png]]
![[02.FLP_SecuenciaNoRecursiva.png]]
![[03.FLP_SecuenciaNoRecursiva.png]]

# Recorrido de rutas de archivos, secuencias de recorrido eliminadas con decodificación de URL superflua

![[01.DobleDecodificacion.png]]
![[02.DobleDecodificacion.png]]
![[03.DobleDecodificacion.png]]
![[04.DobleDecodificacion.png]]
![[05.DobleDecodificacion.png]]
![[06.DobleDecodificacion.png]]

# Recorrido de rutas de archivos, validación del inicio de la ruta

![[01.ValidacionDeInicioRuta.png]]
![[02.ValidacionDeInicioRuta.png]]
![[03.ValidacionDeInicioRuta.png]]

# Recorrido de rutas de archivos, validación de extensiones de archivos con omisión de bytes nulos

![[01.OmisionDeBytes.png]]
![[02.OmisionDeBytes.png]]
![[03.OmisionDeBytes.png]]

