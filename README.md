<img src="https://raw.githubusercontent.com/estacionckweb/Telegram2Icecast/master/t2i_logo_sml_fondoblanco.jpg" /> <br>


# Telegram2Icecast



Software que permite crear una radio a partir de un grupo de chat en la red libre de mensajeria instantanea y anonima conocida como Telegram (similar al Whatsapp de la red controlada por FakeBook). t2i permite enviar/recibir/reunir y administrar contenidos individuales o grupales en un lugar accesible o privado en Internet. 

Con t2i es posible que los archivos de audio sean transmitidos en tiempo real por una emisora en Internet (via Icecast).

Un bot (script) de Telegram captura todo lo que le envias y:

-Alamacena (Text,Docs,Video,Audio) en un servidor web. <br>
-Los audios son enviados, en orden de llegada a un streaming en icecast.<br>

El bot de Telegram sirve para recoger mensajes de audio, video, documentos y textos en una rpi al mismo tiempo que genera un archivo estructurado y asequible vía navegador web, dicho archivo recoge/agrupa según categorías como: audio, video, texto, archivo todo lo compartido en el grupo de telegram (donde escucha dicho bot).


### Corre con:
node-v8.9.0-linux-armv6l en rPi - https://nodejs.org/dist/v8.9.0/node-v8.9.0-linux-armv6l.tar.gz <br>

## Pasos a seguir para correr una instancia en un computador con Node.js instalado

Solicitar un Token para el bot de Telegram usando el botFather oficial de telegram.
Una vez se haya creado el bot, crear un nuevo archivo secret.js en la carpeta raíz con el siguiente contenido:

```bash
TOKEN = "aca-va-el-token-que-genero-el-botfather"
```

Antes de correr la aplicación por primera vez es necesario instalar las dependecias:

```bash
npm install
```

Con las dependencias instaladas ya se puede correr el script con:

```bash
node t2i.js
```
