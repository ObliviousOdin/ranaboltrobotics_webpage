# ranaboltrobotics_webpage


## Install Dependencies

apt-get install build-essential git fontconfig libpng-dev ruby ruby-dev

gem install sass


## Install MongoDB
In this section, we are going to install MongoDB as our Database, in order to install the latest stable version of MongoDB you should add the official repository:

apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6
Execute the following command to add the repository data in the proper path:

echo "deb [ arch=amd64,arm64 ] http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4 multiverse" | tee /etc/apt/sources.list.d/mongodb-org-3.4.list
Now you can easily install MongoDB with the following command:

apt-get install mongodb-org
After the installation process is finished you can start and enable the MongoDB service with the commands below:

systemctl start mongod
systemctl enable mongod


## Install NodeJS and NPM
In order to install Node.JS and NPM we have to add the “NodeSource” repository, the following bash script will do this easily:

curl -sL https://deb.nodesource.com/setup_8.x | -E bash -
Now you can execute the command below to install Node.JS and NPM:

apt-get install nodejs

### Check the installed versions:

node -v
v8.9.1

npm -v
5.5.1

### change node to js 
ln -s /usr/bin/nodejs /usr/bin/node








