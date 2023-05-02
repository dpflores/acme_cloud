# CLOUD ACME

En este repositorio están algunos aspectos útiles para el manejo de servidor en la nube y aplicaciones en contenedores que se podrían utilizar


# Acceso SSH 

Para acceder al servidor en la nube utilizando ssh, se tiene que tener la `hostname` o `ip`, el `usuario` y `contraseña`.

Entonces, ejecutamos en la terminal

```
ssh usuario@hostname
```

Luego solicitará la contraseña, una vez ingresado ahora nos ubicamos en la terminal del servidor en la nube.

Otra forma de agilizar el ingreso por ssh sin tener que ingresar la contraseña es que en nuestra computadora personal ejecutemos

```
ssh-keygen
```
Seleccionamos todo por default, y luego visualizamos el archivo creado con cualquier visualizador que tengamos con el comando

```
cat ~/.ssh/id_rsa.pub
```

Esto se puede copiar y guardar para luego pegarlo en el archivo de configuración de la nube o otra forma más fácil de enviar esto a nuestro servidor de la nube es con

```
ssh-copy-id usuario@hostname
```

Con esto, cuando volvamos ingresar por ssh, no será necesario la contraseña.

