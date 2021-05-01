# debug-mac-sql



pour installer SQL POUR Mac OS :
si  vieux mac on update ds le shell :


curl -fsSL -o install.sh https://raw.githubusercontent.com/Homebrew/install/master/install.sh

puis/sinon:

brew install mysql  

brew tap homebrew/services

brew services start mysql

mysql -u root -p


pour connecté le shell sql en cours avec son phpmyadmin:
/Applications/MAMP/Library/bin/mysql --host=localhost -uroot -proot



pour customiser shell avec zsh:
chsh -s /bin/zsh
echo $SHELL
curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh

