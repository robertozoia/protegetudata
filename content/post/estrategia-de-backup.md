---
title: "Estrategias de Backup"
date: 2020-09-20
draft: true
---

A veces actuamos como si los sucesos que rara vez ocurren no fuesen a ocurrir en realidad. Los situamos en un futuro difuminado que no toca nuestro día a día ni afecta nuestras decisiones.

¿Cuánta información perderíamos si en este momento robaran nuestra laptop? De acuerdo, puede ser que nunca roben nuestra laptop.  Pero una computadora, como cualquier equipo, tiene una vida limitada. Tarde o temprano puede suceder que deje de funcionar, simplemente por obsolescencia o por accidente.

Por otro lado, cada vez tenemos más información en nuestros equipos. Fotos, archivos, correos... Tomar alguans previsiones para tener una copia de respaldo que nos permita recuperarnos rápidamente de un accidente informático es importante y urgente.

Poner los medios para tener copias de respaldo consistentes es una de esas actividades por las que nadie siente mucho entusiasmo, porque los beneficios solo se perciben cuando ocurre el desastre.

Una condición básica es la siguiente: la estrategia de backup que usemos debe permitirnos estar trabajando como si nada hubiera pasado en un periodo corto de tiempo. Unas horas, o a lo más, un día.  Y otra condición básica es que el backup tiene que ser lo más automático y transparente posible. Porque si cada día tenemos que correr un programa manualmente para sacar una copia de respaldo, lo más probable es que terminemos por no hacerlo.

## Estrategias de backup

Al menos deberíamos tener una copia de respaldo en un disco externo, y otra copia de respaldo en un servicio en la nube.

## Soluciones sin costo

### Alojamiento en la nube

Muchos servicios ofrecen un _layer_ gratuito que incluye algo de espacio de almacenamiento en la nube. Aunque estos servicios no están pensados como servicios de backup, en la práctica pueden servir ese propósito.

Servicio           | Espacio
-------------------|-------
Dropbox            | 2GB
Microsoft OneDrive | 5GB
Apple iCloud       | 5GB
Box                | 10GB
Mega               | 50GB
Sync.com           | 5GB



Laptops y equipos de escritorio

Apple incluye en sus laptops y equipos de escritorio una aplicación llamada Time Machine precisamente para sacar copias de seguridad del disco. Para usar Time Machine solo necesitamos conectar un disco duro externo a nuestra computaora, y configurar el programa.  A partir de ahí, si dejamos la computadora con el disco conectado cuando estamos en casa o en la oficina, Time Machine se encargará de tener una copia de respaldo siempre al día.

¿De qué tamaño debería de ser el disco externo? Al menos debería tener el doble de capacidad que el disco de nuestro equipo, así Time Machine puede almacenar copias de respaldo de varios días.

En el caso de las PCs...

Time Machine hace una copia completa del equipo, de modo que si perdiéramos la máquina, bastaría conectar el disco externo a una Mac nueva y restarurar toda la información para acabar con un equipo exactamente igual al que teníamos antes.

Una segunda medida de seguridad es usar algún tipo de respaldo en la nube.


Personalmente prefiero Dropbox porque si bien los archivos están sincronizados en la nube, los archivos no dejan de estar en nuestra laptop, de modo que siempre podemos accederlos aunque no estemos conectados.
También, porque al menos en el caso de MacOS, Dropbox puede sincronizar no solo los archivos de trabajo sino también el _Desktop_ (Escritorio) y la carpeta de _Downloads_ (Descargas). Mi carpeta de Downloads es una especie de cajón donde queda todo lo que está por organizar o no amerita una carpeta propia en otra parte de mis archivos.

## Backups de todo el disco

Soluciones como Dropbox nos permiten tener respaldo de nuestros archivos de trabajo. Sin embargo, la configuración completa de nuestra laptop incluye aplicaciones y su configuración. Si tuvieramos que empezar de cero en un equipo nuevo, en el mejor de los casos nos tomaría algunas horas instalando aplicaciones y configurando correo y otros, hasta que pudiéramos tener el equipo listo para trabajar.

Existen aplicaciones que nos permiten sacar una imagen completa de todo el disco, de modo que si necesitamos, podemos restaurarla en nuestro equipo, o usarla de base para trasladar la información a un equipo nuevo.

Para MacOS, dos aplicaciones excelentes son SuperDuper y Carbon Copy Cloner. Estas aplicaciones no solo sacan una imagen exacta del disco de nuestro equipo, sino que incluso es posible arrancar el sistema usando estas copias externas.

Si tenemos un disco externo conectado a nuestra laptop cuando estamos en casa o en la oficina, estos programas se pueden configurar para que automáticamente saquen copia todos los días.


## Probar el sistema

Un punto clave es probar nuestro sistema de Backup.
