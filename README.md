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


## Install Yarn and Gulp
#### Yarn is package management tool for client-side programming and it depends on NodeJS and NPM. You can install Yarn with this NPM command:
npm install -g yarn

#### Gulp is a JavaScript task runner that can automate many tasks, you can install it with NPM command as well:
npm install -g gulp

#### For verifying that Bower and Gulp are installed successfully you can execute the following command:

npm list -g --depth=0


You should see something like below:
/usr/lib
├── yarn@1.3.2
├── gulp@3.9.1
└── npm@5.3.0


#### Download and Install MEAN from GIT

Now we can download the latest version of MEAN which is “0.6.0” at the time of writing.
Execute the following command:

git clone https://github.com/meanjs/mean.git
Switch to the MEAN main directory:

cd mean
Install MEAN with the following command:

npm install
After the installation process is finished without errors you can execute the command below to install the front-end stuff:

yarn install --allow-root
Start and Test
You can easily start your MEAN stack project with the following command:

npm start


### React Native

npm install -g create-react-native-app


create-react-native-app AwesomeProject

cd AwesomeProject
npm start




