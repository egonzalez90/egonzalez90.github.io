--- layout: post title: Instancias con AWScli date: 2014-10-09
15:56:23.000000000 +02:00 type: post parent_id: '0' published: true
password: '' status: publish categories: - OpenStack tags: - amazon -
AWS - aws cli - CLI - cloud - crear - describe-instance-status -
image-id - instance-id - instancia - key-name - run-instance -
security-groups.count - services - web meta: \_edit_last: '2'
\_thumbnail_id: '631' \_publicize_facebook_user:
https://www.facebook.com/dudu.gonzalez90 \_publicize_twitter_user:
"@hidanstillalive" \_wpas_done_all: '1' \_wpas_skip_5226565: '1'
\_wpas_skip_4949654: '1' \_wpas_skip_8706018: '1'
\_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1568627311;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:777;}i:1;a:1:{s:2:"id";i:635;}i:2;a:1:{s:2:"id";i:731;}}}}
dsq_thread_id: '6119936874' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/instancias-con-awscli/" ---

Crear una instancia en EC2 classic:

   aws ec2 run-instances --image-id ami-d02386a7 --count 1
   --instance-type t1.micro --key-name kp1 --security-groups default

-  run-instances: comando para ejecutar una instancia
-  --image-id: ID de la imagen AMI a ejecutar
-  --count: numero de instancias a ejecutar
-  --instance-type: expecificaciones de hardware de la
   instancia(CPU,RAM)
-  --key-name: keypair para poder conectarnos a la instancia
-  --security-groups: grupo de seguridad del que dependera la instancia

Después comprobaremos que el estado de la instancia mediante el
siguiente comando:

    aws ec2 describe-instance-status --instance-id i-7815253a
