--- layout: post title: Crear Raid 1 en Linux date: 2014-02-14
00:34:24.000000000 +01:00 type: post parent_id: '0' published: true
password: '' status: publish categories: - Linux tags: - configuracion -
Debian - disco duro - linux - mdadm - raid meta: \_edit_last: '2'
\_login_radius_meta: a:1:{s:7:"sharing";i:0;}
nxs_snap_sh_FB0_1392338069:
a:32:{s:4:"doFB";i:1;s:5:"nName";s:8:"Facebook";s:7:"fbAppID";s:15:"545659862207806";s:8:"fbAppSec";s:32:"15477463b8c7d194394cc5dba87a27f1";s:6:"catSel";i:0;s:8:"catSelEd";s:0:"";s:8:"postType";s:1:"A";s:7:"fbAttch";s:1:"2";s:12:"fbAttchAsVid";i:0;s:6:"imgUpl";s:1:"1";s:11:"fbMsgFormat";s:52:"Re-subido
(%TITLE%) has been published on
%SITENAME%";s:10:"fbMsgAFrmt";s:0:"";s:13:"useFBGURLInfo";s:1:"1";s:10:"riComments";i:0;s:12:"riCommentsAA";i:0;s:8:"rpstDays";i:0;s:7:"rpstHrs";i:0;s:8:"rpstMins";i:0;s:6:"rpstOn";i:0;s:11:"rpstOnlyPUP";i:0;s:7:"fltrsOn";i:0;s:11:"rpstBtwDays";a:0:{}s:5:"fbURL";s:40:"https://www.facebook.com/dudu.gonzalez90";s:6:"fbPgID";s:15:"dudu.gonzalez90";s:14:"fbAppAuthToken";s:183:"CAAHwRlZABTT4BAHa5L1j1rQSgQeHGVLk8rZCb7JuVgkDizv9FqTtDVQCX02ZA5bDr1kqFEppdFuJz3oS79n7z8COso57qcDaVZBWLA3PuOEwxNXd1d4y39DjUfTJkQJAMWw0TnZCnSqeDG6KRJ6zpfUu6Gt0ZBAs7Ym3NvKf4BPSCJ8HzoaQCH";s:18:"fbAppPageAuthToken";s:183:"CAAHwRlZABTT4BAHa5L1j1rQSgQeHGVLk8rZCb7JuVgkDizv9FqTtDVQCX02ZA5bDr1kqFEppdFuJz3oS79n7z8COso57qcDaVZBWLA3PuOEwxNXd1d4y39DjUfTJkQJAMWw0TnZCnSqeDG6KRJ6zpfUu6Gt0ZBAs7Ym3NvKf4BPSCJ8HzoaQCH";s:13:"fbAppAuthUser";s:10:"1161837279";s:8:"isPosted";s:0:"";s:8:"imgToUse";s:0:"";s:8:"urlToUse";s:0:"";s:2:"ii";i:0;s:9:"timeToRun";i:1392338069;}
snap_isAutoPosted: '1' nxs_snap_sh_TW0_1392338074:
a:36:{s:4:"doTW";i:1;s:5:"nName";s:7:"Twitter";s:5:"twURL";s:29:"https://twitter.com/zombies3c";s:9:"twConsKey";s:21:"QTmaTFDqowEzbyzkicvgg";s:9:"twConsSec";s:43:"9EWEc5dEufuzc3wjm0fZAD8yJdxhFiHcFR06IgsHPb4";s:10:"twAccToken";s:50:"767702022-PedOOiQm697uAVksTggg5Am0W2eiUlXcF1u1kkJ6";s:6:"catSel";s:1:"0";s:8:"catSelEd";s:0:"";s:10:"riComments";i:0;s:11:"riCommentsM";i:0;s:12:"riCommentsAA";i:0;s:8:"rpstDays";s:1:"0";s:7:"rpstHrs";s:1:"0";s:8:"rpstMins";s:1:"0";s:6:"rpstOn";i:0;s:11:"rpstOnlyPUP";i:0;s:7:"fltrsOn";i:0;s:11:"rpstBtwDays";a:0:{}s:13:"twAccTokenSec";s:45:"Bumkti9owi1FxQgY8jOMyRJ6LznMXzcUUWwY0Qmvd0k6N";s:11:"twMsgFormat";s:25:"Re-subido
%TITLE% -
%URL%";s:8:"attchImg";i:1;s:4:"twOK";i:1;s:11:"rpstRndMins";i:0;s:12:"rpstPostIncl";s:1:"0";s:8:"rpstType";s:1:"2";s:12:"rpstTimeType";s:1:"A";s:12:"rpstFromTime";s:0:"";s:10:"rpstToTime";s:0:"";s:10:"rpstOLDays";s:2:"30";s:10:"rpstNWDays";s:3:"365";s:7:"tagsSel";s:0:"";s:8:"tagsSelX";s:0:"";s:8:"isPosted";s:0:"";s:8:"imgToUse";s:0:"";s:2:"ii";i:0;s:9:"timeToRun";i:1392338074;}
\_thumbnail_id: '265' ac_featured_article: '' ac_show_post_thumbnail: ''
snap_MYURL: '' snapEdIT: '1' snapFB: N; snapTW: N;
\_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1567801990;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:284;}i:1;a:1:{s:2:"id";i:584;}i:2;a:1:{s:2:"id";i:393;}}}}
dsq_thread_id: '6094297017' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/crear-raid-1-en-linux/" ---

 

**En esta entrada, voy a mostrar como se crea un raid de nivel 1 bajo
Linux, también simulare como cambiar un disco en caso de que uno
falle.**

**Empecemos:**

**Cuando iniciamos la consola de Linux, comprobaremos que discos duros
tenemos disponibles, en esta pantalla vemos que están sda, sdb**

`1 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/1.jpg>`__

**En esta otra esta sdc, vemos que tanto sdb como sdc están sin formato
alguno**

`2 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/2.jpg>`__

**Ahora instalaremos el paquete mdadm, que será el que nos permita
configurar un raid en el sistema **

`3 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/3.jpg>`__

**Ahora crearemos un nuevo dispositivo llamado md0, con un raid de nivel
1, añadiendo los dispositivos sdb y sdc a este**

 

`4 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/4.jpg>`__

**Ahora configuraremos este dispositivo que hemos creado previamente**

`5 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/5.jpg>`__

**Utilizaremos la opción N para crear una nueva partición**

**Seleccionaremos P para hacerla primaria**

**Estableceremos que la partición es la numero 1**

**Pondremos el cilindro número 1 como primero, y el último de los que
tengamos disponibles como final**

`6 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/6.jpg>`__

**Después utilizaremos la opción W para escribir los cambios al disco**

`7 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/7.jpg>`__

**Ahora crearemos el sistema de fichero mediante el comando mkfs y el
dispositivo que habíamos creado**

`8 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/8.jpg>`__

**Ahora crearemos una carpeta de montaje de nuestro dispositivo mediante
mkdir**

**Después montaremos el dispositivo a dicha carpeta mediante el comando
mount**

`9 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/9.jpg>`__

**Ahora crearemos un fichero de un tamaño determinado que se especifica
en la opción bs **

`10 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/10.jpg>`__

**Ahora comprobamos esta carpeta, y vemos que los tamaños están bien
configurados**

`11 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/11.jpg>`__

**Ahora comprobaremos en este archivo que el raid está activo, y tiene
los dispositivos sdb y sdc**

`12 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/12.jpg>`__

**Ahora haremos como que el disco sdb ha fallado, para poder quitarle
del raid para remplazarle primero hay que marcarle como disco fallido
mediante este comando**

`13 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/13.jpg>`__

**Ahora le quitaremos del raid el disco sdb**

`14 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/14.jpg>`__

**Iremos al archivo del raid y comprobamos que no está el disco sdb
dentro de el**

`15 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/15.jpg>`__

**Ahora borraremos los datos de configuración anterior del disco sdb
mediante el primer comando.**

**Después añadimos el disco sdb al disco raid, esto si tiene datos
tardara un tiempo en sincronizar**

`16 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/16.jpg>`__

**Ahora desactivaremos el raid mediante este comando**

`17 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/17.jpg>`__

**Si queremos volver a activarle, lo haremos mediante este otro
comando**

`18 <http://vps38574.vps.ovh.ca/wp-content/uploads/2014/02/18.jpg>`__
