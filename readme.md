# 1. Nombre del webservice
## El nombre del webservice es Send Api Mail.
# 2. Descripción 
## Este webservice consiste en que mediante el plugin de rest Client, consigas enviarte un email del cualquier usuario que registres en este Send Api Mail.
# 3. Instalación 
## Para alcanzar este objetivo descrito en el apartado anterior, tienes que tener instalado el plugin de rest Client en tu Visual Studio Code. Para instalarlo, tienes que buscar en el icono de extensiones del menú lateral de tu visual: REST Client. El autor de este plugin es Huachao Mao.

# 4. Uso (endpoint, parámetros)
## Una vez instalado el plugin del aparta anterior, la forma de usarlo es creando una carpeta llamada v1 en la raiz del directorio que has tenido que abrir con el visual. En esa carpeta tienes que definir los parámetros para poder hacer solicitudes http.

## Y una vez definidos esos parámetros necesarios, tienes que ir a crear un archivo http en la raiz de este directorio que hayas creado al principio de todo para abrir este visual. Y en ese archivo probarias la solicitud con el metodo POST de esos parámetros definidos. Y para que te salga todo correcto y el email aparezca enviado a tu correo en papercut; antes de darle a send request; asegurate que el el sql y el apache en xamp lo tengas encendido.
# 5. Ejemplo de solicitud (cliente http, formulario o react)

## Tendrias que acabar el proceso de uso del apartado anterior , más o menos como en el ejemplo: 

--- 

### Prueba de correo exitoso
POST http://localhost/api/v1/endpoint-webservices/
Content-Type: application/json

{
    "name": "John Doe",
    "email": "john@example.com",
    "message": "Hello, this is my personal adress"
}


Y el  resultado esperado que te tiene que quedar al dar al send request, tiene que quedarte más o menos así:

---


{
  "status": "success",
  "message": "Correo enviado correctamente."
}

---
---