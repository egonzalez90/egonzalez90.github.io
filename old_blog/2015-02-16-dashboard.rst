--- layout: post title: Dashboard date: 2015-02-16 13:11:29.000000000
+01:00 type: post parent_id: '0' published: true password: '' status:
publish categories: - OpenStack tags: - dashboard - httpd - memcached -
openstack meta: \_edit_last: '2' \_wpas_mess: Dashboard
\_wpas_skip_10228321: '1' \_wpas_skip_5226565: '1' \_wpas_done_all: '1'
\_publicize_facebook_user: https://www.facebook.com/dudu.gonzalez90
\_publicize_twitter_user: "@egongu90" \_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1566543514;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:879;}i:1;a:1:{s:2:"id";i:898;}i:2;a:1:{s:2:"id";i:798;}}}}
dsq_thread_id: '6177881259' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/dashboard/" ---

Instalamos los paquetes necesarios para usar Dashboard.

   # yum install memcached python-memcached mod_wsgi openstack-dashboard

Editamos el siguiente fichero y añadimos/modificamos las lineas
Allowed_hosts y Openstack_host.

   # vi /etc/openstack-dashboard/local-settings

   ALLOWED_HOSTS=['*']

   OPENSTACK_HOST="controller"

Permitimos conexiones al servicio httpd en la politica de SElinux.

   # setsebool -P httpd_can_network_connect on

Iniciamos los servicios y establecemos el nivel de ejecución.

   # service httpd start

   # service memcached start

   # chkconfig httpd on

   # chkconfig memcached on
