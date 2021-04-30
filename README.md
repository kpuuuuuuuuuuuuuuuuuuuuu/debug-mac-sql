# debug-mac-sql
installer sur OS


pour installer SQL POUR MAC:
si  vieux mac on update avec :
curl -fsSL -o install.sh https://raw.githubusercontent.com/Homebrew/install/master/install.sh

puis/sinon:

brew install mysql  
brew tap homebrew/services
brew services start mysql
mysql -u root -p
