Ejercicio Tema 1:
					
Buscar información sobre las tareas o servicios web para los que se usan más los programas que comentamos al principio de la sesión:

	•	apache: 
Apache es un poderoso servidor web y es completamente libre, ya que es un software Open Source y con licencia GPL. Una de las ventajas más grandes de Apache, es que es un servidor web multiplataforma, es decir, puede trabajar con diferentes sistemas operativos y mantener su excelente rendimiento. 
Apache es utilizado principalmente, para realizar servicio a páginas web, ya sean estáticas o dinámicas. Este estupendo servidor se integra a la perfección con otras aplicaciones, creando el famoso paquete XAMP con Perl, Python, MySQL y PHP, junto a cualquier sistema operativo, que por lo general es Linux, Windows o Mac OS.

	•	nginx:
NGINX es un servidor web HTTP de código abierto que también incluye servicios de correo electrónico con acceso al Internet Message Protocol (IMAP) y al servidor Post Office Protocol (POP). Además, NGINX está listo para ser utilizado como un proxy inverso. En este modo, NGINX se utiliza para equilibrar la carga entre los servidores back-end, o para proporcionar almacenamiento en caché para un servidor back-end lento.
Es util usar NGINX por su estabilidad y configuración simple. Tambien es util porque la arquitectura asíncrona del servidor web deja una pequeña huella de memoria y bajo consumo de recursos, haciéndolo ideal para el manejo de múltiples y cambiantes activas páginas Web.

	•	thttpd:
Es un servidor web de código libre disponible para la mayoría de las variantes de Unix. Se caracteriza por ser simple, pequeño, portátil, rápido, y seguro, ya que utiliza los requerimientos mínimos de un servidor HTTP.
No proporciona todas las funcionalidades de apache, pero proporciona las básicas para montar un servidor web, con un hardware modesto.

	•	Cherokee: ¿Que es cherokee y cual es su principal función? Cherokee es un servidor Web Multiplataforma ligero de software libre. Su objetivo es ser rápido y completamente funcional, sin dejar de ser liviano comparado con otros servidores web. Está escrito completamente en C. Puede usarse como un sistema embebido y soporta complementos para aumentar sus funcionalidades. El objetivo era dar una solución a un nicho de mercado que demanda servidores Web más pequeños, pero que incluyan el 95% de la funcionalidad habitual. Esto permite poderlo utilizar en hardware limitado, como un Nokia 770 o un coche teledirigido, o sacar el mayor rendimiento posible al hardware dedicado a tareas de Servidor Web. 
	•	node.js: ¿Qué es node.js? Node es un intérprete Javascript del lado del servidor que cambia la noción de cómo debería trabajar un servidor. Su meta es permitir a un programador construir aplicaciones altamente escalables y escribir código que maneje decenas de miles de conexiones simultáneas en una sólo una máquina física.  
¿Cómo funciona node.js? La meta número uno declarada de Node es "proporcionar una manera fácil para construir programas de red escalables". ¿Cuál es el problema con los programas de servidor actuales? Hagamos cuentas. En lenguajes como Java™ y PHP, cada conexión genera un nuevo hilo que potencialmente viene acompañado de 2 MB de memoria. En un sistema que tiene 8 GB de RAM, esto da un número máximo teórico de conexiones concurrentes de cerca de 4.000 usuarios. A medida que crece su base de clientes, si usted desea que su aplicación soporte más usuarios, necesitará agregar más y más servidores. Desde luego, esto suma en cuanto a los costos de servidor del negocio, a los costos de tráfico, los costos laborales, y más.  Además de estos costos están los costos por los problemas técnicos potenciales — un usuario puede estar usando diferentes servidores para cada solicitud, así que cualquier recurso compartido debe almacenarse en todos los servidores. 


Por todas estas razones, el cuello de botella en toda la arquitectura de aplicación Web (incluyendo el rendimiento del tráfico, la velocidad de procesador y la velocidad de memoria) era el número máximo de conexiones concurrentes que podía manejar un servidor. 
Node resuelve este problema cambiando la forma en que se realiza una conexión con el servidor. En lugar de generar un nuevo hilo de OS para cada conexión (y de asignarle la memoria acompañante), cada conexión dispara una ejecución de evento dentro del proceso del motor de Node. Node también afirma que nunca se quedará en punto muerto, porque no se permiten bloqueos y porque no se bloquea directamente para llamados E/S. Node afirma que un servidor que lo ejecute puede soportar decenas de miles de conexiones concurrentes.  

Bibliografía:

http://culturacion.com/que-es-apache/
http://blog.desdelinux.net/nginx-una-interesante-alternativa-a-apache/#
https://www.ibm.com/developerworks/ssa/opensource/library/os-nodejs/ https://es.wikipedia.org/wiki/Cherokee_(servidor_web)
https://es.wikipedia.org/wiki/Thttpd
http://barrapunto.com/articles/05/10/15/1142235.shtml