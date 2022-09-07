# Flow-2
Este es el segundo ejercicio en Node-RED  donde mostramos la fecha y hora cada segundo en formato normal
## Material necesario

**Software**
- [Ubuntu 20.04](https://releases.ubuntu.com/20.04/)
- Firefox
- Terminal
- Node JS [NodeSource](https://github.com/nodesource/distributions/blob/master/README.md)
- NPM
- Node-RED [Locally](https://nodered.org/docs/getting-started/local)


**Hardware**
- Equipo PC

## Material de referencia 
En los siguientes enlaces entontraras las piginas y cursos de donde se sacó la información para el desarollo de este primer Flow en Node-RED

- [Instalacion de Virtual Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)

- [Instalacion de Node-RED](https://edu.codigoiot.com/course/view.php?id=817)

- [Introduccción a Node-RED](https://edu.codigoiot.com/enrol/index.php?id=278)

## Instrucciones
**Requisistos previos**
Para el correcto funcionamiento de este flow debes cumplir con los siguientes requisitos previos

1. Instalación de NodeJS. Para este ejercicio se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM

2. nstalación de NodeRed. La instalación se realiza por NPM. para este ejercicio, se usó la versión 3.0.2

**Preparación de Node-RED**
1. Arranacar Node-RED mediante la terminal usando el comando `node-red`.

2. Abrir Node-RED en [Firefox](localhost:1880/) escribiendo "localhost:1880/" en el buscador. 

3. Importar el primer programa realizado [Flow_1](https://github.com/aramisroldan/Flow-1.git)


4. Agregar un bloque `function` y agregarle el siguiente codigo:

// Lo que está después de “//” son comentarios
// Crea un objeto Date a partir del payload enviado por timestamp
var date = new Date(msg.payload);
// Cambia el payload para que sea una fecha con formato
msg.payload = date.toString();
// Regresa el mensaje para que se envíe al sigueinte nodo
return msg;

## Resultados
En la siguente imagen se puede observar una vista del funcionamiento de este flow:

![Funcionamiento del programa](https://github.com/aramisroldan/Flow-1/blob/main/Flow_1.png)

## Evidencias 

## Creditos