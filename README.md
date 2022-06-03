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

### Log in as root 
mysql -u root

### Change your root password after installation:
mysqladmin -u root password [newpassword]

### Log in as root using password
mysql -u root -p