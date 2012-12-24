<h1> Basic PHP and Mongodb connection files </h1>

What the does collection of files do? 
----
* Connect with your MongoDB database using PHP. 
* Can able to connect local or remote database by just commenting and un-commenting a single line
* Easily maintainable connection file to change any source 
* Sample JSON file for to import MongoDB data
How to install MongoDB
-----
* Go to http://www.mongodb.org/downloads to download your copy of MongoDB 
* To install MongoDB at your machine visit the installation guide at http://docs.mongodb.org/manual/installation/


How to add MongoDB Drivers at Apache ?
-----
<i> For Windows </i>

Download the correct driver for your environment from http://github.com/mongodb/mongo-php-driver/downloads. Thread safe is for running PHP as an Apache module (typical installation), non-thread safe is for CGI
Unzip and add the php_mongo.dll file to your PHP extensions directory (usually the "ext" folder in your PHP installation.)

How to configure PHP.INI file ?
---
Add to your php.ini:
* <b> extension=php_mongo.dll </b>
* Restart your web server (Apache, IIS, etc.) for the change to take effect

How to access the Front end?
---
* Download or clone the enitire source at your local and move the entire folder to your web root.
* Import the data from file <b> data.json </b> in to your collection.
* Update the file connections.php as per your DB specifications.
* Point your browser at <b> index.php </b> to view the front end (for example: http://localhost/mongo-php/index.php


What needs to be done?
---
* Inserting and retrieving binary data like MP3 & Images.
* Pagination to limit records par page.
