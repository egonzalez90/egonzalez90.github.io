--- layout: post title: Montar volumen AWS en RHEL date: 2014-09-17
17:05:47.000000000 +02:00 type: post parent_id: '0' published: true
password: '' status: publish categories: - Linux - OpenStack tags: -
amazon - añadir - AWS - cloud - computing - formatear - linux - montar -
red hat - rhel - services - volumen - web - xvdf meta: \_edit_last: '2'
\_thumbnail_id: '631' snap_MYURL: '' snapEdIT: '1' snapFB: N;
snap_isAutoPosted: '1' snapTW: N; \_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1566787474;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:731;}i:1;a:1:{s:2:"id";i:665;}i:2;a:1:{s:2:"id";i:635;}}}}
dsq_thread_id: '6107974831' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/montar-volumen-aws-en-rhel/" ---

Para poder realizar estos pasos es necesario que se haya creado un
volumen previamente en EC2 de AWS, nos conectaremos a la maquina por SSH
y seguiremos los siguientes pasos

Primero comprobaremos que el volumen que habíamos creado en EC2 le ve el
SO, utilizaremos este comando

   lsblk 

Lo normal es que el primer  volumen que añadas se llame xvdf alojado en
/dev/

Ahora lo formatearemos en EXT4

   sudo mkfs -t ext4 /dev/xvdf

A continuación crearemos la carpeta en donde montaremos el volumen y
después lo montaremos en dicha carpeta

   sudo mkdir /mnt/volumen

   sudo mount /dev/xvdf /mnt/volumen

Ahora con el comando df -h comprobaremos que el SO ya lo ve montado

::
