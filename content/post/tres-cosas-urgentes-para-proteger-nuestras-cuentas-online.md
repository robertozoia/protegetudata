---
title: "Tres medidas urgentes para proteger nuestras cuentas online"
date: 2020-10-19
draft: false
---

Un elemento importantes para la seguridad de nuestras cuentas online son las contraseñas. En abril de 2019, Scientific American publicó un excelente artíciulo titulado [The Mathematics of (Hacking) Passwords](https://www.scientificamerican.com/article/the-mathematics-of-hacking-passwords/), en el que el autor intenta explicar cómo se relacionan la longitud y complejidad de nuestra contraseña y la seguridad de nuestras cuentas.

Por ejemplo, si escogemos un password de 6 letras minúsculas, hay 26 posibilidades para la primera letra, 26 posibilidades para la segunda, etc. Como estas posiblidades son independientes entre sí, el "tamaño" del espacio para esta contraseña es de 26 x 26 x 26 x 26 x 26 x 26 = 26<sup>6</sup>, o lo que es lo mismo, estaremos generando una contraseña entre 26<sup>6</sup> ó 308,915,776 posibilidades. Si alguien tratara de encontrar nuestra contraseña probando una a una las distintas posibilidades --un tipo de ataque que en ciberseguridad se llama, apropiadamente, de _fuerza bruta_-- tendría que estar dispuesto a probar las 26<sup>6</sup> posibilidades.

Si en cambio usamos un password de 12 caracteres, e incluimos no solo letras minúsculas sino también mayúsculas, dígitos y símbolos (!, @, &, etc.), el aumento en la complejidad de encontrar la contraseña para un posible atacante aumenta significativamente con respecto a la contraseña de 6 caracteres. Ahora tenemos 72 posibilidades para cada caracter. El tamaño del espacio sería de  72<sup>12</sup> o 19,408,409,961,765,342,806,016, un número cercano a 19 seguido de 21 ceros.

La contraseña de 6 caracteres se puede romper hoy en menos de 1 hora. Pero tendrán que pasar al menos unos 29 años para que la tecnología nos permita romper la contraseña de 26 caracteres en menos de 1 hora.[^moore]

[^moore]: Esto suponiendo que no habrá un descubrimiento tecnológico significativo como computación cuántica practicable, o un descubrimiento matemático importante que permita romper el cifrado de modo más eficiente. El artículo mencionado arribna presenta una fórmula que usa la Ley de Moore para estimar la capacidad de procesamiento disponible en determinado año. La Ley de Moore es una ley empírica que dice que la capacidad de procesamiento disponible a precio constante se duplica cada 18 meses.

## Robos de información, contraseñas triviales y contraseñas repetidas

Con cierta frecuencia, algún servicio importante sufre un _data breach_, es decir, un robo de información que puede contener datos como usuarios y contraseñas[^microsoft-data-breach]. Aunque estas contraseñas robadas estén cifradas, si son triviales pueden ser rotas en poco tiempo por los criminales.

Si queremos saber si nuestro usuario aparece en uno de estos _data breaches_, podemos consultarlo en [Have I been Pwned?](https://haveibeenpwned.com/), creado por Troy Hunt, Director de Microsoft y MVP.

Gracias a que esta información robada se puede comprar en el mercado negro, los expertos en seguridad han recopilado información estadística sobre las contraseñas más usadas en el mundo[^my-password-pwned]. Desde hace años, la contraseña que aparece en el primer lugar del ranking de contraseñas más usadas es nada menos que *123456*. En estas estadísticas, el número de personas que usan contraseñas triviales también es alto, así como el número de personas que usa la misma contraseña para distintos servicios.

[^microsoft-data-breach]: Por ejemplo, en enero de 2020, [Microsoft sufrió el robo de la información](https://www.forbes.com/sites/daveywinder/2020/01/22/microsoft-security-shocker-as-250-million-customer-records-exposed-online/#cb5710d4d1b3) de 250 millones de usuarios.

[^my-password-pwned]:  [';--have i been pwned?](https://haveibeenpwned.com/Passwords) permite verificar si una contraseña ha sido comprometida contra una base de 500 millones de contraseñas robadas.

Aunque no usemos contarseñas como *123456*, quizá sí estemos usando una palabra fácil de recordar y algunos números para nuestra contraseña: el nombre de una ciudad a la que estamos vinculados emocionalmente, el nombre de una canción, o de alguno de nuestros hijos.  Esto tampoco nos protege mucho, y para un programa para romper passwords es igual de fácil romper la contraseña del ejemplo anterior que acertar con el nombre de nuestro jugador de fútbol favorito.

## Tres cosas que deberíamos hacer

La primera medida de seguridad que podemos tomar es usar una contraseña tan larga como podamos, lo más aleatoria que podamos, y que combiene letras mayúsculas, minúsculas, números y símbolos. Si el servicio en cuestión acepta contraseñas de 64 caracteres, usemos 64 en vez de 12. Con eso ponemos una barrera importante entre nosotros y los atacantes, que se conformarán con escoger víctimas con contraseñas más sencillas que romper.

La segunda medida importante es usar contraseñas distinta para servicios distintos. Si un ladrón robara la llave de la casa y nuestra dirección, lo primero que haríamos sería cambiar la cerradura. Si además esa llave abre la puerta de nuestro auto, de nuestra oficina, y la casa de otros familiares, estamos en verdaderos problemas.

Si usamos el mismo usuario y contraseña en varios servicios, basta que roben información de uno de esos servicios par que puedan comprometer nuestras cuentas en todos los servicios en los que usamos esa contraseña. Y no nos engañemos: todos los principales servicios (Facebook, LinkedIn, Microsoft, Google, etc.) han sufrido robos de información importantes.


Si mucha gente usa contraseñas triviales y la misma contraseña para varios servicios, es en parte porque crear y recordar contraseñas aleatorias, suficientemente largas, y diferentes es inconveniente y molesto[^token]. Algunos encargados de TI corporativos se lavan las manos estableciendo políticas que obligan o a sus usuarios que renueven la contraseña cada 30 días... Lo que hacen muchos usuarios es anotarlas en un Excel o en un post-it que pegan en su laptop.

[^token]: Como se explica en otro artículo, la contraseña larga y aleatoria debe complementarse con un segundo factor de autenticación, un token que se regenera cada tanto tiempo generado por una aplicación. De ese modo, aunque el atacante logre hacerse con la contraseña, no podrá acceder al servicio con nuestro usuario pues no tiene el token.

La tercera medida de seguridad es utilizar un manejador de contraseñas (password manager). Se trata de una aplicación que almacena nuestros usuarios y contraseñas, y los protege con una contraseña única. Así, solo tenemos que recordar _esa_ contraseña. Hay muchos buenos _password managers_ disponibles, como [1Password](https://1password.com) o [LastPass](https://lastpass.com). Estos programas ofrecen extensiones para el navegador, permiten generar contraseñas aleatorias (mi longitud actual cuando el servicio lo permite es 64 caracteres), e incluso incorporan un generador de tokens asociado a la cuenta. Cuando un servico que usamos sufre una brecha de seguridad, el manejador de contraseñas nos alerta, cambiamos la contraseña, y volvemos a estar del lado seguro.

En conclusión, usar una contraseña segura es el primer paso para asegurar nuestra presencia online. La segunda es usar un token como segundo factor de autenticación para nuestras cuentas.  Pero eso lo dejaremos para otro artículo.
