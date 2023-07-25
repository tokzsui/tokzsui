- 👋 Hi, I’m @tokzsui
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
tokzsui/tokzsui is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Teampass 3
StandWithUkraine

  PRs Welcome

  Scrutinizer Code Quality Build Status Code Intelligence Status

Teampass is a Collaborative Passwords Manager

Copyright © 2009-2023, Nils Laumaillé

Teampass 3
Requirements
Documentation
With Docker
With Docker Compose
Languages
Licence Agreement
Website
Bugs
Requirements
MySQL 5.7 or higher,
Mariadb 10.7 or higher
PHP 7.4 or higher (recommended is 8.x),
PHP extensions:
mcrypt
openssl
ldap (if used)
mbstring
bcmath
iconv
xml
gd
mysql
curl
gmp
Documentation
Read V3 documentation
With Docker
The Docker image provided will create a Teampass installation in its /var/www/html/ directory, which you should mount as a volume to keep persistent. SSL is not provided if you use this image without a proxy in front of it. See the included Docker Compose file for an example setup.

Note: Use /var/www/html/sk as your "Absolute path to saltkey" during installation.

With Docker Compose
The included docker-compose.yml file is an example setup, using virtual host-based reverse proxy routing to provide SSL. If you want to use the Compose file as-is, you will need to provide an SSL certificate with a CN matching the teampass service's VIRTUAL_HOST variable. See the documentation for the jwilder/nginx-proxy image for details. In short, you'll need to put your certificate file (with extension .crt, e.g. teampass.domain.local.crt) and the according private key file (with extension .key, e.g. teampass.domain.local.key) into the directory ssl, named exactly after the FQDN you put into the VIRTUAL_HOST variable. Make sure to restart the nginx service after changes to the certificate or at least signal it with the reload command: docker-compose exec nginx nginx -s reload.

Note1: The database's hostname is db. You can find the database's credentials in the environment variables of the db service.

Note2: Use /var/www/html/sk as your "Absolute path to saltkey" during installation.

Languages
Teampass is currently available in the following languages:

ENGLISH
CATALAN
CHINESE
CZECH
DUTCH
ESTONIAN
FRENCH
GERMAN
HUNGARIAN
ITALIAN
JAPANESE
NORWEGIAN
PORTUGUESE
PORTUGUESE (BR)
ROMANIAN
RUSSIAN
SPANISH
TURKISH
UKRAINIAN
VIETNAMESE
Languages strings are managed at POEditor.com.

Licence Agreement
Licence defined as GNU General Public License v3.0 only.

This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Read Licence

Website
Visit Teampass.net

Bugs
If you discover bugs, please report them in Github Issues.
