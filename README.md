Seguridad en el aire: cómo sobrevivir a una Wi-Fi pública

alumno David Esteban Carranza Muñoz

 Introducción

En esta actividad revisé una conexión HTTP con las herramientas de desarrollador del navegador para ver qué información se envía y qué riesgos puede haber al usar una red Wi-Fi pública.

 Sitio Web analizado y evidencia: 

Visité “http://neverssl.com”. En la solicitud observada aparecen estos datos:

- URL: “http://beautifulsplendidglowingmagic.neverssl.com/online/”
- Método: “GET”
- Estado: “200 OK”
- Dirección remota: “34.223.124.45:80”
- Host: “beautifulsplendidglowingmagic.neverssl.com”
- Referer: “http://neverssl.com/”
- User-Agent: indica que usé Chrome en Windows
- También aparecen “Accept-Language” , `Accept-Encoding` y otros encabezados.

La URL comienza con `http://` y usa el puerto 80, así que la conexión observada es HTTP. En la respuesta se ven, entre otros, `Content-Type` y `Server`.

¿Qué riesgos existen al navegar mediante HTTP desde una red Wi-Fi pública? 

Los riesgos que existen son: Alguien que pueda observar el tráfico de la red podría ver la dirección visitada y los encabezados enviados, como el host, el idioma y el navegador. También podría leer o alterar datos que se envíen por una página HTTP. HTTP no cifra la comunicación.
¿Qué aporta una VPN?

Una VPN  cifra el tráfico entre mi dispositivo y el servidor VPN, creando un túnel que ayuda a protegerlo de otras personas conectadas a la misma Wi-Fi. La VPN no convierte HTTP en HTTPS: el tramo entre el servidor VPN y una página HTTP aún puede quedar sin cifrar. Por eso conviene usar sitios HTTPS, sobre todo para iniciar sesión o enviar información privada.

 Mis 3 reglas de oro

1. Revisar que el sitio use HTTPS antes de ingresar contraseñas o datos personales.
2. Evitar enviar información sensible cuando la conexión o la red no sean confiables.
3. Usar una VPN confiable en redes públicas y mantener el dispositivo actualizado.

