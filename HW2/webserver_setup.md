{\rtf1\ansi\ansicpg1252\cocoartf2761
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 HelveticaNeue;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\deftab560
\pard\pardeftab560\slleading20\partightenfactor0

\f0\fs26 \cf0 sudo apt-get update\
sudo apt-get upgrade\
sudo apt-get install apache2\
sudo nano /etc/apache2/ports.conf\
	added 8008 with \'93Listen 8008\'94\
\pard\pardeftab560\slleading20\pardirnatural\partightenfactor0
\cf0 sudo nano /etc/apache2/sites-available/000-default.conf\
\pard\pardeftab560\slleading20\partightenfactor0
\cf0 	added 8008 here as well\
sudo systemctl restart apache2\
echo "1 2 3 4 I declare a thumb war" | sudo tee /var/www/html/comp370_hw2.txt\
	create the file where i need it\
Then went to lightsail panel and under firewall added access to 8008}