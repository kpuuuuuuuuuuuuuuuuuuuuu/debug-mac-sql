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




       __                                     __
  ____  / /_     ____ ___  __  __   ____  _____/ /_
 / __ \/ __ \   / __ `__ \/ / / /  /_  / / ___/ __ \
/ /_/ / / / /  / / / / / / /_/ /    / /_(__  ) / / /
\____/_/ /_/  /_/ /_/ /_/\__, /    /___/____/_/ /_/
                        /____/                       ....is now installed!



CUSTOMISER shell avec zsh:                  https://medium.com/wearetheledger/oh-my-zsh-made-for-cli-lovers-installation-guide-3131ca5491fb

                        
                        
Choisir un thème

https://github.com/ohmyzsh/ohmyzsh/wiki/Themes


voir les themes dispo sur l'ordi
cd ~/.oh-my-zsh/themes
ls


Before you scream Oh My Zsh! please look over the ~/.zshrc file to select plugins, themes, and options.

Install prerequisite packages
$ sudo apt install git-core zsh

Install Oh-My-Zsh from Robby Russell’s repository
$ sh -c “$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Install the Powerline font to spice up your CLI with icons
$ sudo apt install fonts-powerline

Change theme from ‘robbyrussell’ to ‘agnoster’ for the legendary Oh-My-Zsh theme
$ nano ~/.zshrc

Find the ZSH_THEME variable and change it:ZSH_THEME="agnoster"    aussi le  alanpeabody

I don’t like it that the theme shows my username and host. To get rid of this, we change the directory to
$ cd ~/.oh-my-zsh/themes
Next we open the theme file for ‘agnoster’ in the editor
$ nano agnoster.zsh-theme
Now we can change the ‘Main prompt’. We don’t need to prompt_context in the function build_prompt(). Just comment out this line or remove it. At last, change the PROMPT variable to $(build_prompt).

Agnoster theme configuration     
To actually see the theme, you have to source your .zshrc file like this: source ~/.zshrc. If everything worked out fine, you should see something like the cover image!
Extra: Set zsh as our default shell. Execute this in your default shell, in most cases this will be bash. If you execute this command in zsh, it won’t change anything:
$ chsh -s $(which zsh)
Note: If you use sudo it will change the shell for root, but not for your working user. Besides that, make sure to logout and login again to see the changes.
Install Plugins
All plugins listed on the plugins Github page are pre-installed with Oh-My-Zsh at ~/.oh-my-zsh/plugins. Custom plugins can be installed at ~/.oh-my-zsh/custom/plugins. To use a plugin, you can simply add it to the plugins list in your ~/.zshrc file. Add wisely, as too many plugins slow down shell startup. Leave a blank between each plugin.

Colored-man-pages
In this example, I’ve installed a useful plugin to give color highlighting to your man pages . To be able to use the plugin, source your .zshrcfile:
$ source ~/.zshrc




