# Configuration Vm

## Le grimoire

https://slack-files.com/files-pri-safe/TNAK3NVEG-FQPBALU8M/le_grimoire_du_t__l__porteur_-_temporaire.pdf?c=1575491030-a021fc82ff1c0d0ca57cfdeb2c1823537debba3a

## Maj vscode

pour le liveshare, il faudra mettre à jour Vscode, pour cela : 

```
sudo oclock-apt-enable
sudo apt-get update
sudo apt-get install code
sudo oclock-apt-disable
```

## Configurer php pour afficher les bonnes erreurs 

https://github.com/O-clock-Alumni/fiches-recap/blob/master/php/config.md

En résumé, il faut que `display_errors = On`  et `error_reporting = E_ALL`  dans le php.ini soit comme montré ici(son emplacement dépend de la version exact de php) -> `php -v`

## Installer Xdebug ( By William et Aurélien ) 

Je propose un petit tutoriel complémentaire à celui qui figure parmi les fiches récapitulatives sur Github, trouvable ci-dessous pour ceux et celles qui souhaiteraient installer Xdebug et / ou qui n'ont pas réussi à le faire :
https://github.com/O-clock-Alumni/fiches-recap/blob/master/php/xdebug.md

J'en profite en outre pour condenser ce dernier en le résumant par les lignes de commandes à saisir dans votre terminal, histoire de n'avoir que l'essentiel :

`sudo oclock-apt-enable`
`sudo apt-get update`
`sudo apt install php-pear`
`sudo apt install php7.2-dev` 
(après un php -v pour vérifier votre version de PHP, mais tout le monde devrait avoir la 7.2 en principe)

`pecl version` 
(vérification de la version ici également)
`sudo pecl install xdebug`
`sudo code /etc/php/X.x/apache2/conf.d/xdebug.ini` 
(je l'ai fait avec nano, mais normalement la commande ouvrira le fichier xdebug.ini dans VSCode)
Le contenu suivant est à copier-coller dans xdebug.ini (n'oubliez pas de faire Ctrl + S pour sauvegarder les modifications) :

`zend_extension=/usr/lib/php/20170718/xdebug.so
[XDebug]
xdebug.remote_enable = 1
xdebug.remote_autostart = 1`

## Configurer la clé ssh github

https://github.com/O-clock-Alumni/fiches-recap/blob/master/ldc/git.md#cr%C3%A9er-une-cl%C3%A9-ssh-pour-github


## Installer Composer, Vardumper, AltoRouter, AltoDispatcher

https://github.com/arnaud35300/RecapController

## Corriger les erreurs PhpMyAdmin


## Les extensions VScode utiles

Pour les commande suivantes, faites Ctrl+p et collez : 

- `ext install HookyQR.beautify` : https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify
- `ext install mrmlnc.vscode-autoprefixer` : https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-autoprefixer
- `ext install rifi2k.format-html-in-php` : https://marketplace.visualstudio.com/items?itemName=rifi2k.format-html-in-php
- `ext install ritwickdey.LiveServer` : https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer
- `ext install MS-vsliveshare.vsliveshare-pack` : https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack
- `ext install yzhang.markdown-all-in-one` : https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one
- `ext install Equinusocio.vsc-material-theme` : https://marketplace.visualstudio.com/items?itemName=Equinusocio.vsc-material-theme (le thème des bg)
- `ext install coderfee.open-html-in-browser` : https://marketplace.visualstudio.com/items?itemName=coderfee.open-html-in-browser
- `ext install neilbrayfield.php-docblocker` : https://marketplace.visualstudio.com/items?itemName=neilbrayfield.php-docblocker
- `ext install phproberto.vscode-php-getters-setters` : https://marketplace.visualstudio.com/items?itemName=phproberto.vscode-php-getters-setters
- `ext install bmewburn.vscode-intelephense-client` : https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client
- `ext install thibaudcolas.stylelint :` https://marketplace.visualstudio.com/items?itemName=thibaudcolas.stylelint
- `ext install calvinhong.stylelint-fix` : https://marketplace.visualstudio.com/items?itemName=calvinhong.stylelint-fix
- `ext install vscode-icons-team.vscode-icons` : https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons


