# qrcode-website
Imprimir código QR en sitio Web

Ejemplo simple de como generar un código QR en nuestro sitio web.

Para poder implementarlo es necesario lo siguiente:
Jquery la versión que gusten.
Librería jquery.qrcode.js
Con su complemento qrcode.js

        <script src="jquery-1.11.3.min%20.js"></script>
        <script src="jquery.qrcode.js"></script>
        <script src="qrcode.js"></script>

Luego hacemos la petición con 

    	                    
    	                    $(document).ready(function () {
    	                        ('#qrcodeCanvas').qrcode({
    	                            text: "Valor del Código QR",//valor que se renderizará a QR
    	                            width: 75,//tamaño de largo
    	                            height: 75//tamaño de alto
    	                        });
    	                    });
    	                    
Para ello es necesario tener en nuestro html un div con identificador "qrcodeCanvas" para poder ejecutarlo

    <div style="width:50px;text-align:center;margin:0 auto;" id="qrcodeCanvas"></div>

Y es lo único que hay que realizar y ya tenemos la impresión de un código QR en una página html (php, aspx, en lo que decidas hacerlo)
