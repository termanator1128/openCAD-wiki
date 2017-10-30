---
title: Installing OpenCAD
---
### Instructions
1. Download the [zip file](https://github.com/StormlightTech/openCAD-php/archive/master.zip) and extract it to either the root of your website or the folder you want it in within the website. You are also able to clone the repository and move it to either the root of your website or a folder you want it within the website.
2. Using phpMyAdmin or your favorite MySQL client, execute the openCad_Initialization.sql.
3. Copy oc-config.sample.php and name it oc-config.php.
4. In the oc-config.php, fill out the information accordingly. (Make sure you edit - define('BASE_URL', '//website url/'); )
5. Go to the website using a browser.
6. The default login information is:
	> Email: admin@test.com
	> Password: cad2017!
7. Change the default login information.
