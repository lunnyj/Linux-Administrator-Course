# OTUS-Linux-Administrator

Репозиторий будет обновляться по мере выполнения домашних заданий. Папки с наименованием домашнего задания выделены **bold**.

- **kernel_update** - Обновление ядра ОС
  - С репозитория elrepo
  - Из source kernel.org (Осторожно, образ весит ~ 5 Gb)

- **RAID** - Сборка софтверного RAID массива с помощью mdadm. Очень помогла статья [xgu.ru](http://xgu.ru/wiki/mdadm), судя по всему, методичка OTUS собиралась по ней.
  - Измененый Vagrantfile и bash скрипт сборки RAID10;
  - Vagrantfile, который собирается сразу с подключенным RAID;
  - Необходимо перенесети работающую систему с одним диском на RAID 1. Но пока не понимаю как делать, возможно потом получится.

- **LVM** - Работа с LVM разделами:
  - Уменьшение / раздела;
  - Зеркалирование раздела /var
  - Создание раздела /home
  - Снятие и разворот snapshot'а LVM раздела

- **Systemd** - Инициализация системы. Systemd и SysV:
  - Переписать unit файл запуска JIRA. Дз со *

- **Docker** - Работа с Dockerfile, docker-compose:
  - Создание кастомного образа nginx с Alpine. Загрузка в Dockerhub
  - Docker-compose с nginx и php-fpm

- **init** - работа с загрузчиком Linux:
  - Попасть в систему без пароля несколькими способами
  - Установить систему с LVM, после чего переименовать VG
  - Добавить модуль в initrd
