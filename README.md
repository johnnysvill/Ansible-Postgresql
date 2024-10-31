# Ansible-Postgresql
# Установка и конфигурирование PostgreSQL на Debian 11

Этот проект предназначен для автоматизации процесса установки и конфигурирования PostgreSQL 16 на сервере с операционной системой Debian 11 с помощью Ansible. Он включает в себя необходимые шаги для настройки сервера, изменения методов аутентификации, создания базы данных и пользователей.

Для развертывания проекта необходимо на Debian 11:
1. Установить ssh
sudo apt update
sudo apt install openssh-server -y
sudo systemctl start ssh
3. Убедиться, что имеется доступ к серверу Debian по ssh через пароль или ключи
4. Установить ansible
sudo apt install ansible -y
5. Установить git
sudo apt install git -y.
6. Настроить файл inventory, установив адрес своего хоста, имя и пароль пользователя 
7. Клонировать репозиторий на сервер:
git clone https://github.com/johnnysvill/Ansible-Postgresql.git
Войти в директорию скачанного репозитория:
cd Ansible-Postgresql
8. Запустить playbook:
ansible-playbook playbook.yml
