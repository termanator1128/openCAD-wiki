## Prerequisite
### Requirements
* cPanel
* MySQL database access
* File Manager with zip extract feature

## Let's Get Started
### Installation
1. Download the files from the [OpenCAD-php](https://github.com/StormlightTech/openCAD-php) Github such as so:
![](http://cloud.murfasa.com/3a2H1F2Q0H10/Image%202017-10-07%20at%206.31.37%20PM.png)
2. Login to your cPanel.
3. Go to the File Manager.
![](http://cloud.murfasa.com/0k1p2m2V1j22/Image%202017-10-07%20at%206.34.10%20PM.png)
4. Go to the folder where you want OpenCAD installed.
5. Upload the Zip file to that location.
6. Return to where the Zip file is.
7. Extract the zip file.
8. Delete the zip file
9. Enter the OpenCAD folder and move all of the files to the location where you want the openCAD to be.
10. Delete the OpenCAD folder we moved all of the files from.
11. Download the OpenCAD_Initialization.sql file open it in notepad.
12. Go to your cPanel and enter the MySQL Database Wizard.
13. Create the Database, it's user, and grant ALL PRIVILEGES. Make sure you take note of the FULL database name, username, and password. (This includes the letters and/or numbers and underscore before it.)
14. In the notepad, delete the first TWO lines and replace 'opencad' with your database username.
15. Go back to your cPanel and go to phpMyAdmin.
16. Navigate to the SQL tab in phpMyAdmin.
17. Go to the notepad of OpenCad_Initialization.sql, right click & click Select All and then right click & click Copy.
18. Paste this into the text box in the SQL tab in phpMyAdmin.
19. Click Go at the bottom right.
20. Make sure there are no errors.
21. Go back to the File Manager and rename 'oc-config.sample.php' to 'oc-config.php'.
22. Fill out the information for COMMUNITY_NAME, DB_NAME, DB_USER, and DB_PASSWORD.
23. Change the information for BASE_URL so there is a // in front and then the link to the location with the OpenCAD. For example, I have my OpenCAD at www.example.com/otherstuff/cad, I would put '//www.example.com/otherstuff/cad/'.
24. Go to your website and request access.
25. Go back to phpMyAdmin and then go to your database. Then go to the 'users' table. Take note of your user_id.
26. Change your approved status to '1'
27. Now go to the 'user_departments' table and select all, then copy them.
28. Change all of the user_ids to your own user_id.
29. Go to the 'users' field and delete the Default Admin user for security reasons.

### Congratulations!
Your OpenCAD is now successfully installed!
Please keep in mind we are still in a pre-Alpha stage, so many of our features are still in the works.

## More information
### Important Notes
* The OpenCAD Development team **DOES NOT** recommend the utilization of "free" webhosting solutions due to a multitude of reasons. The team has compiled a *[list of Recommended Hosting Providers](https://github.com/StormlightTech/openCAD-php/wiki/Recommended_Hosting_Provieders)*.

### Support
Still Having Trouble? on the community Discord we have setup the corresponding channels to get assistance [#linux-support](https://discord.gg/3bzVhnZ), [#windows-support](https://discord.gg/Zs3F9T). In addition to the Discord support channel we urge you to [register an account on our JIRA](https://jira.opencad.io/secure/Signup!default.jspa) and [submit any issues you have there so they may be tracked](https://jira.opencad.io/secure/CreateIssue!default.jspa). If you encounter problems with registering in JIRA please let someone in [#general-support](https://discord.gg/KYrdyv2) know.