--- layout: post title: Fix Keystone malformed endpoint url 500
Openstack date: 2015-02-04 17:34:56.000000000 +01:00 type: post
parent_id: '0' published: true password: '' status: publish categories:
- OpenStack tags: - '500' - database - delete - endpoint - entry - error
- fix - http - keystone - malformed - openstack meta: \_edit_last: '2'
\_publicize_twitter_user: "@egongu90" \_wpas_done_all: '1'
\_wpas_skip_10228321: '1' \_wpas_skip_8706018: '1'
\_jetpack_related_posts_cache:
a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1566932886;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:1140;}i:1;a:1:{s:2:"id";i:879;}i:2;a:1:{s:2:"id";i:871;}}}}
dsq_thread_id: '6470916868' author: login: egongu90 email:
egongu90@hotmail.com display_name: Editor first_name: '' last_name: ''
permalink: "/fix-keystone-malformed-endpoint-url-500-openstack/" ---

 

How to fix error malformed endpoint url (HTTP 500) in Openstack

DON'T DO IT IN A PRODUCTION ENVIRONMENT
=======================================

1st - Delete the malformed endpoint in the database.

   mysql -u root -p

   # use keystone;

   # select \* from endpoint;

   # delete from endpoint where service_id="ENDPOINT_ID";

2nd - Recreate the endpoint with the keystone endpoint-create command.
