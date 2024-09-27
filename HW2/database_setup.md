{\rtf1\ansi\ansicpg1252\cocoartf2761
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 HelveticaNeue;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\deftab560
\pard\pardeftab560\slleading20\partightenfactor0

\f0\fs26 \cf0 sudo apt-get install mariadb-server\
	to get mariaDB\
sudo systemctl start mariadb\
	to start mariaDB\
sudo nano /etc/mysql/mariadb.conf.d/50-server.cnf\
	change address to allow any ip (0.0.0.0)\
	add port 6002\
sudo systemctl restart mariadb\
	restart\
sudo mysql -u root -p\
	start database\
\pard\pardeftab560\slleading20\pardirnatural\partightenfactor0
\cf0 \
\pard\pardeftab560\slleading20\partightenfactor0
\cf0 for sql commands\
CREATE DATABASE comp370_test;\
CREATE USER 'comp370'@'%' IDENTIFIED BY '$ungl@ss3s';\
GRANT ALL PRIVILEGES ON comp370_test.* TO 'comp370'@'%';\
FLUSH PRIVILEGES;\
EXIT;\
\pard\pardeftab560\slleading20\pardirnatural\partightenfactor0
\cf0 \
\pard\pardeftab560\slleading20\partightenfactor0
\cf0 then add 6002 to lightsail port}