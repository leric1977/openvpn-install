# OpenVPN Install — редакция leric1977

Скрипт автоматической установки и управления сервером OpenVPN для Linux.

Репозиторий основан на проекте
[Nyr/openvpn-install](https://github.com/Nyr/openvpn-install)
и сохраняет совместимость с оригинальным установочным скриптом.

## Поддерживаемые системы

- Debian
- Ubuntu
- AlmaLinux
- Rocky Linux
- CentOS
- Fedora

Скрипт необходимо запускать от имени пользователя `root`.

## Быстрая установка

Загрузите и запустите скрипт:

```bash
wget https://raw.githubusercontent.com/leric1977/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh
```

Установка одной командой:

```bash
wget -qO openvpn-install.sh https://raw.githubusercontent.com/leric1977/openvpn-install/master/openvpn-install.sh && chmod +x openvpn-install.sh && ./openvpn-install.sh
```

Альтернативный вариант с использованием `curl`:

```bash
curl -O https://raw.githubusercontent.com/leric1977/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh
```

## Управление OpenVPN

После первоначальной установки повторно запустите скрипт:

```bash
./openvpn-install.sh
```

С помощью меню можно:

1. создать нового клиента;
2. отозвать существующий клиентский сертификат;
3. удалить OpenVPN;
4. выйти из программы.

## Обновление локальной копии

Если репозиторий уже склонирован:

```bash
cd /opt/openvpn-install
git pull origin master
```

## Синхронизация с оригинальным проектом

В локальной копии настроены два источника:

- `origin` — пользовательская редакция `leric1977/openvpn-install`;
- `upstream` — оригинальный проект `Nyr/openvpn-install`.

Получение последних изменений оригинального проекта:

```bash
cd /opt/openvpn-install
git fetch upstream
git log --oneline --decorate --graph --all -20
```

Изменения из оригинального проекта рекомендуется объединять только после проверки совместимости с редакцией `leric1977`.

## Восстановление исходной версии

Перед внесением пользовательских изменений было сохранено исходное состояние:

```text
nyr-original-2026-07-20
```

Просмотреть его можно командой:

```bash
git show nyr-original-2026-07-20
```

## Происхождение проекта

- автор оригинального проекта: Nyr;
- оригинальный репозиторий: `Nyr/openvpn-install`;
- пользовательская редакция: `leric1977/openvpn-install`.

## Лицензия

Проект распространяется по лицензии MIT.

Оригинальный текст лицензии сохранён в файле
[`LICENSE.txt`](LICENSE.txt).
