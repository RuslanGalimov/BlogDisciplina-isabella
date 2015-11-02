# BlogDisciplina-isabella
Войдите на сервер Ghost и перейдите к каталогу themes:

cd /var/www/ghost/content/themes/

Для установки темы в этот каталог используйте git.

Примечание: Чтобы установить git, используйте:

apt-get update && apt-get install git-core -y

Затем клонируйте тему с GitHub:

git clone https://github.com/polygonix/***.git

Передайте права на файлы пользователю и группе Ghost:

chown -R ghost:ghost isabella

Перезапустите Ghost, чтобы обновить содержимое каталога themes:

service ghost restart

Откройте браузер и перейдите на страницу общих настроек:

your_domain_name/ghost/settings/general

Прокрутив вниз, найдите раздел Theme. Измените тему на isabella. Затем нажмите кнопку Save в верхнем правом углу экрана.
Теперь откройте блог, чтобы просмотреть изменения.

а вообще все расписано на сайте digitalocean.com 
https://www.digitalocean.com/community/tutorials/how-to-change-themes-and-adjust-settings-in-ghost
