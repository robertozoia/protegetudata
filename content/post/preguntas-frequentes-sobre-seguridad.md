---
title: "10 Cosas sobre seguridad informática que todos deberíamos saber"
date: 2020-09-16T17:31:25-05:00
draft: true
---

Nuestro correo electrónico es una de las piezas claves de nuestra identidad en internet. A nuestro buzón de correo llegan los estados de cuenta bancarios, las boletas de pago del trabajo, confirmaciones de compra online, boarding passes, etc[^why-gmail-is-free]. Nuestra dirección de correo está también vinculada a multitud de servicios online.  Si en algún momento no recordamos la contraseña de alguna de nuestros servicios, el enlace para cambiarla llegará probablemente a nuestro correo electrónico.

[^why-gmail-is-free]:  Por si se pregutan por qué Google y otros ofrecen cuentas de correo gratis, una respuesta es que nuestro correo es una mina de datos.

Dicho de otro modo, tenemos mucho que perder si algun atacante malicioso logra hacerse nuestra cuenta de correo.  Sin embargo, muchas personas siguen usando contraseñas triviales para sus cuentas.

Quién va a estar entrando a mi cuenta. Yo no soy una persona importante.

Según el reporte de xxx de tal fecha, [buscar en el PPT de Vistage], la industria del crimen informático genera US$ billones al año.  Aún si quitamos la cifra que corresponde a la piratería de películas, juegos y otra propiedad intelectual, nos quedan yyy millones.  Sigue siendo un sector bastante atractivo.

## Tres cosas que podemos hacer para proteger nuestra cuenta de correo

1. Usar una contraseña segura y única

No hay contraseña irrompible. Pero podemos complicar las cosas a nuestro atacante de modo que no sea práctico tratar de descifrarla.

Una regla de oro es no usar la misma contraseña para varios servicios. Todos los meses hay robo de datos de diversos servicios online. Por ejemplo, el 2016 alguien [robó](https://www.usnews.com/news/technology/articles/2020-09-30/russian-man-sentenced-for-linkedin-dropbox-data-breaches) [167 millon de usuarios y contraseñas de LinkedIn](https://fortune.com/2016/05/18/linkedin-data-breach-email-password/). Si estábamos usando el mismo usuario y contraseña en LinkedIn, Facebook y GMail, nuestras cuentas de estos dos últimos servicios estarían en grave peligro.

Hay que tener en cuenta que hoy en día cualquier criminal informático que se precie usa herramientas automatizadas cuando intenta acceder ilegalmente a cuentas de terceros. Prueban miles de combinaciones de usuario/contraseña, de modo que no hace falta ser alguien especialmente destacado o un personaje público para estar expuerto a estos ataques.

Pero, ¿qué quiere decir que una contraseña es segura? Quiere decir que un atacante tardará tanto tiempo en descifrarla, que preferirá pasar a atacar a otra persona y dejará nuestra contraseña en paz.  Así, una contraseña de 12 dígitos

2. Usar un manejador de contraseñas (Password manager)

Apenas empecemos a usar una contraseña diferente para cada servicio, y teniendo en cuenta de que las buenas contraseñas no son fácilmente recordables, nos encontraremos con el problema de dónde anotarlas. Lo más recomendable es utilizar un majenador de contraseñas. Se trata un programa que nos permite guardar de modo seguro los usuarios y contraseñas de nuestras distintas cuentas. Así, solo necesitamos recordar una contraseña: la del manejador de contraseñas.

Dos manejadores bastante recomendados son:

* 1Password (https://1password.com/)
* Lastpass (https://lastpass.com/), que incluye un layer gratuito bastante completo.

La mayoría de manejadores de contraseñas ofrecen integración con los distintos navegadores, generación de passwords aleatorios según distintos parámetros (longitud de la contraseña, si tiene o no símbolos, etc.). 1Password, por ejemplo, nos alerta si inadvertidamente estamos usando una misma contraseña en distintos servicios.

3. Usar un token de seguridad

En esencia, se trata de un segundo password generado sobre la marcha que añade un nivel de seguridad importante a nuestras cuentas. El uso de token de seguridad se denomina también, en inglés,  _two-factor authentication_ (2FA), _one-time password_ (OTP), _multi-factor authentication_ (MFA).

Este password dinámico o token es un número generado normalmente por una aplicación en nuestro celular o laptop. Añade un nivel importante de seguridad a nuestra cuenta, pues aunque alguien logre hacerse con nuestro password, sin el token no podrá acceder a nuestra cuenta.

Algunas aplicaciones que permiten generar este token son [Google Authenticator](https://www.google-authenticator.com/) y [Authy](https://authy.com/) de Twilio. La ventaja de Authy, a mi parecer, es que sincroniza las cuentas entre dispositivos, de modo que podemos generar los tokens indistintamente de nuestra laptop, tablet, o smartphone.

Hoy en día los servicios más importantes como Google, Yahoo!, Facebook, Hotmail, Instagram, LinkedIn, etc.,  permiten activar 2FA para sus cuentas. Incluso algunos, como Apple, lo han hecho obligatorio para acceder a sus servicios.

Vale la pena darnos el trabajo de activar esta funcionalidad. El peligro de no hacerlo es que si un atacante  logra acceder a nuestra cuenta, éste puede activar la autenticación de dos factores y entonces perderemos el acceso a nuestra cuenta para siempre.
