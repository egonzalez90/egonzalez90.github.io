--- layout: post title: Habilitar SSH a host ESXi date: 2014-05-05
22:20:10.000000000 +02:00 type: post parent_id: '0' published: true
password: '' status: publish categories: - Virtualizacion tags: -
connection refused - error - esxi - host - putty - ssh - vcenter -
virtualizacion - vmware - vSphere meta: \_edit_last: '2'
\_login_radius_meta: a:1:{s:7:"sharing";i:0;} \_layout: inherit
\_thumbnail_id: '514' \_nxs_snap_sh_FB0_1399324812:
a:33:{s:4:"doFB";i:1;s:5:"nName";s:8:"Facebook";s:7:"fbAppID";s:15:"545659862207806";s:8:"fbAppSec";s:32:"15477463b8c7d194394cc5dba87a27f1";s:6:"catSel";i:0;s:8:"catSelEd";s:0:"";s:8:"postType";s:1:"A";s:7:"fbAttch";s:1:"2";s:12:"fbAttchAsVid";i:0;s:6:"imgUpl";s:1:"1";s:11:"fbMsgFormat";s:42:"(%TITLE%)
has been published on
%SITENAME%";s:10:"fbMsgAFrmt";s:0:"";s:13:"useFBGURLInfo";s:1:"1";s:10:"riComments";i:0;s:12:"riCommentsAA";i:0;s:8:"rpstDays";i:0;s:7:"rpstHrs";i:0;s:8:"rpstMins";i:0;s:6:"rpstOn";i:0;s:11:"rpstOnlyPUP";i:0;s:7:"fltrsOn";i:0;s:11:"rpstBtwDays";a:0:{}s:5:"fbURL";s:40:"https://www.facebook.com/dudu.gonzalez90";s:6:"fbPgID";s:15:"dudu.gonzalez90";s:14:"fbAppAuthToken";s:184:"CAAHwRlZABTT4BAJUZAayCdD8sT9vucqP95dtUZAPJ5bmoC6gIB55tOiHIny4rESJKtch31GgGgKVPKMn22UrmAy0QDSE1A2jeun45RPysZAvHGxiz6KoWknUrezqkRtdThZAgxAYOVgKZC8XQ1gp4MAhyNNbsIjeBVlCAn9h6aZAAmih8x3NFKM";s:18:"fbAppPageAuthToken";s:184:"CAAHwRlZABTT4BAJUZAayCdD8sT9vucqP95dtUZAPJ5bmoC6gIB55tOiHIny4rESJKtch31GgGgKVPKMn22UrmAy0QDSE1A2jeun45RPysZAvHGxiz6KoWknUrezqkRtdThZAgxAYOVgKZC8XQ1gp4MAhyNNbsIjeBVlCAn9h6aZAAmih8x3NFKM";s:13:"fbAppAuthUser";s:10:"1161837279";s:17:"fbAppAuthUserName";s:31:"Dudu
Gonzalez
(dudu.gonzalez90)";s:8:"isPosted";s:0:"";s:8:"imgToUse";s:0:"";s:8:"urlToUse";s:0:"";s:2:"ii";i:0;s:9:"timeToRun";i:1399324812;}
snap_isAutoPosted: '1' \_nxs_snap_sh_TW0_1399324815:
a:37:{s:4:"doTW";i:1;s:5:"nName";s:7:"Twitter";s:5:"twURL";s:34:"https://twitter.com/DuduGonzalez90";s:9:"twConsKey";s:21:"QTmaTFDqowEzbyzkicvgg";s:9:"twConsSec";s:43:"9EWEc5dEufuzc3wjm0fZAD8yJdxhFiHcFR06IgsHPb4";s:10:"twAccToken";s:50:"767702022-PedOOiQm697uAVksTggg5Am0W2eiUlXcF1u1kkJ6";s:6:"catSel";s:1:"0";s:8:"catSelEd";s:0:"";s:10:"riComments";i:0;s:11:"riCommentsM";i:0;s:12:"riCommentsAA";i:0;s:8:"rpstDays";i:0;s:7:"rpstHrs";i:0;s:8:"rpstMins";i:0;s:6:"rpstOn";i:0;s:11:"rpstOnlyPUP";i:0;s:7:"fltrsOn";i:0;s:11:"rpstBtwDays";a:0:{}s:13:"twAccTokenSec";s:45:"Bumkti9owi1FxQgY8jOMyRJ6LznMXzcUUWwY0Qmvd0k6N";s:11:"twMsgFormat";s:15:"%TITLE%
-
%URL%";s:8:"attchImg";i:1;s:4:"twOK";i:1;s:11:"rpstRndMins";i:0;s:12:"rpstPostIncl";s:1:"0";s:8:"rpstType";s:1:"2";s:12:"rpstTimeType";s:1:"A";s:12:"rpstFromTime";s:0:"";s:10:"rpstToTime";s:0:"";s:10:"rpstOLDays";s:2:"30";s:10:"rpstNWDays";s:3:"365";s:7:"tagsSel";s:0:"";s:8:"tagsSelX";s:0:"";s:8:"rpstStop";s:1:"O";s:8:"isPosted";s:0:"";s:8:"imgToUse";s:0:"";s:2:"ii";i:0;s:9:"timeToRun";i:1399324815;}
snap_MYURL: '' snapEdIT: '1' snapFB: N; snapTW: N;
kopa_resolution_total_view: '1' \_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1567908887;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:551;}i:1;a:1:{s:2:"id";i:545;}i:2;a:1:{s:2:"id";i:527;}}}}
dsq_thread_id: '6127560330' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/habilitar-ssh-a-host-esxi/" ---

 

Cuando instalas un host ESXi, lo normal es acceder a el a través de
vSphere Client, web client o por un vCenter por alguno de los modos
anteriores. El problema es que hasta que no lo necesitas, no te acuerdas
de que existe el SSH, y el día que lo necesites no podrás utilizarlo...
Es la Ley de Murphy.

Lo mas normal es acceder por SSH con un cliente como PUTTY, pues bien,
una vez pones la direccion IP o el FQDN del host ESXi y das a
conectar(esto tambien pasa desde una consola de Linux), te sale este
mensaje de conexion rechazada.
`Captura <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura13.png>`__

Esto se debe a que por defecto, los host ESXi tienen deshabilitado el
acceso por SSH. Para habilitarlo, tenemos dos métodos: Desde vSphere
Client al ESXi o vCenter, o desde el propio host ESXi

vSphere Client

Una vez hemos accedido al VSphere Client, pulsaremos sobre el host al
que queramos habilitar SSH, aquí iremos a la pestaña superior de
Configuration.\ `Captura1 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura14.png>`__

Una vez dentro de la pestaña de Configuration, buscaremos por la barra
lateral izquierda Security Profile, dentro de Software, nos mostrara
esta ventana en la que iremos a el botón de Properties de la parte
superior
derecha\ `Captura2 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura21.png>`__

Esto nos abrirá esta ventana en la que buscaremos SSH, veremos que esta
en estado Stoped, pulsaremos sobre el botón Options

`Captura3 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura31.png>`__

Aqui marcaremos la segunda opción para que inicie el servicio con el
arranque y parada del host ESXi, ademas también pulsaremos sobre el
botón Start para iniciar el servicio en estos momentos y finalizaremos
pulsando sobre el botón OK

`Captura4 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura41.png>`__

Ahora nos quedaría comprobar que efectivamente tenemos acceso al host a
través de SSH.

Una vez pongamos la dirección de nuestro host en PuTTY, en vez de
mostrarnos el mensaje de error, nos pedirá que aceptemos la clave del
host, esto lo haremos pulsando sobre
Si\ `Captura5 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura51.png>`__

Se nos abrirá una consola de comandos en la que introduciremos el
usuario y contraseña del host ESXi.

Ya estaríamos conectados por
SSH\ `Captura6 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura61.png>`__

**Host ESXi**

Ahora haremos lo mismo que anteriormente pero a través del propio host.

Para entrar en el menú de configuración, pulsaremos F2, esto nos pedirá
usuario y contraseña. Una vez loggeados, veremos esta pantalla, aquí
iremos a la opción Troubleshootin Options y pulsaremos
Enter\ `Captura7 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura71.png>`__

Nos abrira esta otra pantalla en la que observamos que tenemos SSH
deshabilitado, nos ponemos sobre Enable SSH y pulsamos
Enter\ `Captura8 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura81.png>`__

Como vemos ahora tenemos SSH habilitado y tendríamos acceso remoto desde
PuTTY

Esta forma es mas sencilla que la anterior, pero deberemos de tener
algún tipo de acceso hacia nuestro host para poder
configurarlo\ `Captura9 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/05/Captura91.png>`__

Espero les sirva de ayuda.

Un saludo.
