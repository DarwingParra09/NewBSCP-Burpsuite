**Server-Side Request Forgery (SSRF)** es un tipo de vulnerabilidad en la que un atacante puede hacer que un servidor realice solicitudes HTTP a dominios o direcciones IP arbitrarias, incluidas las internas, que normalmente no estarían accesibles para el atacante. Esta vulnerabilidad surge cuando una aplicación web acepta entradas de usuario para formar o redirigir una solicitud desde el servidor, y no valida o restringe adecuadamente esa entrada.
# SSRF básico contra el servidor local 

![[01.SSRF_Basico.png]]
![[02.SSRF_Basico.png]]
![[03.SSRF_Basico.png]]
![[04.SSRF_Basico.png]]
![[05.SSRF_Basico.png]]
![[06.SSRF_Basico.png]]
![[07.SSRF_Basico.png]]

# SSRF básico frente a otro sistema back-end

![[01.SSRF_Back-End.png]]
![[02.SSRF_Back-End.png]]
![[03.SSRF_Back-End.png]]
![[04.SSRF_Back-End.png]]
![[05.SSRF_Back-End.png]]
![[06.SSRF_Back-End.png]]


# SSRF con omisión de filtro a través de una vulnerabilidad de redirección abierta

![[01.SSRF_OmisionDeFiltro.png]]
![[02.SSRF_OmisionDeFiltro.png]]
![[03.SSRF_OmisionDeFiltro.png]]
![[04.SSRF_OmisionDeFiltro.png]]

# # SSRF ciego con detección fuera de banda

![[01.SSRF_Ciego_FueradeBanda.png]]
![[02.SSRF_Ciego_FueradeBanda.png]]

# SSRF con filtro de entrada basado en lista negra

![[01.SSRF_BasadoListaNegra.png]]
![[02.SSRF_BasadoListaNegra.png]]
![[03.SSRF_BasadoListaNegra.png]]
![[04.SSRF_BasadoListaNegra.png]]
![[05.SSRF_BasadoListaNegra.png]]
![[06.SSRF_BasadoListaNegra.png]]
![[07.SSRF_BasadoListaNegra.png]]
![[08.SSRF_BasadoListaNegra.png]]
![[09.SSRF_BasadoListaNegra.png]]
![[10.SSRF_BasadoListaNegra.png]]

