OpenVPN Install — редакция leric1977

Скрипт автоматической установки и управления сервером OpenVPN для Linux.

Репозиторий основан на проекте Nyr/openvpn-install и сохраняет совместимость с оригинальным установочным скриптом.

Поддерживаемые системы
Debian
Ubuntu
AlmaLinux
Rocky Linux
CentOS
Fedora

Скрипт необходимо запускать от имени пользователя root.

Быстрая установка
wget https://raw.githubusercontent.com/leric1977/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh

Также можно выполнить одной командой:

wget -qO openvpn-install.sh https://raw.githubusercontent.com/leric1977/openvpn-install/master/openvpn-install.sh && chmod +x openvpn-install.sh && ./openvpn-install.sh
Управление OpenVPN

После первоначальной установки повторно запустите скрипт:

./openvpn-install.sh

С помощью меню можно:

создать нового клиента;
отозвать существующий клиентский сертификат;
удалить OpenVPN;
выйти из программы.
Обновление скрипта

Если репозиторий уже склонирован:

cd /opt/openvpn-install
git pull origin master
Синхронизация с оригинальным проектом

В локальной копии настроены два источника:

origin — репозиторий leric1977/openvpn-install;
upstream — оригинальный репозиторий Nyr/openvpn-install.

Получение последних изменений оригинального проекта:

cd /opt/openvpn-install
git fetch upstream
git log --oneline --decorate --graph --all -20

Изменения из оригинального проекта следует объединять только после проверки совместимости с редакцией leric1977.

Происхождение проекта

Основано на проекте:

автор оригинального проекта: Nyr;
оригинальный репозиторий: Nyr/openvpn-install;
пользовательская редакция: leric1977/openvpn-install.
Лицензия

Проект распространяется по лицензии MIT.

Оригинальный текст лицензии сохранён в файле LICENSE.txt.