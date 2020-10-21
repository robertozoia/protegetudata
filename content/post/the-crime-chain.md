---
title: "La cadena de valor del cibercrimen"
date: 2020-09-17
draft: true
---



# La cadena de valor del robo de contraseñas


[I've been pwned]() es una página que nos permite saber si hay cuentas de servicios con nuestro correo electrónico en venta en el mercado negro. Creada por el experto en seguridar Troy Hunt, hoy es una de las referencias mundiales para saber si nuestras cuentas online han sido comprometidas. Te invito a escribir tu correo en la página y verificar si alguna de tus cuentas está en peligro.


Muchísimas personas se dan con la sorpresa de que algunas de sus cuentas aparecen en el listado del _I've bene Pwned_.  Y pueden ser cuentas de empresas importantes como Facebook o Adobe.  ¿Qué es lo que está sucediendo?

Todos los años, muchas empresas grandes y pequeñas son atacadas por hackers maliciosos que roban bases de datos con información sobre sus usuarios, sus contraseñas, teléfonos, etc. Estos robos se llaman en inglés _data breaches_. En algunos países como Estados Unidos, las empresas están obligadas a informar de estos robos, y por eso sabemos de ellos. En otros países simplemente no nos enteramos: muchas empresas consideran que comunicar a sus clientes semejante robo afectaría su reputación.

A setiembre de 2020, por ejemplo, estos son los algunos de los robos:
* Twitter (fecha), xxx robados.

La mayoría de servicios cifran las contraseñas [^hashes] de sus usuarios antes de guardarlas en sus servidores. Es decir, un servicio como Facebook no sabe qué contraseña usamos.  Cuando ingresamos nuestra contraseña para ingresar el servicio, éste la cifra y compara el resultado con el registro en su base de datos.  Si el resultado coincide, podemos acceder al sistema.

Si el atacante logra robar listas de usuarios y contraseñas de un servicio online, las contraseñas están cifradas, por lo que no las puede usar inmediatamente para acceder a nuestra cuenta.  Pero como ahora tiene la información en su computadora, cuenta con abundante tiempo para descifrar las contraseñas.  Ni siquiera tiene que ser especialmente brillante, hay un arsenal abundante de herramientas online que pude usar para hacerlo.

Del total de contraseñas robadas, el atacante solo logrará descifrar una parte. Cuántas descifre y si nuestra contraseñas estará entre ellas dependerá de longitud y complejidad de la contraseña. Para hacernos una idea, algunos tiempos referenciales:

[Buscar tiempos referenciales de crackeo de passwords]

Terminado el proceso, el atacante se queda con la relación de usuarios y contraseñas que ha logrado descifrar. Ahora puede utilizar otras herramientas que permitirán probar estos usuarios y claves por supuesto en el servicio del que fueron robados, pero también en otros servicios. Este ataque es efectivo porque, lamentablemente, mucha gente usa el mismo correo y la misma contraseña para los servicios que usa.

Aunque hemos narrado el proceso como si el atacante fuera la misma persona en cada caso, en realidad pueden haber más actores involucrados en el proceso. Así, el que inicialmente roba los datos probablemente los ponga a la venta tal cual, sin intentar descifrar las contraseñas. Otros compraran esos datos e intentarán descifrarlas, para usarlas directamente o para volverlas a vender, descifradas. También hay nichos: por ejemplo, se puede adquirir la relación de usuarios y contraseñas, probar con una herramienta automática cuáles funcionan en Netflix, y luego vender a $5 las cuentas en el mercado negro.

El cibercrimen es una industria. Según xxx, en el año 2019 una industria de $$.

No tenemos control sobre si nuestro correo y contraseña es robado de un servicio online y aparece a la venta en el mercado negro.  Pero sí podemos tomar dos medidas básicas que nos protegerán de que los usen para acceder a nuestras cuentas:  usar una contraseña suficientemente larga y complicada, y habilitar la autenticación por token en todos los servicios que usemos.


Guerra avisada, no mata gente.
