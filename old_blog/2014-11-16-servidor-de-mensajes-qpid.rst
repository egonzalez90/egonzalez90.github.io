--- layout: post title: Servidor de mensajes Qpid date: 2014-11-16
17:47:34.000000000 +01:00 type: post parent_id: '0' published: true
password: '' status: publish categories: - OpenStack tags: -
configuracion - guia - instalacion - openstack - qpid - servidor de
mensaje meta: \_edit_last: '2' \_thumbnail_id: '615'
\_publicize_facebook_user: https://www.facebook.com/dudu.gonzalez90
\_publicize_twitter_user: "@hidanstillalive" \_wpas_done_all: '1'
\_wpas_skip_5226565: '1' \_wpas_skip_4949654: '1' \_wpas_skip_8706018:
'1' \_wpas_skip_10228321: '1' \_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1567488061;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:788;}i:1;a:1:{s:2:"id";i:790;}i:2;a:1:{s:2:"id";i:866;}}}}
dsq_thread_id: '6826367692' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/servidor-de-mensajes-qpid/" ---

En nuestro entorno, necesitaremos un servidor de mensajes con el que se
comunicaran los diferentes nodos y complementos de Openstack. Openstack
soporta algunos servidores de mensajes, nosotros utilizaremos Qpid,
siendo fácil su instalación y configuración básica sin autenticacion

Instalar Qpid

   yum install qpid-cpp-server

Deshabilitar el uso de la autenticación en los mensajes, asi no
necesitaremos configurar mas cosas

   vi /etc/qpidd.conf

   auth=no

Iniciar servicios y establecer el nivel de ejecución durante el arranque

   service qpidd start

   chkconfig qpidd on

Con esto ya tendríamos instalado y configurado Qpid en nuestro entorno,
en la próxima entrada ya empezaremos a configurar lo que de verdad es
Openstack. Estas entradas serán mas largas e interesantes.
