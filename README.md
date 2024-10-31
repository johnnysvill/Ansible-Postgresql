# Ansible-Postgresql
# Установка и конфигурирование PostgreSQL на Debian 11

Этот проект предназначен для автоматизации процесса установки и конфигурирования PostgreSQL 16 на сервере с операционной системой Debian 11 с помощью Ansible. Он включает в себя необходимые шаги для настройки сервера, изменения методов аутентификации, создания базы данных и пользователей.

Для развертывания проекта необходимо на Debian 11:
1. Установить ssh
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install openssh-server -y
sudo systemctl start ssh
```
2. Убедиться, что имеется доступ к серверу Debian по ssh через пароль или ключи
3. Установить ansible
```bash
sudo apt install ansible -y
```
4. Установить git
```bash
sudo apt install git -y
```
5. Настроить файл inventory, установив адрес своего хоста, имя и пароль пользователя 
6. Клонировать репозиторий на сервер:
```bash
git clone https://github.com/johnnysvill/Ansible-Postgresql.git
```
Войти в директорию скачанного репозитория:
```bash
cd Ansible-Postgresql
```
7. Запустить playbook:
```bash
ansible-playbook playbook.yml
```
