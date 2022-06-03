## Create a BlogAPI
Using FastAPI and mySQL

mkdir blog-api
cd blog-api


### Create and activate virtual environment 

python3 -m venv env
<br/>
source env/bin/activate


### Installing dependencies
brew install mysql 
pip install -r requirements.txt

### Check mySQL Version
mysql --version


<!-- If you installed MySQL through Homebrew, you can start and stop it using the commands: -->
brew services start mysql
brew services stop mysql

### Log in as root using password
sudo mysql -u root -p

### Create a new user in mysql>
CREATE USER 'blessing'@'localhost' IDENTIFIED BY 'blessing';

### Grant user all privileges in mysql>
GRANT ALL PRIVILEGES ON *.* TO 'blessing'@'localhost' WITH GRANT OPTION;

FLUSH PRIVILEGES;

SHOW GRANTS FOR 'username'@'host';

### After creating your MySQL user and granting them privileges, you can exit the MySQL client:
exit 

### In the future, to log in as your new MySQL user, you’d use a command like the following:
mysql -u blessing -p



### Create and Select Database
CREATE DATABASE blog_api;
USE blog_api;