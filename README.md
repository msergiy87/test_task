# test_task

Опреаційна система - Ubuntu 14.04
Інструмент - Ansible
Web server - Apache
Database - Mysql

ansible-playbook -i hosts test_task.yml

Проводиться початкова конфігурація сервера.
Встановлюється і налаштовується Apache2, Mysql, php, pfoftpd, завантажуються дані сайту і дамп бази. Все на одній віртуальній машині.
Також встановлюється zabbix agent, налаштований для автореєстрації на zabbix сервері.

На іншій віртуальній машині власним скриптом встановлюється zabbix server 3
https://github.com/msergiy87/zabbix-install

На ньому вручну необхідно налаштувати умови автореєстрації і необхідні link to templates для отримання бажаних даних.
