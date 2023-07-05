# Instalando Go tools

## Descarga

Primero debemos descargar el binario que contiene el ejecutable, aunque también podemos installar Go desde su código fuente. Para ello debemos descargar la versión que deseemos instalar desde este enlace [Descarga](https://go.dev/dl/). Eligiendo la versión correcta para nuestro sistema operativo.

## Instalción

Estas son las instrucciones para realizar la instalación desde Linux, Mac o Windos.

### Linux

Debemos remover cualquier version de Go que tengamos instalada anteriormente en la carpeta `/usr/local/go` (si es que existe), entonces extraemos el archivo que acabamos de descargar en `/usr/local`, creando un nuevo arbol de directorios en `/usr/local/go`, lo podemos realizar con el siguiente comando:

```
$ rm -rf /usr/local/go && tar -C /usr/local -xzf go1.20.5.linux-amd64.tar.gz
```

(Probablemente necesites correr el comando como `root` o utilizar el comando `sudo`).

No debemos extraer el archivo en una extructura de directorios `/usr/local/go` pre-existente. Es sabido que eso rompe con la instalación de Go.

Debemos añadir esta ruta `/usr/local/go/bin` a nuestra variable de entorno `PATH`.

Puede hacer eso añadiendo la siguiente línea a su `$HOME/.profile` o `/etc/profile`:

```
export PATH=$PATH:/usr/local/go/bin
```

Nota: Los cambios realizados en el archivo de perfil pueden no aplicarse hasta la proxima vez que se "loguee" en su computadora. Para aplicar los cambios de inmediato, debe correr el comando direcatemente en la `shell` o o ejecutarlo en el perfil utilizando el comando como en el archivo `$HOME/.profile`.

Para verificar que a realizado una correcta instalación de Go debe abrir la línea de comando y ejecutar lo siguiente:

```
$ go version
```

Si salio todo correctamente el comando debe imprimir en pantalla la version de Go instalada.

### Mac

Abra el archivo que descargo y siga las instrucciones que va a ver en el `prompts` para instalar Go.

El paquete instalara la distribucion de Go en `/usr/local/go`. El paquete debe colocar la ruta `/usr/local/go/bin` en su variable de entorno PATH. Puede necesitar re-iniciar cualquier sesión en la terminal para que los cambios surjan efecto.

Para verificar que a realizado una correcta instalación de Go debe abrir la línea de comando y ejecutar lo siguiente:

```
$ go version
```

Si salio todo correctamente el comando debe imprimir en pantalla la version de Go instalada.

### Windows

Abra el archivo MSI que descargo y siga las instruccion que vera en el prompts para instalar Go.

Por defecto, el instalador va a instalar Go en Program Files o Program Files (x86). Usted puede cambiar la ubicación si lo necesita. Despues de la instalación, va a necesitar cerrar y volver a abrir cualquier terminal para que la cambie el entorno para que la instalación de Go se vea reflejada.

Para verificar que tiene instalado Go.

En Windows, haga click en el menú de Inicio.
En el buscador, tipee cmd, y presione la tecla Enter.
En la línea de comando que aparece en la ventana, tipee el siguiente comando:

```
$ go version
```

Si salio todo correctamente el comando debe imprimir en pantalla la version de Go instalada.

## Siguiente paso

Eso es todo, también pueden leer la [Documentación oficial](https://go.dev/doc/install). Una vez terminado este proceso vamos a continuar eligiendo un editor de código.
