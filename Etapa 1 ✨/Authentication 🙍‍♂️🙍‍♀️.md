Las vulnerabilidades de autenticación son fallas en los mecanismos de autenticación de una aplicación o sistema que pueden ser explotadas por atacantes para obtener acceso no autorizado a recursos restringidos. Estas vulnerabilidades pueden comprometer la seguridad de la aplicación, permitiendo a los atacantes realizar acciones como suplantación de identidad, acceso a datos sensibles o incluso tomar el control total del sistema.

- [[Usernames.txt]]
- [[Passwords.txt]]

# Enumeración de nombres de usuario mediante diferentes respuestas

![[01.AutenticacionBasico.png]]
![[02.AutenticacionBasica.png]]
![[03.AutenticacionBasica.png]]
![[04.AutenticacionBasica.png]]
![[05.AutenticacionBasica.png]]
![[06.AtenticacionBasica.png]]

# Bypass simple de 2FA

![[01.BypassSimple.png]]
![[02.BypassSimple.png]]
![[03.BypassSimple.png]]
![[04.BypassSimple.png]]
![[05.BypassSimple.png]]

# Lógica rota en el restablecimiento de contraseña

![[01.RestablecerContraseña.png]]
![[02.RestablecerContraseña.png]]
![[03.RestablecerContraseña.png]]
![[04.RestablecerContraseña.png]]
![[05.RestablecerContraseña.png]]
![[06.RestablecerContraseña.png]]
![[07.RestablecerContraseña.png]]
![[08.RestablecerContraseña.png]]
![[09.RestablecerContraseña.png]]
![[10.RestablecerContraseña.png]]
![[11.RestablecerContraseña.png]]

# Enumeración de nombres de usuario mediante respuestas sutilmente diferentes

![[01.EnumeracionSutil.png]]
![[02.EnumeracionSutil.png]]
![[03.EnumeracionSutil.png]]
![[04.EnumeracionSutil.png]]
![[05.EnumeracionSutil.png]]
![[06.EnumeracionSutil.png]]
![[07.EnumeracionSutil.png]]

# Enumeración de nombres de usuario mediante tiempos de respuesta

![[01.Enumeracion_TiempoRespuesta.png]]
Al estar un usuario verificado se toma un tiempo un poco más largo para verificar la contraseña, en este caso vemos que demora 1 segundo
![[02.Enumeracion_TiempoRespuesta.png]]
![[03.Enumeracion_TiempoRespuesta.png]]
En esta es  instantáneo, pero dentro de otras posibles contraseñas al no ser la verificada como su credencial duraría menos su tiempo respuesta
![[04.Enumeracion_TiempoRespuesta.png]]
![[05.Enumeracion_TiempoRespuesta.png]]
![[06.Enumeracion_TiempoRespuesta.png]]
![[07.Enumeracion_TiempoRespuesta.png]]
![[08.Enumeracion_TiempoRespuesta.png]]
![[09.Enumeracion_TiempoRespuesta.png]]
![[10.Enumeracion_TiempoRespuesta.png]]
![[11.Enumeracion_TiempoRespuesta.png]]

# Protección de fuerza bruta rota, bloqueo de IP

Después de varios intentos erróneos se bloquea por un minuto, cada 3 intentos se bloquea
![[01.FuerzaBruta,BloqueoIP.png]]
![[02.FuerzaBruta,BloqueoIP.png]]
Se observa que al validar las credenciales nos envia una redireccion de la peticion avisando que las credenciales fueron encontradas
![[03.FuerzaBruta,BloqueoIP.png]]
Para no pasar por el tiempo de bloqueo, hacemos nuestros propio username.txt, con el nombre del usuario al cual sabemos la credencial y el otro del cual no sabemos, podemos fallar dos veces escribiendo la contraseña de carlos, pero a la hora de ingresar con wiener el contador de fallos se restablece 
![[04.FuerzaBruta,BloqueoIP.png]]
![[05.FuerzaBruta,BloqueoIP.png]]
Encontramos la contraseña del usuario carlos gracias a que nos lanza un codigo de estado 302, asi como en el ingreso del usuario wiener
![[06.FuerzaBruta,BloqueoIP.png]]
![[07.FuerzaBruta,BloqueoIP.png]]

# Enumeración de nombres de usuario mediante bloqueo de cuenta

![[01.NombresUsuarioBloqueoDeCuenta.png]]
![[02.NombresUsuarioBloqueoDeCuenta.png]]
![[03.NombresUsuarioBloqueoDeCuenta.png]]
![[04.NombresUsuarioBloqueoDeCuenta.png]]
![[05.NombresUsuarioBloqueoDeCuenta.png]]
![[06.NombresUsuarioBloqueoDeCuenta.png]]
![[07.NombresUsuarioBloqueoDeCuenta.png]]
![[08.NombresUsuarioBloqueoDeCuenta.png]]
![[09.NombresUsuarioBloqueoDeCuenta.png]]
![[10.NombresUsuarioBloqueoDeCuenta.png]]

# Lógica rota de 2FA

![[01.LogicaRota2FA.png]]
![[02.LogicaRota2FA.png]]
![[03.LogicaRota2FA.png]]
![[04.LogicaRota2FA.png]]
![[05.LogicaRota2FA.png]]
![[06.LogicaRota2FA.png]]
![[07.LogicaRota2FA.png]]
![[08.LogicaRota2FA.png]]
![[09.LogicaRota2FA.png]]
![[10.LogicaRota2FA.png]]
![[11.LogicaRota2FA.png]]
![[12.LogicaRota2FA.png]]
![[13.LogicaRota2FA.png]]

# Forzar bruscamente una cookie que impide permanecer conectado

![[01.AutenticacionCookieForzada.png]]
![[02.AutenticacionCookieForzada.png]]
![[03.AutenticacionCookieForzada.png]]
![[04.AutenticacionCookieForzada.png]]
![[05.AutenticacionCookieForzada.png]]
![[06.AutenticacionCookieForzada.png]]
![[07.AutenticacionCookieForzada.png]]
![[08.AutenticacionCookieForzada.png]]

# Descifrado de contraseñas sin conexión

![[01.DescifradoSinConexion.png]]
![[02.DescifradoSinConexion.png]]
![[03.DescifradoSinConexion.png]]
![[04.DescifradoSinConexion.png]]
![[05.DescifradoSinConexion.png]]
![[06.DescifradoSinConexion.png]]
![[07.DescifradoSinConexion.png]]
![[08.DescifradoSinConexion.png]]
![[09.DescifradoSinConexion.png]]

# Envenenamiento por restablecimiento de contraseñas mediante middleware

![[01.EnvenamientoContraseñasMiddleware.png]]
![[02.EnvenamientoContraseñasMiddleware.png]]
![[03.EnvenamientoContraseñasMiddleware.png]]
![[04.EnvenamientoContraseñasMiddleware.png]]
![[05.EnvenamientoContraseñasMiddleware.png]]
![[06.EnvenamientoContraseñasMiddleware.png]]
![[07.EnvenamientoContraseñasMiddleware.png]]
![[08.EnvenamientoContraseñasMiddleware.png]]
![[09.EnvenamientoContraseñasMiddleware.png]]
![[10.EnvenamientoContraseñasMiddleware.png]]

# Fuerza bruta de contraseñas mediante cambio de contraseña

![[01.FuerzaBrutaCambiodeContraseña.png]]
![[02.FuerzaBrutaCambiodeContraseña.png]]

Contraseña correcta pero la nueva contraseña no coincide

![[03.FuerzaBrutaCambiodeContraseña.png]]
![[04.FuerzaBrutaCambiodeContraseña.png]]

![[05.FuerzaBrutaCambiodeContraseña.png]]
![[06.FuerzaBrutaCambiodeContraseña.png]]
![[07.FuerzaBrutaCambiodeContraseña.png]]
![[08.FuerzaBrutaCambiodeContraseña.png]]
![[09.FuerzaBrutaCambiodeContraseña.png]]
