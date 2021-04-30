# debug-mac-sql



pour installer SQL POUR Mac OS :
si  vieux mac on update ds le shell :


curl -fsSL -o install.sh https://raw.githubusercontent.com/Homebrew/install/master/install.sh

puis/sinon:

brew install mysql  

brew tap homebrew/services

brew services start mysql

mysql -u root -p
