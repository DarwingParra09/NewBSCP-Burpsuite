# Vulnerabilidad de inyección SQL en la cláusula WHERE que permite la recuperación de datos ocultos

![[01.SQLClausulaWhere.png]]
![[02.SQLClausulaWhere.png]]

# Vulnerabilidad de inyección SQL que permite omitir el inicio de sesión

![[01.SQL_OmitirInicioSesion.png]]
![[02.SQL_OmitirInicioSesion.png]]
![[03.SQL_OmitirInicioSesion.png]]

# Ataque de inyección SQL, consultando el tipo y la versión de la base de datos en Oracle

Falta

# Ataque de inyección SQL, consultando el tipo y la versión de la base de datos en MySQL y Microsoft

Falta

# Ataque de inyección SQL, enumerando el contenido de la base de datos en bases de datos que no son Oracle

![[01.BasicosOracle.png]]
![[02.BasicosOracle.png]]
![[03.BasicosOracle.png]]
![[04.BasicosOracle.png]]
![[05.BasicosOracle.png]]
![[06.BasicosOracle.png]]
![[07.BasicosOracle.png]]
![[08.BasicosOracle.png]]

# Ataque de inyección SQL, que enumera el contenido de la base de datos de Oracle

Falta

# Ataque UNION de inyección SQL, determinando el número de columnas devueltas por la consulta

![[Pasted image 20240816012757.png]]
![[Pasted image 20240816013126.png]]
![[Pasted image 20240816013146.png]]
![[Pasted image 20240816013207.png]]

# Ataque UNION de inyección SQL, búsqueda de una columna que contiene texto

![[01.AtaqueUNION_SQL.png]]
![[02.AtaqueUNION_SQL.png]]
![[03.AtaqueUNION_SQL.png]]
![[04.AtaqueUNION_SQL.png]]
![[05.AtaqueUNION_SQL.png]]
![[06.AtaqueUNION_SQL.png]]

# Ataque UNION de inyección SQL, recuperando datos de otras tablas

![[01.RecuperarDatosConTablas.png]]
![[02.RecuperarDatosConTablas.png]]
![[03.RecuperarDatosConTablas.png]]
![[04.RecuperarDatosConTablas.png]]
![[05.RecuperarDatosConTablas.png]]

# Ataque UNION de inyección SQL, recuperando múltiples valores en una sola columna

![[Pasted image 20240816020113.png]]
![[Pasted image 20240816020238.png]]
![[Pasted image 20240816020334.png]]
![[Pasted image 20240816020426.png]]

# Ataque UNION de inyección SQL, búsqueda de una columna que contiene texto

![[Pasted image 20240820214407.png]]
![[Pasted image 20240820214622.png]]
![[Pasted image 20240820214642.png]]
![[Pasted image 20240820214701.png]]
![[Pasted image 20240820214814.png]]
![[Pasted image 20240820214837.png]]

# Ataque UNION de inyección SQL, recuperando datos de otras tablas 

![[Pasted image 20240820221843.png]]
![[Pasted image 20240820221906.png]]
![[Pasted image 20240820223005.png]]
![[Pasted image 20240820223023.png]]
![[Pasted image 20240820223041.png]]

# Ataque UNION de inyección SQL, recuperando múltiples valores en una sola columna

![[Pasted image 20240820223151.png]]
![[Pasted image 20240820223215.png]]
![[Pasted image 20240820223238.png]]
![[Pasted image 20240820223257.png]]

# Inyección SQL ciega con respuestas condicionales

![[Pasted image 20240820223510.png]]
![[Pasted image 20240820223531.png]]
![[Pasted image 20240820223620.png]]
![[Pasted image 20240820223641.png]]
![[Pasted image 20240820223802.png]]

# Inyección SQL ciega con errores condicionales

![[Pasted image 20240820231016.png]]
![[Pasted image 20240820231130.png]]
![[Pasted image 20240820231504.png]]
![[Pasted image 20240820231526.png]]
![[Pasted image 20240820231553.png]]
![[Pasted image 20240820231628.png]]
![[Pasted image 20240820231652.png]]

# Inyección SQL visible basada en errores

![[Pasted image 20240820233242.png]]
![[Pasted image 20240820233330.png]]

# Inyección SQL ciega con retrasos de tiempo

Falta

# Inyección SQL ciega con retrasos temporales y recuperación de información

![[Pasted image 20240823011419.png]]
![[Pasted image 20240823011432.png]]
![[Pasted image 20240823011524.png]]
![[Pasted image 20240823011540.png]]
![[Pasted image 20240823011953.png]]
![[Pasted image 20240823012004.png]]
![[Pasted image 20240823012142.png]]
![[Pasted image 20240823012206.png]]
![[Pasted image 20240823012439.png]]
```
%3BSELECT+CASE+WHEN+(username='administrator'+AND+SUBSTRING(password,1,1)='§a§')+THEN+pg_sleep(5)+ELSE+pg_sleep(0)+END+FROM+users--
```
![[Pasted image 20240823012834.png]]
![[Pasted image 20240823013339.png]]
![[Pasted image 20240823013508.png]]
![[Pasted image 20240823014637.png]]
![[Pasted image 20240823014651.png]]

# Inyección SQL ciega con exfiltración de datos fuera de banda

Falta

# Inyección SQL con omisión de filtros mediante codificación XML

Falta

